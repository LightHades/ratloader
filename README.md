# ratloader

This is a Pentest tool which automates the process of payloads creations.
There are included the following formats:

Android (apk)
Windows (exe)
Linux (elf)
Mac (macho)
Php (php)
Python (py)
Bash (sh)
Perl (pl)

# Instalation
Run the following command as superuser:
~# bash install.sh

# End
Then, ratloader will be able to work, to run it, execute the file 'main.py', or the command 'ratloader'


# Errors
If you get an error while trying to create a payload for windows, it's because of your metasploit version... To update it type:
~# apt-get remove metasploit-framework
~# curl https://raw.githubusercontent.com/rapid7/metasploit-omnibus/master/config/templates/metasploit-framework-wrappers/msfupdate.erb > msfinstall && chmod 755 msfinstall && ./msfinstall
Or, for any other error envolving metasploit, maybe it's because of your database, to correct it, type:
~#  msfdb delete && msfdb init
