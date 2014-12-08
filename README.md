Boundary Process Memory Plugin
------------------------------

Displays memory use (RSS) for specific processes. Use Regular Expressions to specify a process name, process full path, and/or the process current working directory. Currently only works for Linux based systems that support procfs (i.e. have a/proc directory). **Note**: to monitor processes with elevated priviledges requires running the meter as root, which is not recommended.

### Platforms
- Linux

#### Prerequisites
- node version 0.8.0 or later
- npm version 1.4.21 or later

### Plugin Setup

None

### Plugin Configuration Fields

|Field Name        |Description                                                                                                                                                                                                                                                    |
|:-----------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|Source            |The source to display in the legend for the memory data.                                                                                                                                                                                                       |
|Process Name Regex|A regular expression to match the name of the process.                                                                                                                                                                                                         |
|Process Path Regex|A regular expression to match the full path of the process.                                                                                                                                                                                                    |
|Process CWD Regex |A regular expression to match the current working directory of the process.                                                                                                                                                                                    |
|Reconcile option  |How to reconcile in the case that multiple processes match.  Set to First Match to use the first matching process, Parent to choose the parent process (useful if process is forked), or Longest Running to pick the process that has been running the longest.|

### Metrics Collected

|Metric Name   |Description                   |
|:-------------|:-----------------------------|
|Memory Process|Process specific memory usage.|




