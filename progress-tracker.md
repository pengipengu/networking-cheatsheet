====================
PROGRESS TRACKER - GIT 
Date: April 24, 2025
====================

1. Github Repo Setup
--------------------
- Created Github repo: networking-cheatsheet
- Initialized local Git Repo:
	git init

- Created and commited readme.md:
	touch readme.md
	git add readme.md
	git commit -m "Initial Commit: Networking Cheat Sheet"
		(-m is for message)

- Renamed default branch to 'main' (GOOD PRACTICE):
	git branch -M main

- Linked to Github Repo:
	git remote add origin [link in the github repo] may .git sa dulo

- Pushed to Github:
	git push -u origin main 
		( -u sets upstream to remember this connection)

[X] ERROR FIXES: Nagka problema sa credentials, tried changing it via:
	
	git credential-manager erase
	git config --global user.name "pengipengu"
	git config --global user.email "password"
		(initially worked, but ang gumana ay...)
	
	1. Open Windows Control Panel > Credential Manager > Windows Cred.
	2. Removed the original "carlosmatthew" github (gbox)
	3. Git bash login, then may nag pop-up  na github login with browser!

- Branch (Made progress-tracker)
--------------------------------
- Created a new branch:
	git checkout -b progress-tracker
		( -b creates and switches to the branch, checkout means "switch to")

- Created and edited file:
	touch progress-tracker.md
	nano progress-tracker.md
		(Ctrl + 0 to save, CTRL + X to exit)
 
- Commited and pushed:
	git add progress-tracker.md
	git commit -m "Add progress tracker"
	git push -u origin progress-tracker

- Since may branch, in order to have a "remote" version of it, you can do:
	git push --set-upstream origin progress-tracker 
tas if may future changes you can now just do:
	git push


[Common Git Commands]:
git init 				->	initialize repo

git branch -M main             		->      rename branch(master) to main (good practice) [TRY DOING THIS HERE TOO]

touch 					-> 	create new file

nano 					-> 	edit file (via terminal)

git add 				-> 	"Stage" file

git commit -m "msg"			->	Commit with "message" (for taking notes)

git branch -M main 			->	rename branch(master) to main (good practice)

git remote add origin <repourl>		->	Connect local repo to Github Web

git push -u origin main 		->	Push na!

git checkout -b name 			-> 	create and checkout(switch) sa new branch

git push --set-upstream origin		-> 	basis where it will be pushed. 
							basically, clarifiy where it WILL be pushed. technically diba, yung -u yung "-upstream" pero if --set-upstream, manually mo ilink sa branch 

==================================

** DAILY GIT DRILL **

[REMEMBER] 
Init.Touch.Write.Add.Commit...Link.Push.DONE
I T W A C L P D

or

Init.Touch.Write.Add.Commit...Branch.Link.Push.DONE

I T W A C B L P D

(Branch if needed)


[MEANING]
Init 	->	git init
Touch 	->	touch README.md (or file)
Write 	->	nano README.md
Add	-> 	git add README.md 
Commit 	->	git commit -m "Update"
Branch 	->	git branch -M main
Link	-> 	git remote add origin <repo-url>
Push	->	git push -u origin main
DONE	-> 	LEZGO!

=================================
APRIL 26, 2025
=================================

- Will try to push this change to the repository
- Recalling git commands

=================================
APRIL 27, 2025
=================================
LOTS OF GIT COMMANDS I DISCOVERED TODAY!!

Not that sure (di ko nakita how it worked) pero may isa, which is git reset --hard HEAD~1 which i got this: "HEAD is now at 7798db5 April 26, 2025: Trying to recall git commands" - Local Changes Only!

These are for local changes only, if gusto mo mag undo talaga tapos MAWALA lahat ng changes na nacommit sa github web version (RISKY!) - do git push --force. (Mas safe parin pag di tinotouch ang remote, kaya dapat mag branch)


The git commands:

git reset --soft HEAD~1 		-> 	good for fixing messages
git reset --mixed HEAD~1 		-> 	good for re-seleting files
git reset --hard HEAD~1			-> 	DANGER ZONE (discard everything)


i think kaya HEAD~1 kasi aatras ung head (pointer) ng isa 



