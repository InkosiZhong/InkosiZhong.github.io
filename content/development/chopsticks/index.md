---
title: "Chopsticks: Sequential Task Manager for Linux and MacOS"
draft: false
date: 2023-05-03
description: "I often run complex computing jobs on a single node. When I am ready to leave, and the submitted task has not yet finished, I still wanna append new tasks so that it has done more work when I come back. Therefore I build a task manager similar to SLURM, but in a serial execution style."
language: 'Python'
platform: 'Linux/MacOS'
link: 'https://github.com/InkosiZhong/Chopsticks'
tags:
  - Developments
---

![chopsticks2.gif](https://s2.loli.net/2024/03/13/3FoPRuJ6ViLhjY2.gif)

### Who need it

- If you use a single computing node, and often run complex computing jobs, limited by hardware bottlenecks (RAM size, GPU memory size, number of CPU cores, etc.)
- When you are ready to leave, and the tasks you have submitted has not yet finished running, but you still wanna append some new tasks so that it has done more work when you come back.

### Usage

Chopsticks supports 7 commands: redirect, submit, cancel, restart, ls, clean, quit, you can use them with  `cs`

#### cs reidirect

```bash
usage: cs redirect [--dst DST]

redirect: redirect the output

optional arguments:
  --dst DST   redirect destination
# Examples
cs redirect # redirect to current terminal
cs redirect --dst out # redirect the output into a file
cs redirect --dst /dev/pts/5 # redirect to a terminal
```

#### cs submit

```bash
usage: cs submit cmd [cmd ...]

submit: submit a new task

positional arguments:
  cmd         command you want to submit
# Examples
# if you have a add.py that input 2 args, such as
python test.py 0 1
# now you can submit them only by adding csubmit
cs submit python test.py 0 1
# Chopsticks will give you an unique id for this task
> [submit] id=0
```

#### cs cancel

```bash
usage: cs cancel [--id ID]

cancel: cancel a task by ID

optional arguments:
  --id ID     task ID you want to cancel
# Examples
cs submit python test.py 0 1
> [submit] id=0
cs submit python test.py 0 1
> [submit] id=1
cs cancal --id 1
> [cancel] id=1
```

#### cs restart

```bash
usage: cs restart --id ID

restart: restart a task by ID

optional arguments:
  --id ID     task ID you want to restart
# Example
cs submit python test.py 0 1
> [submit] id=0
cs cancel 0
> [cancel] id=0
cs restart 0
> [restart] id=0->1
```

#### cs ls

```bash
usage: cs ls [-l] [-p] [-n LATEST_N] [--done] [--not-done]

ls: list all tasks

optional arguments:
  -l, --long            show long info
  -p, --pid             show PID
  -n LATEST_N, --latest-n LATEST_N
                        show the latest n records
  --done                show the records that are already finished|crashed|cancelled
  --not-done            show the records that are still running|waiting
# Example
cs ls
>
  id  state      submit    command
----  ---------  --------  ------------------
   0  finished   22:35:02  python test.py 0 1
   1  cancelled  22:35:03  python test.py 0 1

cs ls -n 1 # the latest one
>
  id  state      submit    command
----  ---------  --------  ------------------
   1  cancelled  22:35:03  python test.py 0 1
   
cs ls -n 1 -l --done # the latest one that is done
>
  id  state      submit    start     end       duration        command
----  ---------  --------  --------  --------  --------------- ------------------
   1  cancelled  22:35:03  22:35:03  22:35:03  0 days 00:00:00 python test.py 0 1
```

#### cs clean

```bash
# Example
cs clean
> [clean] 2 tasks
cs ls
>
  id  state      submit    command
----  ---------  --------  ------------------
```

#### cs quit
```bash
usage: cs quit [-f]

cquit: quit the guard process

optional arguments:
  -f, --force  quit anyway, ignoring the running|waiting tasks
```