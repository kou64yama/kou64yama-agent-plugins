# kou64yama-agent-plugins

Reusable agent skills distributed as purpose-specific portable Agent Plugins.
The repository marketplace makes each plugin available separately. Plugin
versions are managed independently.

## Plugins

| Plugin                                                  | Description                                                                           |
| ------------------------------------------------------- | ------------------------------------------------------------------------------------- |
| [`conventional-commits`](plugins/conventional-commits/) | Write and review Conventional Commits messages.                                       |
| [`explain-artifacts`](plugins/explain-artifacts/)       | Explain artifacts in a self-contained HTML page.                                      |
| [`github-workflows`](plugins/github-workflows/)         | Create issues and pull requests and merge pull requests using repository conventions. |
| [`review`](plugins/review/)                             | Coordinate independent reviews and format pull request review comments.               |
| [`technical-writing`](plugins/technical-writing/)       | Apply technical writing principles to documentation and error messages.               |
| [`translation`](plugins/translation/)                   | Translation, proofreading, and multilingual reply workflows.                          |

## Installation

This repository adheres to the open [Agent Plugins](https://agent-plugins.org/)
standard and provides marketplaces for multiple agent environments.

### OpenAI Codex / ChatGPT

The repository includes a Codex marketplace manifest at
[`.agents/plugins/marketplace.json`](.agents/plugins/marketplace.json). In a
supported Codex CLI, add the repository as a marketplace and install the desired
plugin:

```sh
codex plugin marketplace add kou64yama/kou64yama-agent-plugins
codex plugin list --marketplace kou64yama-agent-plugins
codex plugin add translation@kou64yama-agent-plugins
```

Replace `translation` with any plugin name in the table. For local development,
run `codex plugin marketplace add .` from the repository root instead. The
marketplace can also be selected in the ChatGPT desktop app's Plugins Directory;
restart the app after adding a local marketplace. See the
[OpenAI plugin packaging documentation](https://developers.openai.com/plugins/build/plugins)
for supported clients and marketplace setup.

### Claude Code

The repository includes a Claude Code marketplace manifest at
[`.claude-plugin/marketplace.json`](.claude-plugin/marketplace.json). In a
Claude Code session, add the marketplace and install plugins:

```sh
/plugin marketplace add kou64yama/kou64yama-agent-plugins
/plugin install translation@kou64yama-agent-plugins
```

For local development or testing, add the local directory as a marketplace:

```sh
/plugin marketplace add .
```

### GitHub Copilot

The repository includes a Copilot marketplace manifest at
[`.github/plugin/marketplace.json`](.github/plugin/marketplace.json). In a
supported GitHub Copilot client, add the repository as a marketplace:

```sh
gh copilot plugin marketplace add kou64yama/kou64yama-agent-plugins
gh copilot plugin install translation@kou64yama-agent-plugins
```

For local development, add the local directory as a marketplace instead:

```sh
gh copilot plugin marketplace add .
```

### Google Antigravity (`agy`)

Antigravity automatically discovers customizations in `.agents/` or via explicit
manifests (`plugins.json` / `skills.json`). To use plugins from this repository
in an Antigravity project:

- Reference the plugin in your project's `.agents/plugins.json`:
  ```json
  {
    "entries": [
      { "path": "path/to/kou64yama-agent-plugins/plugins/translation" }
    ]
  }
  ```
- Or place this repository (or desired plugins) under `.agents/plugins/`.

---

The former `npx skills add` repository-wide installation has not been verified
with this layout. Use the plugin marketplace for distribution.

## Usage

After installation, reference a skill by name in a request, for example:

```text
Use $translate to help with this task.
```

Some skills include agent-specific metadata under `agents/`.

## Repository layout and development

This repository uses [Microsoft APM](https://github.com/microsoft/apm) as the
Single Source of Truth (`apm.yml`) for managing plugin metadata and generating
cross-platform marketplaces.

```text
apm.yml                              # Single Source of Truth for plugins & marketplaces
.agents/plugins/marketplace.json     # Generated: Codex marketplace manifest
.claude-plugin/marketplace.json      # Generated: Claude Code marketplace manifest
.github/plugin/marketplace.json      # Generated: GitHub Copilot marketplace manifest
plugins/
  <plugin-name>/
    plugin.json                      # Agent Plugins standard manifest
    .claude-plugin/plugin.json       # Claude Code manifest
    skills/
      <skill-name>/
        SKILL.md
        agents/
        references/  # optional
        assets/      # optional
```

Each plugin owns its skills and portable root `plugin.json`. Keep related skills
that use relative links together.

### Adding or updating plugins

1. Create or edit the plugin directory under `plugins/<plugin-name>/`.
2. Add or update the plugin definition in **`apm.yml`** under
   `marketplace.packages`.
3. Run the generator to rebuild all marketplace manifests:
   ```sh
   apm pack
   # or via npm
   npm run build:marketplaces
   ```
4. Verify the manifests are in sync:
   ```sh
   npm run check:marketplaces
   ```
5. Update the table above and increment the affected plugin's version when
   releasing changes.

When changing a skill, check its trigger, workflow, metadata, and relative
links. After changing a plugin, refresh its installed copy and restart the
client before testing discovery and behavior.

## Consuming this repository as an APM dependency

External projects can depend on individual plugins from this repository using
[APM](https://github.com/microsoft/apm). Each plugin lives in its own directory,
so reference the repository and select the plugin with `path`:

```yaml
dependencies:
  apm:
    - git: github.com/kou64yama/kou64yama-agent-plugins
      path: plugins/translation
    - git: github.com/kou64yama/kou64yama-agent-plugins
      path: plugins/conventional-commits
      # add more plugin paths as needed
```

Then run `apm install` to fetch the declared plugins into your project.

You can also install a plugin directly from the command line:

```sh
apm install kou64yama/kou64yama-agent-plugins/plugins/translation
```

Alternatively, register the repository marketplace and install by plugin name:

```sh
apm marketplace add kou64yama/kou64yama-agent-plugins
apm install translation@kou64yama-agent-plugins
```

### Release tags

Releases follow the `v{version}` tag convention (e.g. `v1.0.0`). Pin to a tag
for reproducible installs:

```yaml
dependencies:
  apm:
    - git: github.com/kou64yama/kou64yama-agent-plugins
      path: plugins/translation
      ref: v1.0.0
```

For a marketplace install, pin the marketplace registration to the tag:

```sh
apm marketplace add kou64yama/kou64yama-agent-plugins#v1.0.0
```

## License

MIT. See [LICENSE](./LICENSE) for details.
