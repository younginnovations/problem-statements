## Back'em up

### What you need to do

* If you haven’t used git before, take a [git class in codeschool](https://www.codeschool.com/courses/try-git).
* Once complete, create a private repo called “yipl-se-back-them-up” in [bitbucket](https://bitbucket.org)
* Solve the problem detailed below
* Push your code to the repo (make sure that you have multiple commits with proper messages) 
* Invite bitbucket@yipl.com.np to that particular private repo
* Submit your application

#### Problem

You need to write a script (in python or bash) that backs-up the database every day. The filenames should be named as follows `dbname-yyyy.mm.dd-day` and should be tar-gzipped. For example the database backed-up on Oct 24, 2016 should be dbname-2016.10.24-mon.tar.gz. 

Everytime the script runs, it should also check for files for deletion based on the following conditions. 

1. The files backed-up less than 7 days old should not be deleted.
2. If the files are more than 7 days old, then all the files other than the files backed up on last 4 fridays should be deleted.
3. For the files old than a month, all the files other than the one backed up on the last day of the month should be deleted.

For eg, if the files have been backed up since October 2016 till Nov 24 2016. These should be the only files that should be present in the backup folder. 

>dbname-2016.09.30-thu.tar.gz

>dbname-2016.10.28-fri.tar.gz

>dbname-2016.10.31-mon.tar.gz

>dbname-2016.11.04-fri.tar.gz

>dbname-2016.11.11-fri.tar.gz

>dbname-2016.11.18-fri.tar.gz

>dbname-2016.11.19-sat.tar.gz

>dbname-2016.11.20-sun.tar.gz

>dbname-2016.11.21-mon.tar.gz

>dbname-2016.11.22-tue.tar.gz

>dbname-2016.11.23-wed.tar.gz

>dbname-2016.11.24-thu.tar.gz

The code should be written in any one of the following programming languages: python or bash. 

The filename should be: backup.py or backup.sh upon the language you choose.

In python, 
`python backup.py`

In bash,
`bash backup.sh`

If the above script is run on Nov 24, 2016 in the folder containing the following files, all the crossed-out files should be deleted except for the bold ones.

> **dbname-2016.09.30-thu.tar.gz**

> ~~dbname-2016.10.01-sat.tar.gz~~

> ~~dbname-2016.10.02-sun.tar.gz~~

> ~~dbname-2016.10.03-mon.tar.gz~~

> ~~dbname-2016.10.04-tue.tar.gz~~

> ~~dbname-2016.10.05-wed.tar.gz~~

> ~~dbname-2016.10.06-thu.tar.gz~~

> ~~dbname-2016.10.07-fri.tar.gz~~

> ~~dbname-2016.10.08-sat.tar.gz~~

> ~~dbname-2016.10.09-sun.tar.gz~~

> ~~dbname-2016.10.10-mon.tar.gz~~

> ~~dbname-2016.10.11-tue.tar.gz~~

> ~~dbname-2016.10.12-wed.tar.gz~~

> ~~dbname-2016.10.13-thu.tar.gz~~

> ~~dbname-2016.10.14-fri.tar.gz~~

> ~~dbname-2016.10.15-sat.tar.gz~~

> ~~dbname-2016.10.16-sun.tar.gz~~

> ~~dbname-2016.10.17-mon.tar.gz~~

> ~~dbname-2016.10.18-tue.tar.gz~~

> ~~dbname-2016.10.19-wed.tar.gz~~

> ~~dbname-2016.10.20-thu.tar.gz~~

> **dbname-2016.10.21-fri.tar.gz**

> ~~dbname-2016.10.22-sat.tar.gz~~

> ~~dbname-2016.10.23-sun.tar.gz~~

> ~~dbname-2016.10.24-mon.tar.gz~~

> ~~dbname-2016.10.25-tue.tar.gz~~

> ~~dbname-2016.10.26-wed.tar.gz~~

> ~~dbname-2016.10.27-thu.tar.gz~~

> **dbname-2016.10.28-fri.tar.gz**

> ~~dbname-2016.10.29-sat.tar.gz~~

> ~~dbname-2016.10.30-sun.tar.gz~~

> **dbname-2016.10.31-mon.tar.gz**

> ~~dbname-2016.11.01-tue.tar.gz~~

> ~~dbname-2016.11.02-wed.tar.gz~~

> ~~dbname-2016.11.03-thu.tar.gz~~

> **dbname-2016.11.04-fri.tar.gz**

> ~~dbname-2016.11.05-sat.tar.gz~~

> ~~dbname-2016.11.06-sun.tar.gz~~

> ~~dbname-2016.11.07-mon.tar.gz~~

> ~~dbname-2016.11.08-tue.tar.gz~~

> ~~dbname-2016.11.09-wed.tar.gz~~

> ~~dbname-2016.11.10-thu.tar.gz~~

> **dbname-2016.11.11-fri.tar.gz**

> ~~dbname-2016.11.12-sat.tar.gz~~

> ~~dbname-2016.11.13-sun.tar.gz~~

> ~~dbname-2016.11.14-mon.tar.gz~~

> ~~dbname-2016.11.15-tue.tar.gz~~

> ~~dbname-2016.11.16-wed.tar.gz~~

> ~~dbname-2016.11.17-thu.tar.gz~~

> **dbname-2016.11.18-fri.tar.gz**

> **dbname-2016.11.19-sat.tar.gz**

> **dbname-2016.11.20-sun.tar.gz**

> **dbname-2016.11.21-mon.tar.gz**

> **dbname-2016.11.22-tue.tar.gz**

> **dbname-2016.11.23-wed.tar.gz**

> **dbname-2016.11.24-thu.tar.gz**


### Further instruction

* Write readme file with the instructions necessary to run the code


### Bonus points

* If you can write and include unit tests for your code
