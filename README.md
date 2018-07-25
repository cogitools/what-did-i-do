# WhatDidIDo

A php package to help developers figure out what they did so they can put it on their timesheet.

WhatDidIDo collects your commit subjects to copy/paste into your time tracker.
The commits are assembled into single-line text blocks for each day.
This makes it very easy to select the text.

*Pro tip*: try tripple clicking the text on a Mac - it selects the whole line.

## Installation

`composer global require cogitools/whatdidido`

More details coming soon.

## WhatDidIDo Parameters

Default (no parameter)  
    Display 2 days worth of commits (yesterday & today).  
    This is the most commonly needed set of commits.  

-y/--yesterday  
    Display just yesterday's commits.  

-t/--today  
    Display just today's commits.  

-m/--multiline  
    Display the commits with each subject on it's own line.  

-w/--with-body  
    Include the body of the commit as well as the subject.  

-b/--before <argument>  
    Display the commits before a particular date.  
    This parameter is passed through to git log.  

-a/--after <argument>  
    Display the commits after a particular date.  
    This parameter is passed through to git log.  

-s/--since <argument>  
    Display the commits since a particular date.  
    This parameter is passed through to git log.  

-u/--until <argument>  
    Display the commits until a particular date.  
    This parameter is passed through to git log.  

## Git Log Utility

This utility is a based on git log, which is an incredibly powerful repoting tool built right into git. If your reporting needs go beyond what we've provided here you should look into that, maybe starting with the [git log docs](https://git-scm.com/docs/git-log).

## Commit Harvester for Automated Commit Harvesting

WhatDidIDo is very useful for micro indy shops with no budget. But its biggest shortfall is that you have to go into each repo and run it to see what you did. If you're looking for a more complete, integrated, and automatic solution we've got [Commit Harvester](http://commitharvester.com). 

## License

Licensed under the [MIT](LICENSE) license.

## Cogitool Software

This package is another fine product of [Cogitools Software](http://cogitools.com).

