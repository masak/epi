Like git, but for managing the workflow around an intentional application.

Some ideas for the subcommands:

    epi goto commands       -- edit model/commands.xsd
    epi goto events         -- edit model/events.xsd
    epi goto MyAggregate    -- edit lib/MyAggregate.pm
    epi goto -t MyAggregate -- edit t/myaggregate.t
    
    epi test MyAggregate    -- run t/myaggregate.t
    
    epi newtest MyAggregate -- add a test
    epi newtest MyAggregate -g Event1,Event2 -w Command3 -t Event4,Event4
                            -- add a test, events and commands pre-filled
    
    epi goto                -- edit file/line, DWIM based on recent events
    
    epi make                -- rebuild Makefile, run make

The test cases are meant to be central to it all, so

* Saying "I want to implement this test" will set things up properly and
  take you to the relevant file and line in vim.

* Mentioning a new type of command, event, or attribute to a command or
  event will automatically trickle back into the model.

* It just keeps making git commits with excellent commit messages all the
  time through this.
