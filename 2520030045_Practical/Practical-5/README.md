# OS Lab 5 – Anonymous Pipes

## Files
- producer_consumer.c
- pipe_exec.c

## Compile and Run

### Producer–Consumer Program
```bash
nano producer_consumer.c
gcc producer_consumer.c
./a.out
```

### Pipe Execution Program
```bash
nano pipe_exec.c
gcc pipe_exec.c
./a.out
```

## Description

**producer_consumer.c**
- Parent process produces data.
- Child process consumes data using an anonymous pipe.
- Demonstrates inter-process communication.

**pipe_exec.c**
- Implements the shell command:
  `ls -l | grep ".c"`
- Uses `fork()`, `pipe()`, `dup2()`, and `exec()`.

## System Calls Used
- `fork()`
- `pipe()`
- `dup2()`
- `exec()`
- `wait()`
