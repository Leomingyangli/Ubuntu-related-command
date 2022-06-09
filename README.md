# Ubuntu-related-command
## Create ubuntu user
'''
sudo adduser username
sudo usermod -aG sudo rui # add user to sudo group
grep -Po '^sudo.+:\K.*$' /etc/group # list users in sudo group
'''

## Check CPU configuration
'''
htop
lscpu
#check pysical cpu
cat /proc/cpuinfo |grep "physical id"|sort |uniq|wc -l 
# check logical cpu
cat /proc/cpuinfo |grep "processor"|wc -l 
# check cores in each cpu
cat /proc/cpuinfo |grep "cores"|uniq 
'''

## check ubuntu version and GPU information
'''
lsb_release -a
nvidia-smi
'''

## Check disk space and memory usgae 
'''
df -hl
free -g
'''
