---
source: https://developers.google.com/tech-writing/error-messages/want-to-play-a-game.md.txt
---

# Want to play a game?

<br />

Challenge yourself by answering these five questions.

## Question 1

The following error message is supposed to target non-technical users:

- You entered a bad age (32.6)

If you were reviewing this error message, which replacement error message would
you recommend instead? The specified age, 32.6, contains a decimal point. Enter
an age that doesn't contain a decimal point. For example: 32 This answer
demonstrates how to correct the problem. The wording is appropriate for the
target audience. The specified age, 32.6, is a floating-point number instead of
an integer. The terms "floating-point number" and "integer" aren't ideal for an
audience of non-technical users, so the error message doesn't really demonstrate
how to correct the problem. You entered an age, 32.6, that our software can't
process. This error message doesn't demonstrate how to correct the problem, or
even explain what the problem is.

## Question 2

Which one of the following error messages would be best for application
programmers? The call read_file(my_input_stream) failed because my_input_stream
does not exist. To open a stream for reading, call the open_file function. For
example: my_input_stream = open_file("\~/.bashrc"). This error message explains
the problem and the solution. Also, the solution provides an example. You forgot
to open my_input_stream. This error message blames the user. Also, this error
message doesn't provide a solution. my_input_stream doesn't exist. Open
my_input_stream before calling read_file. This error message is so concise that
some helpful information (for example, how to open an input stream) has been
excluded.

## Question 3

What problem do you see in the following error message:

- The file you are attempting to upload is too big (12 MB). Please pick a
  smaller file and try again. The problem statement is missing the maximum
  allowable file size. This error message should have been:

The file you are attempting to upload is too big (12 MB). You can only upload
files that are 8MB or smaller. Please pick a smaller file and try again. The
error message doesn't provide a solution to the problem. Actually, the error
message does provide a solution. The error message contains a double negative.
This error message doesn't contain a double negative.

## Question 4

What problem do you see in the following error message:

- The specified file ('camelia.txt') does not exist. Pick a different datastore
  and try again. The first sentence and second sentence use different terms for
  the same kind of object. The first sentence uses the term \*file\*. The second
  sentence calls the same object a \*datastore\*. This error message will likely
  confuse some users. The error message doesn't specify the problem. Actually,
  the first sentence of the error message does specify the problem. The error
  message blames the user. The error message doesn't blame anyone. The error
  message is overly apologetic. The error message doesn't apologize.

## Question 5

Consider the following error message displayed for a consumer appliance:

- Error: Bad checksum. Change the battery in this device.

What error message would be more appropriate for a consumer appliance? The
battery is starting to fail. Replace the battery as soon as possible by
following these directions: \<_URL of battery replacement documentation_\> This
error message explains the problem in an appropriate way for nontechnical
people. A full description of how to change a battery is probably too detailed
for an error message, so providing the URL of full documentation is wiser.
(Also, if the battery is removed, the user cannot read the directions in an
error message.) Your device has reported a bad checksum. Change the battery in
this device. Very few people know what "bad checksum" means, so this phrase will
just annoy and confuse most people. The battery is starting to fail. Replace the
battery as soon as possible by following these directions:

1. Turn off the device by moving the switch from 1 to 0.
2. Unlatch the battery case located in the rear of this device. ...
3. Turn the device back on by moving the switch from 0 to 1. If the directions
   for replacing the battery were two steps instead of ten steps, then putting
   battery replacement instructions inside the error message might be okay.
   However, for a ten-step process, it is probably wiser to refer users to
   complete documentation that contains illustrations or videos. (Also, if the
   battery is removed, the user cannot read the directions appearing in the
   error message.) The error message is fine as is. This error message doesn't
   describe the problem appropriately for the target audience. The description
   of the solution isn't adequate.

<br />

<br />

**Next unit:** [Summary](./technical-writing-error-messages-15-summary.md)
