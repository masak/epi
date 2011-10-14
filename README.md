Like git, but for managing the workflow around an intentional application.

Don't have a clear view of what the subcommands will be yet, but this is
what should be possible/easy with the program:

* Adding new commands and events
* Editing old ones
* Adding a new test case
* Implementing code to pass test cases

The test cases are meant to be central to it all, so

* Saying "I want to implement this test" will set things up properly and
  take you to the relevant file and line in vim.

* Mentioning a new type of command, event, or attribute to a command or
  event will automatically trickle back into the model.

* Changes to the model automatically trickle back into the code, too.
  Maybe a yes/no question to confirm.

* It just keeps making git commits with excellent commit messages all the
  time through this.
