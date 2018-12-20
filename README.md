# Ansible Backup
Ansible playbook to set up hosts with backup support (group backup_slave) and backup targets which support backup (group backup_master). Each backup slave can have multiple sources. 

A shell script is generated to backup all slaves. USB backup devices can be configured with their unique identifier and backup will start automatically if USB device is plugged into any backup master.

rsync is being used to support incremental backup, all rsync options are configurable for each backup slave.
