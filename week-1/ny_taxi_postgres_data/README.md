## NY Taxi PostgreSQL Data

This folder represents the volume of the docker container of the PostgreSQL Server that was run locally in a docker container. 

Below is the snapshot of the files as shown by command `ls -la` as of February 12, 2024 (user is censored):


```plaintext
total 92
drwxr-xr-x 1 user 197609     0 Feb 12 01:10 .
drwxr-xr-x 1 user 197609     0 Feb 11 02:23 ..
-rw-r--r-- 1 user 197609     3 Jan 21 23:51 PG_VERSION
drwxr-xr-x 1 user 197609     0 Jan 24 13:53 base
drwxr-xr-x 1 user 197609     0 Feb 10 23:02 global
drwxr-xr-x 1 user 197609     0 Jan 21 23:51 pg_commit_ts
drwxr-xr-x 1 user 197609     0 Jan 21 23:51 pg_dynshmem
-rw-r--r-- 1 user 197609  4782 Jan 21 23:51 pg_hba.conf
-rw-r--r-- 1 user 197609  1636 Jan 21 23:51 pg_ident.conf
drwxr-xr-x 1 user 197609     0 Feb 11 00:54 pg_logical
drwxr-xr-x 1 user 197609     0 Jan 21 23:51 pg_multixact
drwxr-xr-x 1 user 197609     0 Jan 21 23:51 pg_notify
drwxr-xr-x 1 user 197609     0 Jan 21 23:51 pg_replslot
drwxr-xr-x 1 user 197609     0 Jan 21 23:51 pg_serial
drwxr-xr-x 1 user 197609     0 Jan 21 23:51 pg_snapshots
drwxr-xr-x 1 user 197609     0 Feb 10 03:01 pg_stat
drwxr-xr-x 1 user 197609     0 Feb 12 01:09 pg_stat_tmp
drwxr-xr-x 1 user 197609     0 Jan 21 23:51 pg_subtrans
drwxr-xr-x 1 user 197609     0 Jan 21 23:51 pg_tblspc
drwxr-xr-x 1 user 197609     0 Jan 21 23:51 pg_twophase
drwxr-xr-x 1 user 197609     0 Feb 10 23:07 pg_wal
drwxr-xr-x 1 user 197609     0 Jan 21 23:51 pg_xact
-rw-r--r-- 1 user 197609    88 Jan 21 23:51 postgresql.auto.conf
-rw-r--r-- 1 user 197609 28156 Jan 21 23:51 postgresql.conf
-rw-r--r-- 1 user 197609    36 Feb 10 03:01 postmaster.opts
-rw-r--r-- 1 user 197609    94 Feb 10 03:01 postmaster.pid
total 92
drwxr-xr-x 1 user 197609     0 Feb 12 01:10 .
drwxr-xr-x 1 user 197609     0 Feb 11 02:23 ..
-rw-r--r-- 1 user 197609     3 Jan 21 23:51 PG_VERSION
drwxr-xr-x 1 user 197609     0 Jan 24 13:53 base
drwxr-xr-x 1 user 197609     0 Feb 10 23:02 global
drwxr-xr-x 1 user 197609     0 Jan 21 23:51 pg_commit_ts
drwxr-xr-x 1 user 197609     0 Jan 21 23:51 pg_dynshmem
-rw-r--r-- 1 user 197609  4782 Jan 21 23:51 pg_hba.conf
-rw-r--r-- 1 user 197609  1636 Jan 21 23:51 pg_ident.conf
drwxr-xr-x 1 user 197609     0 Feb 11 00:54 pg_logical
drwxr-xr-x 1 user 197609     0 Jan 21 23:51 pg_multixact
drwxr-xr-x 1 user 197609     0 Jan 21 23:51 pg_notify
drwxr-xr-x 1 user 197609     0 Jan 21 23:51 pg_replslot
drwxr-xr-x 1 user 197609     0 Jan 21 23:51 pg_serial
drwxr-xr-x 1 user 197609     0 Jan 21 23:51 pg_snapshots
drwxr-xr-x 1 user 197609     0 Feb 10 03:01 pg_stat
drwxr-xr-x 1 user 197609     0 Feb 12 01:09 pg_stat_tmp
drwxr-xr-x 1 user 197609     0 Jan 21 23:51 pg_subtrans
drwxr-xr-x 1 user 197609     0 Jan 21 23:51 pg_tblspc
drwxr-xr-x 1 user 197609     0 Jan 21 23:51 pg_twophase
drwxr-xr-x 1 user 197609     0 Feb 10 23:07 pg_wal
drwxr-xr-x 1 user 197609     0 Jan 21 23:51 pg_xact
-rw-r--r-- 1 user 197609    88 Jan 21 23:51 postgresql.auto.conf
-rw-r--r-- 1 user 197609 28156 Jan 21 23:51 postgresql.conf
-rw-r--r-- 1 user 197609    36 Feb 10 03:01 postmaster.opts
-rw-r--r-- 1 user 197609    94 Feb 10 03:01 postmaster.pid

