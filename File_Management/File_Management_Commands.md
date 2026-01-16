>## Directory Commands

```bash
pwd                         # Print Working directory
```

>## The `ls` Command
```bash
ls                          # List Directory contents
ls [-option] [File/directory]
 
ls -l                       # Detailed Listing (permissions, owner, size, date)
ls -lh                      # Human Readable Size
ls -S                       # Sort by file size
ls -r                       # Reverse order sorting
ls -a                       # Include hidden files
ls -R                       # Shows all subdirectories
ls -t                       # Sort by modification time
ls -i                       # Show innode number
ls -1                       # One entry per line

```
>## `cd`

```bash
cd [Directory_path]         # Change Directory 
cd /home/ravi/projects      # Example
cd                          # Go to home directory
cd ~                        # Go to home directory 
cd ..                       # Go up one 
cd -                        # Move to the last directory where you are
cd ./Downloads              # Moves into downloads inside the current directory
```
>## Create `mkdir` and Remove `rmdir`.
```bash
mkdir Dname                 # Create a new directory
mkdir D1 D2 D3 D4           # Create Multiple Directory 
mkdir -p                    # Create nested directories like D1/D2/D3
mkdir -m 700 D5             # set permission at the time of directory creation  
mkdir -v                    # Shows confirmation message when directories are created
mkdir Month_{Jan,Fab,Mar}   # Creates Month_Jan,Month_Feb,MOnth_Mar in one command.
```
>## Remove Directory
```bash
rmdir name                  # Remove Directory
rmdir D1 D2 D3              # Remove all 
rmdir -p /D1/D2/D3          # Remove Nested directories
rmdir -v D1                 # Verbose Output, Confirm Before deletion
rmdir -p -v /home/ravi/D    # Remove directory tree Empty only
```
