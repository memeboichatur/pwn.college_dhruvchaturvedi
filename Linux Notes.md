### **Hello Hackers:**

cat reads a file

echo prints



### **Pondering Paths:**

the parent(biggest) directory is called the root dir

/usr -(unix system resource) contains all system files

/usr/bin contains all executable files on the comp

/user/lib contains shared libraries

/usr/share contains program resources

/home contains user onwed data

/tmp contains runtime process data



cd -> change dir

cd / -> go back to root dir

cd home -> go to home dir

pwd -> print working directory

ls -> list files in dir



absolute paths start with / (root)

relative paths don't start with / and are relative to current working dir

/. signifies current dir (used for specifying navigation for run commands etc)

/.. signifies going up one dir



The ~ in the prompt is the current working directory, with ~ being shorthand for /home/hacker.

Whenever bash sees ~ provided as the start of an argument in a way consistent with a path, it will expand it to your home directory



expansion of ~ is a relative path and only the leading ~ is expanded



### **Comprehending Commands:**

the cat command also concatenates multiple files if needed

the cat command can also run files from any given directory



grep - we have the grep command to search for what we need

grep can be used to search a string using: grep SEARCH\_STRING /path/to/file , where SEARCH\_STRING is the string you want to search.



diff - compares two files line by line and shows you exactly what's different between them

ls - is used to list files in a directory

ls -ld is used to give additional info about a file while listing it

touch - you can create a new, blank file by touching it with the touch command

rm - remove files with the rm command

mv- moves one file into another file



hidden files- interestingly, ls doesn't list all the files by default. Linux has a convention where files that start with a . don't show up by default in ls and in a few other contexts. To view them with ls, you need to invoke ls with the -a flag



mkdir - makes directories

find - The find command takes optional arguments describing the search criteria and the search location. If you don't specify a search criteria, find matches every file. If you don't specify a search location, find uses the current working directory (.)
we can use find -name to search a file by name.



symbolic links- they are accessed by ln -s <original file> <link location>
file - the file command lets us know the type of file, including symbolic links

man - the man command stands for manual and will display the manual of the command you pass. (press q to quit)
You can scroll man pages with the arrow keys (and PgUp/PgDn) and search with /. After searching, you can hit n to go to the next result and N to go to the previous result. Instead of /, you can use ? to search backwards!

the -h command can further help with usage of commands 

