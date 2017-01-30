# boss
Brother of SPARTA - Linux performance monitoring and analytics toolkit.

Boss is an attempt to port some functionality delivered by SPARTA toolkit to Linux. Sparta was developed for Illumos by Jason Banham:
https://github.com/jasonba/sparta

There are vast differences in performance monitoring between Illumos and Linux so while some functionality is to be ported from SPARTA, the underlying tools will be different.

Some desired functionality:
- monitor and save cpu, memory and disk io statistics in files
- draw graphs from the above files
- run continuously or for defined period of time and quit
- define granularity
- monitor dcache
- monitor network statistics (netstat -s, bandwidth)
- monitor resource usage by processes (top)
- monitor single process 
- define file rotation policy

some commands to run:
   - mpstat -P ALL 1 > mpstat.out
   - vmstat -t 1 > vmstat.out
   - sar -u -P ALL -t  1 > sar.out
