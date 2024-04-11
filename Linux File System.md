
<iframe width="100%" src="https://www.youtube-nocookie.com/embed/42iQKuQodW4?si=0RW2DL7_2w5V7PyP" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen style="border-radius: 4px; aspect-ratio: 16/9;"></iframe>

Directory System:
- BIN: binaries or executables (applications)
- SBIN: binaries or executables only for ROOT user
- LIB: shared binaries executables for BIN and SBIN
- USR/BIN: non-essential binaries or executables
- USR/LOCAL/BIN: manually compiled executables by user
	- Mapped to the $PATH variable so they can be executed anywhere in the system
- ETC: editable text configuration for customized configurations
- HOME: contains folders for each user that contain files, configurations, and software for said user
- BOOT: files for the boot system, includes the Linux kernel itself
- DEV: device files, drivers, hardware access, can create disk partitions
- OPT: Optional or add-on software
- VAR: variable files, logs and cache files, that change as the OS is used
- TMP: temporary files that are deleted between reboots
- PROC: virtual folder created in memory used to keep track of running processes