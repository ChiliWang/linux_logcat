# linux support android logger
## open config in linux kernel 
CONFIG_ANDROID_LOGGER=y

## then there will have below node in filesystem
 ls /dev/log*
/dev/log         /dev/log_main    /dev/log_system
/dev/log_events  /dev/log_radio


## test
logcat -v time &
logwrapper ls
logwrapper ps
