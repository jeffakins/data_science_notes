Data Science Notes

CODEUP Quick Reference

Command Line

Directories
•	pwd – Print Working Directory i.e. “you are here”
•	ls – “list”; will list the contents of a directory
•	cd – change directory
•	cd ~/ – will take you to your home directory
•	. –  single dot, current directory
•	.. –  double dot, directory immediately above the current directory (ex: “cd ../../” would go up two directories)
•	touch – creates a new empty file of whatever name we specify
•	mkdir – make directory; creates a directory
•	mv – moves a file; needs two pieces of information, or arguments, to work. The first is the original file that you want to move, the second is the location where you want to move it.
•	rm – is used to remove a file(s)
•	find – used to search for files
•	cat – used to display the contents of a file
•	less – another way to display file contents on the command line
•	open – (MacOS) will try to guess which program to use to open a given file
•	head; tail – can be used to view the first or last few lines of a file
•	pbpaste; pbcopy – (exclusive to MacOS) can be used to show and set the contents of your clipboard
•	grep – used to search for text in a file
•	-h; --help: 

Flags
•	-a – all files
•	-l – long format
•	-h – human readable output

Keyboard Shortcuts
•	Tab – will show you auto complete suggestions
•	Up Arrow – will autofill the last command line input
•	ctrl-a – go to the beginning of the line
•	ctrl-e – go to the end of the line
•	ctrl-k – delete from the cursor to the end of the line
•	ctrl-l – clear the screen
•	ctrl-w – delete one word backwards
 
Git

Linking a folder to GitHub – First time setup
1.	Create a directory 
a.	mkdir “name of new directory”
b.	cd “name of new directory”
2.	Initialize a repository inside of it
a.	git init – initializes a new repository. Run from the top-level directory of your project. Should only be run once per project. 
3.	Create a repository on github and add the remote to your project
a.	git remote add origin “url from github”
4.	Create readme
a.	Type in terminal (in folder that you want to add README): clone README.md
i.	open file and add content
5.	git add <new file names> (or add .)
6.	git commit -m ‘notes’
7.	git push origin main
a.	git push -u origin main (allows you to type “git push” instead of “git push origin main”)
Or
8.	(Quick Method) 
a.	Create new repository on GitHub
b.	Get clone address
c.	In terminal (in folder that you want to add new repo): git clone <clone address> 
d.	Add README.md (see above)

Daily Workflow
1.	Create/modify files
2.	Git add filename
a.	(Or) git add .
3.	Git commit -m “notes/message”
4.	Git push origin main
5.	Git status (throughout) 

Restore files to your computer from GitHub
1.	Navigate to that repo’s address in GitHub
2.	Click on the green Code button
3.	Copy the clone address (will be https or ssh)
4.	Navigate to the folder we want to be the parent folder
5.	In terminal type: git clone <paste in that git clone address>
6.	This makes a new folder/repo on your machine w/ the same name as the github repo
7.	If you *know* you want to go back to the last repo commit locally, `git checkout -f`
8.	If you need to go back to the last commit of a single file, `git checkout filename.py`
 
SQL
Vocab
•	RDBMS: Relational Database Management System
•	Client/Server: Server provides service and client consumes that service
o	Client sends SQL Queries to the DBMS and DBMS sends back results
Ways we can interact with the SQL Server
•	Sequel Ace: running one or multiple SQL queries
o	Edit a .sql file
o	MySql command to run a shell connected to the SQL server

Keyboard Shortcuts:
•	Command + R to run a query
•	comments
•	/* */ comments multiple lines
•	Command / -- will place /* */ around a selection


Joins
1.	List out tables you will need to access
2.	SELECT * from your first table
3.	Determine the type of join that you might need and make first joins
4.	Determine if you need a WHERE clause to refine the information

