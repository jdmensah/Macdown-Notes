#Text Editors 
What do we need from text editors ?  
* Syntax Highlighting   
* Code Completion  
* Keyboard Shortcuts  
* File Management/ Folder Management  

##Types of text editors
Sublime Text  
Brackets  
Atom  
Notepad++  
Visual Studio

##VIM
A text editor on the command line, 

##IDE - Intergrated Development Environment
Eclipses  
NetBeans  
Swing   
RubyMine  
Visual Studio 	

##Diff Tools
Used to compare the differences in file and text documents

#Version Control 

##Why Do We Need VCS - Version Control Systems 
* We can use it to backup and restore files  
* Synchronization between different developers  
* short-term undo - allows you to jump back to a clean state of the file/version that the stable (worked)  
* Tracking of who changed what, and when  
* Sandboxing - make temporary changes in isolated areas  
* Branching and merging (a much larger sandbox) - taking individual files where the developer can work on in isolation, then when stable merge to the main branch   
* provides history of content changes 
	* graphics 
	* design 
	* programming code
	* changes in text 
	* adding of logo
	* website changes

It is a collaborative tool - allowing people to do the same thing on the same file, whilst keeping track of who, when, why and what the person changed to the file. Merging allows the joining of changes made to files into one unified file.  

##Terminology  
**REPO(Repository)** - The database storing the files  
**LOCAL COPY** - your directory of files. the version of the project on your machine.    
**REMOTE COPY** - the version of the project on a remote server - the copy of the file the lives online.  
**MASTER/TRUNK** - The primary branch   
**COMMIT** - save a snapshot of the files in your staging area.   
**PULL** - get a version of the file you wish to use from the repo
**INIT** - initialise new local repository 
**STATUS** - view the status of the files, including staged and unstaged files  
**LOG** - view a log of all the commits made  
**-m** - add a message to the commit  
**--amend** - amend a commit 


Local VCS - Local Version Control System  
![Local VCS](http://pigne.org/teaching/images/vcs-diag.png)

CVS - Centralized Version Control System  
![CVS](http://pigne.org/teaching/images/cvcs-diag.png)

SVN - Subversion  
![SVN]()   
* A tool to help with version control systems  
* Make sure when you make a snapshot copy, your commit does not break the file so make sure you have no error in your build. 

Distributed VCS - Distributed Version Control System
![Distributed VCS](http://ahsio.com/code-versioning/images/distributed.png)

##Git 
[Git Training & Guides](https://www.youtube.com/channel/UCP7RrmoueENv9TZts3HXXtw)  

Locally enabled, control item on your desktop, no complicated software needed  

###Example Git Code 

git init myproject -  
cd myproject - change directory to the myproject directory(folder)  
git add - notices the files and put them in a staging areas  
git commit - stores snapshot version of file  

Distributed Git  
designed for team collaboration  

git checkout master  
got commit -a -m "my new logo"  
git push  

git checkout -b   
git commit -a(add all)  -m(add message of changes made) "" 
git push origin danasfeature  

git pull  
git merge danasfeature  

--
