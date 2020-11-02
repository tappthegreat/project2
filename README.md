# project2

#4 For step 4, the simple script of day, calendar, ls and pwd, I had to use nano task.sh instead of the tutorials vi. Also,cal does not work in Gitbash, but task.sh is now a script.

#9 Created the Hello World Script using the default method in the tutorial. I tried the alternative approach, but found that it erased my previous script. It was good practice to recreate the script again though. Created the file by "nano hello-world.sh" Used a shebang to define the interpreter as bash on the first line, line 3 "echo "hello world", then saved. Made the file executable by chmod +x hello-world.sh.

#10 "man" command does not work in GitBash. I had to change the directory to where my backup script was located using cd~ and then making a new folder. The default folder for my projects was my "users" folder, which is around 30GB! 

#11 Created the welcome script. Very fun, although very simple. Simply used the previous steps to create a script, by using "nano welcome.sh" Then inputting the proper instructions from the tutorial. At first, I thought (Whoami) was just entering my own name but found out that its actually a command that gathers the name of your Computer! Changed the error to reflect the correct name.

#13 Implemented two functions, total files and total directories. It is similar to coding as it has brackets and curly braces. The functions located the number of files within a directory and reports the number of directories. wc and find.


***NOTE : In my backup script, I found I had to make folders with my username or else the script would not backup my home directory. The username folder remained empty and unused, but was required to save.

#14
Created a comparison script that used variables like -lt -gt etc. to compare to numerical values attached to variables a and b. It used a simple less than, equal than etc to show if a statement was true (0) or false (1). Similar to java, you attached numbers to variables, used echo as a "printout" statement to echo the results.

#15 
Conditionals were a little difficult for me. The biggest hurdle was typing mistakes! 
I had to read over the tutorial a few times to understand of how everything worked together, but it seems straightforward now. The script is checking to see if every file was backed up and if there is one error, it will not backup that specific area. I had numerous typing errors which resulted in multiple errors, but it shows that even the smallest of mistakes can lead to a scripting error.

#16 
Positional parameters were pretty straightforward. Introducing -z and -d, I was able to use an if/else conditional to check to see
if the users home directory existed and it did BUT, there you have be careful not to have "then" on teh same line as the if statement. Also, making there is a space before and after the bracket is imperative as it will give you a syntax error if you don't.

#17
For loop
For some reason, I could not get the for loop to work within my bash. There are no compilation errors, it just doesn't execute. When I added the new commands as notes with "#" it worked. I'll have to look more into why this isn't working, because the tutorial is either not telling me correctly, or it's an error on my part.



		"Code Review (Rudy Carreon)"

So, I forked your Project 2 back when it was due. I was looking at the forked items this week and saw that some of the code was missing. I am not sure if you ever went back to add that in, but #17 in your README.md file does say that you could not get the For loop to work. I did want to show you the code I have for the the while.sh and until.sh sections. I don't believe I was able to get the for loop to work in my program too. Here is the code I have for the while.sh if you decide to use it:

while.sh

#!/bin/bash

counter = 2
while [ $counter -lt 3]; do
	let counter += 1
	echo $counter
done

Here is the code for the until.sh

#!/bin/bash

counter = 4
until [$counter -lt 3]; do
	let counter -= 1
	echo $counter
done

I hope this helps with your project. Let me know what you think. The other recommendation that I have is possibly having all the code in your master to be in the main with your README.md file. Maybe I misunderstood Project2, but I think you create a copy of all the code, create the README.md file separately, and then push it through with the original. After that, you'd be able to delete the copy and just be left with the main that holds everything.

