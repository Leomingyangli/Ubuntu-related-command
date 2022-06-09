# Ubuntu-related-command
## Create ubuntu user
```
sudo adduser username

# add user to sudo group
sudo usermod -aG sudo username

# list users in sudo group
grep -Po '^sudo.+:\K.*$' /etc/group 
```

## Check CPU configuration
```
htop
lscpu

#check pysical cpu
cat /proc/cpuinfo |grep "physical id"|sort |uniq|wc -l 

# check logical cpu
cat /proc/cpuinfo |grep "processor"|wc -l 

# check cores in each cpu
cat /proc/cpuinfo |grep "cores"|uniq 
```

## Check ubuntu version and GPU information
```
lsb_release -a
nvidia-smi
```

## Check disk space and memory usgae 
```
df -hl
free -g
```
