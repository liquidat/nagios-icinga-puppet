# nagios-icinga-puppet
Nagios/Icinga check to verify that Puppet client runs actually happened

## What to do with the check
The nrpe plugin must be copied to the monitoring client.

## How to use check_puppetagent
The plugin is an NRPE check and needs to be run on the monitoring client, thus the client which Puppetagent needs to be monitored.
```
$ python check_puppetagent --help
usage: check_puppetagent [-h] [-w WARN] [-c CRIT]

optional arguments:
  -h, --help            show this help message and exit
  -w WARN, --warn WARN  seconds after last Puppet run which issues a warning
  -c CRIT, --crit CRIT  seconds after last Puppet run which are critica
  ```
