# A Kernel Seedling
A kernel seedling counts the number of processes being run on your laptop or computer.

## Building - In order to build the module
```shell
make
```

## Running - To run the program and print the output to the terminal
```shell
sudo insmod proc_count.c
cat /proc/count
```
results: 142

## Cleaning Up - In order to remove the previous build information
```shell
sudo rmmod proc_count.c
make clean
```

## Testing - In order to run the python script that tests the code
```python
python -m unittest
```
results:
Ran 3 tests in 7.469s

OK

Report which kernel release version you tested your module on
(hint: use `uname`, check for options with `man uname`).
It should match release numbers as seen on https://www.kernel.org/.

```shell
uname -r -s -v
```
kernel ver: Linux 5.14.8-arch1-1 #1 SMP PREEMPT Sun, 26 Sep 2021 19:36:15 +0000
