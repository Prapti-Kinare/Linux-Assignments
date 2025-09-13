### Rename a file:
mv oldname.txt newname.txt

### Create a new empty file:
touch newfile.txt

### Remove a file:
rm file.txt

### Show short and long listing formats:
ls
ls -l

### Show attributes (permissions, size, owner, type, etc.) → from ls -l.

### Show all files including hidden:
ls -a

### Show only hidden files:
ls -d .*

### Create and navigate directory:
mkdir cdac-dir
cd cdac-dir

### Remove directory:
rm -r cdac-dir

### Redirect man page to file:
man ls > temp.txt

### Display first 10 and last 5 lines:head -n 10 temp.txt
tail -n 5 temp.txt

### Copy and rename:
cp temp.txt /path/
mv /path/temp.txt /path/newname.txt

### Count lines, words, chars:
wc temp.txt

### Show last 10 commands:
history | tail -n 10

### Create tar archive:
tar -cvf archive.tar directory/

### Create zip archive and list:
zip -r archive.zip directory/
unzip -l archive.zip

### Change permissions:
chmod 700 file.sh

### Change ownership:
chown user file.sh

### List processes:
ps
ps -aux
top

### Date & calendar:
date
cal
### Change system date:
sudo date -s "14 MAR 2024 10:10:00"

### Links & Remote
Hard link:
ln file1.txt hardlink.txt

Soft link:
ln -s file2.txt softlink.txt

### SSH into remote:
ssh user@host -p 22

### SCP file to remote:
scp file.txt user@host:/path/

### SCP dir from remote:
scp -r user@host:/path/ localdir/

### FTP example:
ftp ftp.netbsd.org

### Grep search:
grep "word" *.txt

### Create dir with specific permissions:
mkdir -m 755 mydir

### Compare 2 files:
diff file1 file2

### Rsync directories:
rsync -av dir1/ dir2/

### Cut specific chars:
cut -c 5-10 file.txt

### Extract one file from tar:
tar -xvf archive.tar.gz file.txt

### Count word occurrences:
grep -o "word" file.txt | wc -l

### Copy file:
cp ~/report.pdf ~/documents/

### Move file:
mv ~/downloads/data.csv ~/projects/

### Create multiple files:
touch log1.txt log2.txt log3.txt

### Rename dir:
mv old_project new_project

### Delete file without prompt:
rm -f temp.log

### Human-readable listing:
ls -lh

### File type from ls -l first char:
d → directory
- → regular file
l → symbolic link

### List dotfiles:
ls -a

### Only dotfiles:
ls -d .*

### Create nested dirs:
mkdir -p workspace/projects/web/frontend

### Company structure:
mkdir -p company/departments/{hr,finance,tech} company/employees/{active,former}

### Remove dir:
rm -r test_dir

### Save man page:
man find > find_manual.txt

### Show first 15, last 8 lines:
head -n 15 find_manual.txt
tail -n 8 find_manual.txt

### Copy & rename:
cp find_manual.txt manuals/find_help.txt

### Count lines, words, chars:
wc find_manual.txt

### Last 15 commands:
history | tail -n 15

### Tar.gz of Documents:
tar -czvf docs.tar.gz ~/Documents

### Zip archive of Desktop:
zip -r desktop.zip ~/Desktop
unzip -l desktop.zip

### File permissions (owner only):
chmod 700 script.sh

### Change owner:
sudo chown admin database.txt

### System In Commands
uptime → show uptime/load
df → free disk space
du → disk usage per folder
free → RAM usage

### Umask test:
touch permissions_test.txt
umask 022
touch new_permissions_test.txt
ls -l

### Copy via SCP:
scp -r user@server:/projects ~/Downloads/

### FTP download:
ftp ftp.gnu.org

### Remove old_data dir:
rm -rf old_data

### List logs:
ls -la /var/log

### Create config file:
mkdir -p /opt/myapp/config
touch /opt/myapp/config/config.txt

### Search logs for errors:
grep -r "error" *.log

### Monitor log in real-time:
tail -f application.log

### Find large files:
find / -type f -size +100M

### Create file with content:
echo "Hello World" > file.txt

### Compress dir with gzip:
tar -czf dir.tar.gz dir/

### Files owned by john:
find /home -user john

### Disk usage sorted:
du -sh * | sort -h

### Kill process by name:
pkill process_name

### Create symlink to directory:
ln -s /path/to/dir linkname

### Find executables in PATH:
which -a command

### Merge two sorted files:
sort file1 file2 -o merged.txt

### Unique lines only:
sort file.txt | uniq

### System monitoring:
top
htop

### Empty files:
find . -type f -empty

### Change timestamps:
touch -t 202501010101 file.txt

### File readable only by owner:
chmod 400 file.txt

### Find broken symlinks:
find . -xtype l

### Copy preserving timestamps:
cp -p file.txt newfile.txt
