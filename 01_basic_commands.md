Basic Linux Commands

*Moving around and checking files*
  Command                             What it does
  pwd                               Shows the directory I'm currently in.

  cd DIRECTORY                      Takes me to another directory.

  cd ..                             Moves up one directory.

  cd ~                              Takes me to my home directory.

  ls                                Lists files and directories.

  ls -l                             Shows a detailed list, including permissions and ownership.

  ls -a                             Shows hidden files as well.
ls -lh                            Shows file sizes in a more readable format.


*Creating and managing files and directories*
These are the commands used when setting up folders and moving files
around.
  Command                             What it does
  mkdir practice                    Creates a directory called practice.

  mkdir -p practice/logs            Creates the directory and any missing parent directories.

  touch notes.txt                   Creates an empty file if it doesn't already exist.

  cp notes.txt backup.txt           Copies a file.

  cp -r folder backup-folder        Copies a directory and itscontents.

  mv old.txt new.txt                Renames a file.

  mv file.txt /tmp/                 Moves a file to another directory.

  rm notes.txt                      Deletes a file.
rmdir empty-folder                Removes an empty directory.

*Reading a file*
  Command                             What it does
  cat FILE                          Prints the whole file in the terminal.

  less FILE                         Opens a file in a viewer where I can scroll. Press q to exit.

  head FILE                         Shows the first 10 lines.

  head -n 5 FILE                    Shows the first 5 lines.

  tail FILE                         Shows the last 10 lines.

  tail -n 20 FILE                   Shows the last 20 lines.
tail -f FILE                      Keeps showing new lines as they are added, which is useful for watching logs.

*Finding files and searching text*
use these when I need to find a file or look for a word in a file.

Command                             What it does
  grep "error" app.log              Shows lines containing error.

  grep -i "warning" app.log         Searches without distinguishing uppercase and lowercase.

  grep -n "failed" app.log          Shows matching lines with their line numbers.

  find . -name "*.txt"              Finds .txt files under the current directory.

  wc -l notes.txt                   Counts the lines in a file.
wc notes.txt                      Shows line, word and byte counts.

*A few other useful commands*

  Command                             What it does
  clear                             Clears the terminal screen.

  history                           Shows commands entered in the shell.

  whoami                            Shows which user I'm logged in as.

  date                              Shows the system date and time.

  file notes.txt                    Gives information about the file type.

  which bash                        Shows the path of the bash executable found in my PATH.

  man ls                            Opens the manual for ls. Press
q to exit.
echo "Hello"                      Prints text in the terminal.

*Combining commands*
A few symbols make it possible to connect commands or save their output.
  
Symbol                              What it does
  \|                                Passes the output of one command to another command.

  >                                 Writes output to a file, replacing what was already there.

  >>                                Adds output to the end of a file.

  &&                                Runs the next command only if the previous one succeeds.
;                                 Runs the next command whether or not the previous one succeeds.
lio
