# Simple Cron Handling

## Objective

Scheduling crons can be a pain. Especially if you are unfamiliar with how to schedule them. The objective is to eliminate all and any uncertainty in the preparation and scheduling of your scripts.

## Setup

### Files

Locate where you want to drop the cron_schedulers folder. Once done, get the directory (you can type pwd to get the current directory). Record this directory somewhere safe.

#### Example Case:
/var/www/html/automation/cron_schedulers

### Your Scripts

Locate where you store your current set of scripts. Ideally, this is kept in a single location, and this repository assumes you do so. Locate where you keep them. You can use the pwd command once you find it. Record this directory somewhere safe.

#### Example Case:
/var/www/html/automation

### Cron Setup

In the cron file, you will find the text that you need. You will want to update the variables AUTO_CRON_SCHEDULER_PATH and TARGET_SCRIPT_PATH to the directories you have saved. Copy all of the ones you wish to use. Safe and restart crontab.

#### Example Case:
AUTO_CRON_SCHEDULER_PATH=/var/www/html/automation/cron_schedulers
TARGET_SCRIPT_PATH=/var/www/html/automation

### Script Usage

In your .sh files, you may drop in new scripts you'd like to use, or directly write in the jobs you'd like them to do. Do try to consider best cron practices in writing your scripts.

## Notes

Every script that is "further" along on the scheduling is defaulted to start on the first of that time, may it be minute, hour, day, etc.


### Parting Message

I hope that this makes your cron handling easier to handle in the future! Happy coding!