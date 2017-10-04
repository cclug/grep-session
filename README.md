Local Text Search Session
=========================

Aim
---

Improve skills in doing text based search queries on the local disk.

    grep, egrep, fgrep, git grep, find

Agenda
------

1. Brainstorming session

    What 'search' skills would I like to improve?

2. Challenges

Challenges
==========

Format:

    N. (search-file | directory)

    	q: challenge description

    	r: description of expected result


Set-up:

    git clone https://github.com/cclug/grep-session
    git clone https://github.com/spf13/cobra

Basics
------

1. patch.mbox

    q: Who sent the patch?
    r: Single line containing name and email address.
    
2. patch.mox

    q: List all lines that include an email address.
    r: 48 lines, a bunch of false positives.

2. cobra/

    q: All files that mention the function `OnInitialize`
    r: ```
    	README.md
	    cobra.go
	    cobra/cmd/init.go
	    cobra/cmd/root.go
	    ```

Middle
------

1. patch.mbox

    q: Return the email sender (not the mailing list) and the subject.
    r: Two lines.

2. patch.mbox

    q: All the lines added to the code by the patch i.e starting with a plus symbol.
    r: 2632 lines.

3. cobra

    q: List all lines containing function definitions that include `string` in the parameter list.
    r: 199 lines.

Advanced
--------

1. patch.mbox

    q: What is the email address of the patch author.
    r: Just the email address.

2. patch.mbox

    q: Extract all the email address from the patch.
    r: ?

3. cobra/cobra/

    q: Extract a list of all function names from the source code.
    r: ?
