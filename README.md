plugin-process_memory
=====================

**\* LINUX ONLY \***

Displays memory use (RSS) for specific processes.
Use Regular Expressions to specify a process name, process full path, and/or the process current working directory.

As above, currently only works for Linux based systems that support procfs (i.e. have a /proc directory).
Note that to monitor higher privilege processes you may need to run the relay with sudo permissions.
