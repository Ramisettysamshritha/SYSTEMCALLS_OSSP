# OS Lab 4 – Process Synchronization and Zombie Process

## Files
- wait_compare.c
- zombie.c
- no_zombie.c

## Compile and Run

### wait() and waitpid()
```bash
nano wait_compare.c
gcc wait_compare.c
./a.out
```

### Zombie Process
```bash
nano zombie.c
gcc zombie.c
./a.out
```

### Remove Zombie Process
```bash
nano no_zombie.c
gcc no_zombie.c
./a.out
```

## Description

**wait_compare.c**
- Parent creates multiple child processes.
- Demonstrates synchronization using `wait()` and `waitpid()`.

**zombie.c**
- Creates a zombie process by allowing the child to terminate while the parent does not call `wait()` immediately.

**no_zombie.c**
- Eliminates the zombie process using proper synchronization with `wait()`.

## System Calls Used
- `fork()`
- `wait()`
- `waitpid()`
- `exit()`
- `sleep()`
