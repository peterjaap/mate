ABOUT
'mate' is a command line toolkit for Magento developers. It was written in a few hours to tackle the most repetitive tasks. 'mate' is written by Peter Jaap Blaakmeer.

INSTALLATION
Put the file in a convenient location (like /var/scripts) and name it 'mate' or 'mate.sh' (or whatever you'd like). Open your ~/.bashrc and put in an alias like so;
alias mate='/var/scripts/mate'

Reload your bash; 'source ~/.bashrc'.

USAGE
Go to the root of a Magento installation and run 'mate'. It'll give a warning if you are in the wrong dir. Otherwise, it'll output a list of commands you can use.
Certain commands of mate (such as 'compiler' and 'indexer') are just piped to the existing equivalent file (shell/compiler.php and shell/indexer.php).

CONTACT
GitHub: https://github.com/peterjaap/mate
Twitter: https://twitter.com/PeterJaap
Email: peterjaap@elgentos.nl