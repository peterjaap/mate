# Mate - CLI toolkit for Magento #
## About ##
'mate' is a command line toolkit for Magento developers. It was written in a few hours to tackle the most repetitive tasks. 'mate' is written by Peter Jaap Blaakmeer.

## Installation ##
1) Put the file in a convenient location (like /var/scripts) and name it 'mate' or 'mate.php' or 'mate.sh' (or whatever you'd like).  
2) Then make it executable ('chmod +x mate'). Open your ~/.bashrc and put in an alias like so; alias mate='/var/scripts/mate'  
3) Reload your bash; 'source ~/.bashrc'.  

Or just place it in your $PATH.

## Usage ##
Go into the directory of a Magento installation (any level deep) and run 'mate'.  
It'll give a warning if you are not in a Magento tree. Otherwise, it'll output a list of commands you can use. Certain commands of mate (such as 'compiler' and 'indexer') are just piped to the existing equivalent file (shell/compiler.php and shell/indexer.php).

## Available commands ##
mate index/indexer <default indexer options> (run 'mate indexer options' to see all options)  
mate reindexall - shortcut for mate index reindexall  
mate compiler <default compiler options> (run 'mate compiler' to see all options')  
mate connect <default mage options> (run 'mate connect' to see all options)  
mate modules / mate mod - overview the module list  
mate enable Package_Module - enable a module  
mate disable Package_Module - disable a module  
mate toggle Package_Module - toggle the status of a module  
mate skeleton Package Module Version - create a skeleton module for development  
mate backup - make a database dump to database.sql  
mate import - import a backupped database  
mate events - list all events (for observers) found in the codebase/  
mate cc/cache - clear cache  
mate cs/session(s) - clear sessions  
mate cron - run the cron  
mate connect {arguments} - use default 'mage' exec to interface Magento Connect  
mate install channelName packageName - install packages using default 'mage' exec  
mate user - create an admin account, will prompt for username, pass, email and name  
mate passwd - change password for a user, will prompt for username & pass  
mate minstall {version} {sample} {db_name} - install Magento (use '1600' or '1.6.2.0' for {version}). Use 'sample' for {sample} to download sample data file. Give up db_name to automatically create database.  
mate resetmods - reset all permissions of dirs to 775 and files to 664  
mate devurl - set the secure & unsecure base url to {{base_url}} for during development  
mate hints (admin/scope id/leave empty) on/off - turn the template hints on and off for store or admin  
mate conflicts - looks through all third party modules and checks for possible conflicts  
mate events - look for all events that are available within this installation  
mate logs [enable/disable] / [on/off] - enable/disable logging to var/log/system.log  
mate backup - create a backup of the current database (saves to database.sql)  
mate import {filename} - import a backup into the current database (caution; will drop all tables). When filename is omitted, 'database.sql' is assumed  

## Changelog ##
28-10-2012: Added sample data option to 'mate minstall'  
23-10-2012: Added change password 'passwd' action  
10-10-2012: Added codepool & version to 'mate mod' listing & fixed minor bugs when using mate in a non-Magento environment  
14-08-2012: Added 'mate logs [enable/disable] / [on/off]' to enable/disable logging to var/log/system.log  
01-08-2012: Added 'mate conflicts' to look for conflicts between third party modules  
31-07-2012: Added 'mate devurl' to change the base URL to {{base_url}} for dev purposes  
31-07-2012: Added 'mate user' to create admin users & refactored the root discovery part to be able to use mate from anywhere within a Magento root dir  
23-04-2012: Added admin menu page to extension created by 'mate skeleton'  
12-04-2012: Added 'mate events' to get a list of all the events that are found in the codebase (credits go to Byte - http://www.byte.nl/blog/2012/02/03/how-to-list-all-events-in-magento)  
11-04-2012: Added 'mate log' to view the last 50 lines of system.log  
10-04-2012: Added 'mate import' to import a backupped database, tweaked 'skeleton' a bit  
30-03-2012: Added 'mate reindexall' as a shortcut for 'mate indexer reindexall'  
29-03-2012: Added 'mate skeleton' to quickly create a skeleton module for development  

## Contact ##
GitHub: https://github.com/peterjaap/mate  
Twitter: https://twitter.com/PeterJaap  
Email: peterjaap@elgentos.nl  

## License ##
Copyright (C) 2012 Elgentos

This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program.  If not, see <http://www.gnu.org/licenses/>.
