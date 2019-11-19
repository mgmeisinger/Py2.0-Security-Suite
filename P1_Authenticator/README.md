Security-Suite >> P1_Authenticator
# Author: Michael Meisinger
# Language: Python 2.7.10
# Date Created: December 2018
# Date Last Updated: November 2019


Part 1 of the Security-Suite has 3 files:
	- creator.py
	- authentication.py
	- password.txt

* You will need Python on the local machine to run. *
* Make sure you are in the correct directory AKA P1_Authenticator *
** Leave a blank line at the end of "password.txt" **


How to run:
	Type "python creator.py" or "python authentication.py" to start either program.
	Example: ~$ python creator.py
			 ~$ python authentication.py

How to use:

	creator.py
		- Terminal-based menu that either adds an account or quits.
		- When adding account, checks to make sure username is unique.
		- If username is unique, then md5 hash the password and store them in "password.txt"
		- * If there is no "password.txt" file, creator.py will create it. *

	authentication.py
		- Terminal-based menu that either verifies a login or quits.
		- When verifying the login, prompts user for username and password.
		- First searches "password.txt" for a matching username, if none then authentication fails.
		- * If there is no "password.txt" file, authentication attempt will fail. *
		- If matching username, compares the password hashes, if match then login is successful.
		
		
Structure of "password.txt":
	- First line is username
	- Next line is the corresponding password hash
	- And so on.
	- ** Leave a blank line at the end of file. **
