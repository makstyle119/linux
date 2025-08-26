# Linux

this is my journey to learn and understand Linux

## Question & Answer

**Q1- What Is an Operating System ?** <br />
**A1- Operating System** is something which allow us to run and manage our machine.

**Q2- What Is NULL device ?** <br />
**A2- NULL Device** OR dev/null is a folder which will erase everything inside it like a black hole.

**Q3- What Is Permission ?** <br />
**A3- Permission** is what you can do with the file.
- *`d` = directory*
- *`r` = read*
- *`w` = write*
- *`x` = execute*
- *`-` = no permission*
- why written three times - first is for owner, second is for group and third is for other


## Commands
- *`pwd` = to get your path*
- *`clear` = to clear the screen*
- *`man bash` = give the manual of bash*
- *`ls` = to display folder content*
    - *`ls -a` = to display hidden folder*
    - *`ls -l` = to display all information*
- *`cd` = change directory*
    - *`cd ..` = to go to parent directory*
    - *`cd /` = to go to root directory*
    - *`cd ./path` = to go to specific directory*
- *`sleep` = to sleep the terminal - it will take time in second*
    - *`sleep 10` = wait for 10 second*
- *`mkdir` = to create directory*
- *`touch` = to create file*
    - *`touch file_name` = to update timestamp of a file only if exist*
    - *`less file_name` = to read file*
- *`> file_name` = to create file*
    - *`echo "hello world" > file_name` = to write text in a file - overwrite*
    - *`> existing_file_name` = to overwrite file`*
- *`>> file_name` = to create file and append text in a file*
    - *`echo "hello world" >> file_name` = to append text in a file - not overwrite like >*
- *`rm` = to remove file*
    - *`rm -r` = to remove directory*
- *`rmdir folder_name` = to remove empty directory only*
- *`file` = to check file type*
- *`mv` = to move file*
    - *`mv file_name_before file_name_after` = to move and rename from file1 to file2*
    - *`mv folder_name_before folder_name_after` = to move and rename from folder1 to folder2*
    - *`mv file_name_one file_name_two folder_name` = to move file1 and file2 to folder*
    - *`mv -i file_name_before file_name_after` = to move and rename from file1 to file2 with confirmation*
    - *`mv -u file_name_one file_name_two folder_name` = to move file1 and file2 to folder only if the file is updated`*
    - *`mv -uv file_name_one file_name_two folder_name` = to move file1 and file2 to folder with the verbose mode`*
- *`cp` = to copy file*
    - *`cp file_name_one file_name_two folder_name` = to copy file1 and file2 to folder*
    - *`cp -r folder` = copy all the child folders too*
- *`cat` = to display file content*
- *`ls non-existing file 2> error` = to append error in error file*
    - *`ls 2> error > output` = to display error in error file and output in output file*
    - *`ls 2>> error >> output` = to append error in error file and error in output file too`*
    - *`ls non-existing file > output 2>&1` = to display error and output in output file - old way*
    - *`ls &> output` = to display error and output in output file - new way*
- *`ls -la /etc |` = to pipe(display) the output*
- *`wc -l file_name` = to count the number of lines`*
- *`tail file_name` = to display last 10 lines`*
    - ``tail -n 5 file_name` = to display last 5 lines`*
    - ``tail -n +2 file_name` = to display from line 2`*
- *`ls /etc | tee output.txt` = to display the output and save it in a file*
    - *`ls /etc 2>&1 | tee output.txt` = to display the error and save it in a file*
    - *`ls /etc |& tee output.txt` = to display the error and save it in a file - only for new version of bash*
    - *`ls /etc | tee -a output.txt` = to display the output and append it in a file*
- *`whoami` = to display your username*
- *`id` = to display your user id*
- *`getent passwd` = to display all user**
    - *`getent passwd 1000` = to display user with id 1000**
- *`sudo adduser student` = to create user*
- *`su student` = to login as user`*
- *`su - student` = to login as user and get home directory`*
- *`groups` = to display what groups you belong to*
- *`groups user_name` = to display what groups user belongs to*
- *`sudo usermod -aG sudo user_name` = to add user to sudo group*
- *`sudo groupadd group_name` = to create group*
- *`chmod 777 file_name` = to give permission to all`*
    - *`-` = is equal to 0`*
    - *`x` = is equal to 1`*
    - *`w` = is equal to 2`*
    - *`r` = is equal to 4`*