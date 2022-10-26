# hpc-na-kolenke
Some useful scripts for HPC and other installations, I use in production for different tasks

## borg-backup

Wrapper over borg (borgbackup) to automate regular backups. It uses config
file, so you can use one script for many computers and backup different sets
of dirs, use different retention policies, even use different backup schemes on
one computer for different dirs.

If you dont't want use config file, just write DIRS inside the script and run it
without config. Otrherwise run it like `borg-backup path-to-conf`.

### Prerequisites

- borg (borgbackup)
- jq, yq (apt/yum install jq; pip3 install yq)
- curl, grep

### Notes
First you need to create a borg repo like this:
    `borg init --encryption=repokey /path/to/repo`

Fill config file (see borg-example.conf), then execute script like this: `borg-backup path-to-conf`

To debug this script `export DEBUG=yes` before script run
