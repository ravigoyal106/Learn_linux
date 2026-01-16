>## Create a File

```bash
touch file_Name             # Create a empty file
```
>## Editing Files
```bash
nano file                   # Simple terminal text editor
vim file                    # Advance Editor with modes
gedit file                  # GUI editor
```
>## Remove File

```bash
rm file_Name                # Remove File
rm -i file_Name             # Ask before deleting
rm -f file_Name             # Force delete without prompt
rm -r dir/file_Name         # recursive delete
```
>## Viewing File contents

```bash
cat file_Name               # Display file content
less file_Name              # Scroll one page at a time
head -n 2 file_Name         # Show two lines of file
tail -n 2 file_name         # Shows last two
```
>## Copying, Rename and Moving Files

```bash
cp [source] [destination]       # Copy files
cp file.txt /home/ravi/         # Copy into directory
cp -r dir1 dir2                 # copy directories recursively

mv [source] ][destination]      # move or rename

```
>## File Permissions
```bash
# Link 
```
>## File Metadate

```bash
stat file                       # Detaild info (size,timestamps,innode)
file file_name                  # Identify file type
wc                              # lines, words, bytes 
wc -l                           # only lines
wc -w                           # Count words
wc- c                           # Count bytes
wc -m                           # Count characters
wc -L                           # Print length of longest line
```
