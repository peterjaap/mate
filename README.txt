ABOUT
'mate' is a command line toolkit for Magento developers. It was written in a few hours to tackle the most repetitive tasks. 'mate' is written by Peter Jaap Blaakmeer.

INSTALLATION
Put the file in a convenient location (like /var/scripts) and name it 'mate' or 'mate.sh' (or whatever you'd like). Then make it executable ('chmod +x mate'). Open your ~/.bashrc and put in an alias like so;
alias mate='/var/scripts/mate'

Reload your bash; 'source ~/.bashrc'.

USAGE
Go to the root of a Magento installation and run 'mate'. It'll give a warning if you are in the wrong dir. Otherwise, it'll output a list of commands you can use.
Certain commands of mate (such as 'compiler' and 'indexer') are just piped to the existing equivalent file (shell/compiler.php and shell/indexer.php).

CHANGELOG
10-04-2012: Added 'mate import' to import a backupped database
30-03-2012: Added 'mate reindexall' as a shortcut for 'mate indexer reindexall' for lazy colleague @jhhazelaar
29-03-2012: Added 'mate skeleton' to quickly create a skeleton module for development

CONTACT
GitHub: https://github.com/peterjaap/mate
Twitter: https://twitter.com/PeterJaap
Email: peterjaap@elgentos.nl

LICENSE
Copyright (C) 2012 Elgentos

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program.  If not, see <http://www.gnu.org/licenses/>.