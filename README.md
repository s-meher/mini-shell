# mini-shell

A Unix-style shell implemented in C with support for foreground/background job execution, signal handling, and basic job control.

## Overview

`mini-shell` is a systems programming project that recreates core shell behavior in C. It reads user commands, launches processes, tracks active jobs, and handles signals to manage foreground and background execution safely.

The project was built to strengthen my understanding of process control, signal handling, and the execution model behind Unix-like shells.

## Features

- Execute external commands
- Foreground and background job execution
- Built-in commands:
  - `quit`
  - `jobs`
  - `bg`
  - `fg`
- Signal handling for process control
- Job tracking and state management

## Concepts Practiced

- C systems programming
- `fork`, `exec`, and `waitpid`
- Signal handling
- Foreground/background job control
- Process lifecycle management
- Debugging concurrent process behavior

## Build

```bash
make
```

## Run

```bash
./shell
```

## Example Usage

```bash
./shell
sleep 10
sleep 30 &
jobs
fg %1
quit
```

## Why I Built This

I built this project to get hands-on practice with operating systems concepts beyond the textbook level. Implementing a shell required careful thinking about how processes are created, how signals are delivered, and how a parent process coordinates multiple running jobs.

## Notes

This project is a compact showcase of systems programming fundamentals. It is not intended to be a full replacement for a production shell like `bash` or `zsh`.

## Tech

- C
- GCC
- Make

## Author

**Shree Meher**

- [GitHub](https://github.com/s-meher)
- [LinkedIn](https://www.linkedin.com/in/shree-meher/)
- [Portfolio](https://shree-portfolio-virid.vercel.app/)
