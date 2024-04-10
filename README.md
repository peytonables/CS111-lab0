# A Kernel Seedling
A kernel seedling counts the number of processes being run on your laptop or computer.

## Building
```shell
make
```

## Running
```shell
sudo insmod proc_count.c
cat /proc/count
```
TODO: results? 

## Cleaning Up
```shell
sudo rmmod proc_count.c
make clean
```

## Testing
```python
python -m unittest
```
TODO: results?

Report which kernel release version you tested your module on
(hint: use `uname`, check for options with `man uname`).
It should match release numbers as seen on https://www.kernel.org/.

```shell
uname -r -s -v
```
TODO: kernel ver?