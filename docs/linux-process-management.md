# Linux Process Management

## Process Creation

The coursework used `fork()` to split execution into a parent process and a child process.

The child process could then use `execl()` to replace its current program with a Linux command such as:

- `ps`
- `date`
- `ls`

## Job Control

The module also covered Linux process-control concepts including:

- starting a process
- suspending a process
- running a process in the background
- returning a process to the foreground
- terminating a process
- keeping commands alive with `nohup`
- detaching jobs using `disown`
- persistent terminal sessions using `screen`
- repeated command execution using `watch`

## Analyst Relevance

During Linux investigations, process information can reveal:

- suspicious command execution
- unexpected child processes
- scripts launched by services
- persistence mechanisms
- long-running background processes

The coursework provided an early foundation for understanding those relationships.