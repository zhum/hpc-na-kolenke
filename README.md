<<<<<<< HEAD
# hpc-na-kolenke
Some useful scripts for HPC and other installations, I use in production for different tasks

## borg-backup

Wrapper over borg (borgnackup) to automate regular backups. Uses config
files, so you can use one script for many computers and baclup different sets
of dirs, use different retention policies, even use different backup schemes on
one computer for different dirs.

If you dont't want use config file, just write DIRS inside the script and run it
without config. Otrherwise run it like `borg-backup path-to-conf`.
||||||| constructed merge base
# hpc-na-kolenke
=======
# Some useful (probably not for me only) scripts

## borg-backup

Wrapper over borg (borgbackup) to automate backups. Uses config file, so
you can use ONE script for different backups and hosts. See borg-example.conf.
Run it like borg-backup path-to-conf.

If you like, specify DIRSinside the script and do not specify config.


>>>>>>> first release: add borg-backup scripts
