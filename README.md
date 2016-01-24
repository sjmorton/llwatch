# llwatch
Windows / DOS   Watch program execution similar to unix / linux watch command

LLWatch repeats execution of a DOS command and monitors its console output.
Optionally homing the cusor and highlighting changes. 


Help Banner:

LLWatch v1.1 - Jan 23 2016
By: Dennis Lang
https://landenlabs.com/

SUMMARY:
  Watch - execute a program periodically, showing output

USAGE:
  llwatch [-dhv] [-t #lines][-b #lines] [-n <seconds>] -- <command>

DESCRIPTION:  Watch runs command repeatedly, displaying its output. This allows you to
  Watch the program output change over time. By default, the program is run
  every 2 seconds. 

  -d  Disable highlighting the differences between successive updates.
  -h  Home cursor between updates
  -n <seconds> Specify update interval, default 2 seconds
  -t <#lines> Limit output to top # lines, default is 20
  -b <#lines> Limit output to bottom # lines, default is all
  -v  Toggle verbose output
  -g <pattern> Match grep pattern for line to show.
  -r <replace> Use with -g and perform replacement per line before show.

EXAMPLES:
    To watch the contents of a directory change, you could use:
       watch dir *.txt

    Use grep to filter command output
       watch "dir | grep -i jan"


