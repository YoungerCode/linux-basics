

1. type in ls and press enter. What do you see? What does this mean?

recruit@recruit-Mecer-X102:~$   ls 
Desktop  Documents  Downloads



ls displays the list of directories/folders that are available, in this case folders are Desktop  Documents  Downloads


2. type in pwd and press enter. What do you see? What does this mean?


recruit@recruit-Mecer-X102:~$ pwd
/home/recruit

pwd is a command that displays the current working directory, following is our current directory 
/home/recruit



3. Make a new directory called workspace then cd into your new directory

recruit@recruit-Mecer-X102:~$ mkdir workspace
recruit@recruit-Mecer-X102:~$ cd workspace
recruit@recruit-Mecer-X102:~/workspace$ 

4. type in ls and press enter. What do you see? What does this mean?

recruit@recruit-Mecer-X102:~/workspace$ ls
recruit@recruit-Mecer-X102:~/workspace$ 


Displays the workspace folder, this means that there is nothing inside the folder

5.Make a new file called README.md (you can use the touch command to do this)

recruit@recruit-Mecer-X102:~/workspace$ touch README.md
recruit@recruit-Mecer-X102:~/workspace$ ls
README.md

6.Make a copy of README.md, name your copy CHANGELOG.md
recruit@recruit-Mecer-X102:~/workspace$ cp README.md CHANGELOG.md



Task 2 : Absolute and Relative Paths

1. Create an empty file named exercise.md and move this file to the /tmp directory, using a relative pathname. Then, delete this file using an absolute pathname.

recruit@recruit-Mecer-X102:~/workspace$ sudo mv exercise.md /temp

rm   / tmp/ exercise.md







Task 3 : cat commands


1.Create 3 files namely umuzi.md, recruits.md and cohort.md.

2.Fill all 3 files with contents of your choice. Maybe some nice poems about you MUB experience.

cat > umuzi.md

cat > recruits.md
cat > cohort.md 

3. Write a script that concatenates the content of umuzi.md, recruit.md, cohort.md and displays the result on the screen.
 recruit@recruit-Mecer-X102:~$ cat umuzi.md recruits.md cohort.md


4.Write a script that takes the content of umuzi.md, cohort.md and recruits.md to print/store the output into a new file named summary.md.
recruit@recruit-Mecer-X102:~/workspace$  cat umuzi.md recruits.md cohort.md > summary.md
5. use the command line to append the words “The End” to summary.md. Be careful not to overwrite the exiting contend
recruit@recruit-Mecer-X102:~/workspace$ echo "The end" >> summary.md


Task 4 : The locate command

Write a script to help you locate a file named umuzi
1.recruit@recruit-Mecer-X102:~$ locate umuzi
2.locate umuzi > search_result.md


Task 5 The locate command cont..

1.Create a file within Documents directory, add to is a file named pad.md
recruit@recruit-Mecer-X102:~/Documents$ touch pad.md
2.  change the working directory to Desktop, then create a folder and name it work
recruit@recruit-Mecer-X102:~$ cd Desktop
recruit@recruit-Mecer-X102:~$ mkdir work
3.copy pad.md to the currently working directory as pad_copy.md
recruit@recruit-Mecer-X102:~/Desktop$ cp ~/Documents/pad.md .
recruit@recruit-Mecer-X102:~/Desktop$ mv pad.md pad_copy.md
4.update the database used by locate by running locate updatedb.
recruit@recruit-Mecer-X102:~/Desktop$ locate updatedb
5.  change the working directory to the previous one (cd -)
recruit@recruit-Mecer-X102:~/Desktop$ cd -
6. use locate to find pad_copy.md

recruit@recruit-Mecer-X102:~$ locate pad_copy.md


Task 6 Find commands

1.Write a script to find all files ending with ‘pdf’ on your computer

recruit@recruit-Mecer-X102:~$ locate pdf
2.Write a second command that takes the result of the previous search and copy into a folder of your choice.
recruit@recruit-Mecer-X102:~$ locate pdf > PDF_results

3.Write a command to display files that where modified today.
recruit@recruit-Mecer-X102:~$ find . -mtime -1


















Task 7 Text editor

Your initial commit

1.Using nano text editor create a file named my_bio.md
recruit@recruit-Mecer-X102:~/my_files$ nano my_bio.md

2.Create a folder named my_files and move my_bio.md within.

recruit@recruit-Mecer-X102:~$ mv my_bio.md ./my_files

