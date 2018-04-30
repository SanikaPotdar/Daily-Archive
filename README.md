# Daily-Archive

### Introduction:

Nowhere is shell script programming more useful than writing script utilities for the Linux system administrator. The typical Linux system administrator has many various jobs to do daily, from monitoring disk space to backing up important files to managing user accounts. Shell script utilities can make these tasks much easier!
Whether you’re responsible for a Linux system in a business environment or just using it at home, the loss of data can be catastrophic. To help prevent bad things from happening, it’s always a good idea to perform regular backups (or archives).
However, what’s a good idea and what’s practical are often two separate things. Trying to arrange a backup schedule to store important files can be a challenge. This is another place where shell scripts often come to the rescue.

### Working:

If you’re using your Linux system to work on an important project, you can create a shell script that automatically takes snapshots of specific directories. Designating these directories in a configuration file allows you to change them when a particular project changes. This helps avoid a time-consuming restore process from your main archive files.
The automated shell script that can take snapshots of specified directories and keep an archive of your data’s past versions. The snapshots are compressed versions of the files / directories (.tar.gz files) marked by the time of archive.

If you are just backing up a few files, it’s fine to keep the archive in your personal directory. However, if several directories are being backed up, it is best to create a central repository archive directory. Instead of modifying or creating a new archive script for each new directory or file you want to backup, you can use a configuration file. You can have the script read through the configuration file and add the names of each directory to the archive list. Thus we create a central configuration file and keep adding files in it which we want to archive via a loop. The script must also check whether the file to be archived exists in the system or not.
 The Daily_Archive.sh script automatically creates an archive to a designated location, using the current date to uniquely identify the file.

### Future Scope:

The archives can be further transferred to a remote host or saved in a removable disk so that in case of system failure, information can be restored.
