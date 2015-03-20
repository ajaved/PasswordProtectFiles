Abeer Javed 
Rice University
03/19/2015


To use, simply place script in folder in path (~/bin is good usually), change
script to be executable ('chmod 777 encrypt_files' gets the job done), then call 
from command line as detailed below.

Requires 7z be installed, which is in p7zip-full package.

Example input: encrypt_files -o sensitive_info -i recipes.pdf kill_list.docx
Creates a password protected 7z file with name that follows '-o' containing
files/directories specified after '-i'.
7z program queries user for password.

Currently, files/directory paths must be specified in relation to the current
directory (e.g. using ../../ etc.).
Output .7z file is saved in current directory.

Has not been tested on Windows systems.