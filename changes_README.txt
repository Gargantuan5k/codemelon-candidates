x---------- CODEMELON RELEASE CANDIDATE 1 (v0.6.0) ----------x
x------------------------ CHANGELOG -------------------------x

1. Added Single-line and Multiline comments.
   • Single line comments are defined using the $ character. Example: $ This line will be ignored.
   • Multi-line comments are defined using the #   # character. For example: # These
									       Lines will be
									       Ignored. #

2. Added the run('filename.mln') function and support for external files.
   • Only files with .mln extension can be run.
   • Example: run('test.mln')

   ♦ --EXTERNAL FILES-- ♦
   
   Tabs and spaces are ignored wherever possible. Each line of code must be followed by newline '\n' or newline character ';'.
   For example: 
	• print('hello); print('world')
	• print('hello')
	  print('world')
	$ Are both acceptable, while
	• print('hello') print('world')
	• print('hello')\nprint('world') 
	$ Are not acceptable.

3. Fixed multiple bugs. Notable ones are listed.

• A011 : Single quotes " ' " do not work with strings (FIXED)
• C001 : extend(list1, list2) function for List type reeturns AttributeError Exception (FIXED)
• B003 : Multiline comments not working (FIXED)
• B004 : Multiline comments cause crashes (FIXED)
• D004 : Placing a function after another function generates a Runtime Error 'token cannot be placed after another token' (FIXED)
• B006 : Single-line and Multi-line comment characters are switched (Should be $ for single, # for multi) (FIXED)
• A001 : Conditional statements cannot compare String datatypes (RESURFACED) (FIXED) --previously fixed in v0.4.0
• PEP8 : Multiple PEP8 violations in source code (FIXED)
• E007 : print_ret Builtin function not working (FIXED)

♦ Testing and fixing for other bugs still underway! 

* This release candidate may or may not be stable, report bugs by starting new issue threads on https://github.com/Gargantuan5k/codemelon-candidates/issues
* Issue title must contain version name followed by a very brief description of the issue. A more detailed description may be provided as a comment on the issue thread.
  For example, Comments not working in Release Candidate 1 may be reported as 
  [rc1] Comments not working
  OR
  [v0.6.0] Comments not working.
* New commits not made by the repository owner must be made on forks or separate branches. Your changes will be reviewed and committed to the main branch if found stable.

>> CodeMelon v0.6.0-rc1 --Release Candidate 1

