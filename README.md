# CMPE-443-QEMU-GDP-BUNDLE

## run.sh
This is the installation script for docker image of the specialized QEMU in CmpE443

### How to Run:

### BELOW IS IMPORTANT:
- First, change directory to where your .axf file resides
### ABOVE IS IMPORTANT: 

- Then run the following:
```sh
./run.sh <your_axf_file_name>
```
- This should pull a Docker image from Docker Hub and run it with several parameters, to open QEMU right after pulling the image.

## gdb_pro.sh
This is the GNU Debugger downloader & installer to use with QEMU Docker image.

### How to Run:
```sh
./gdb_pro.sh
```

# PREFERRED RUNNING STRUCTURE:
- Open 2 terminal sessions concurrently and run `run.sh` in one of them at first and wait until it executes completely and you see a (QEMU) prompt.
- Then, switch to the other terminal and run `gdb_pro.sh` to connect with the running QEMU instance which is loaded with your .axf file.

# HOW TO EXIT:
- First, close gdb terminal session and switch back to the QEMU session.
- Type `q` and press Enter.
- Repeat the previous instruction until it works.

