Q1: What did pwd print?
ans: It prints the path of the present working directory.
Q2:What did ls -a show plain ls did not?
ans: ls -a shows all the folders or files that reside in the current working directory including the hidden files whereas ls exclude those hidden files.
Q3:Pick one line from ls -l. What do you think the first column means?
ans:The first column is tecnically called meta data that actually represents the overall information about how the folders have been saved inside the current working directory.
Q4:Why does that work from where you are standing ? Which kind of path is coding-cafe/week02?
ans:It works because the terminal commands work on the current directory.  It is an absolute path.
Q5: mv did two different jobs above. What were they?
ans:i) it moved the file from one directory to another directory.
ii) it changed the name of the file in the existing directory.
Q6:How many folders are on your PATH?
ans:20
Q7:Write down exactly where your python3 lives.
ans:/usr/bin/python3
Q8:Compare your answer to 7 with the person next to you.Are they the same ?If not,why might that be?
ans:No it isn't . Maybe we have different operating system or device.
Q9:What exactly did the shell say?Explain the error in your own words,using the word PATH.
ans:pyton3 can't be found and it suggests us correct command.The python command is actually python3 here.so explicitly it can't found the path to pyton3.
Q10: .venv does not appear with plain ls.Why not?
ans: Because ls does not show hidden files .
Q11:What changed about your prompt?
ans:the start of the prompt./mnt/c/Users/Admin/Desktop/coding-cafe/.venv/bin/python3
Q12:Compare this with what you wrote down for question 7. is it the same path? if not,what does that tell you about what activate actually did to your PATH?
ans:exactly comes out to be different.probably it activated the .venv to the very prompt we used with which python3 command.
Q13:What is in the second list that was not in the first?
ans:other versions of pips that installed afterwars Package            Version
------------------ ---------
certifi            2026.7.22
charset-normalizer 3.5.1
idna               3.19
pip                24.0
requests           2.34.2
urllib3            2.7.0
Q14:Where does python3 point now?
ans:now python points to its system environment./usr/bin/python3
Q15:Find what ls -h does.Write it in your own words.
ans: it did the same as what ls does.
Q16:What is the difference between what Ctrl+C and ctrl+D did?
ans:ctrl+c jumped to another line of prompt in wsl whereas in python3 it shows keyboard interrupt that means ctrl+c is not recognised by python interpreter in case of ctrl+d in python it exits out from python3 to wsl again.