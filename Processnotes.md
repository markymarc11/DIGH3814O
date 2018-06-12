# Module 1
## Exercise 1
- Relatively simple using markdown and dilinger, by following the steps provided and copying code from the markdown cheatsheet
- https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet
## Exercise 2
- when typing in passwords in the command line, it does not show your password, so you just need to type it and press enter
- https://askubuntu.com/questions/86660/i-cannot-enter-my-password-in-the-terminal-cant-install-packages
- same idea as module 1, just needed to follow the step by step commands and everything works out nicely
- cheat sheet for command https://help.ubuntu.com/community/AdvancedCommandlineHowto#Keyboard_shortcuts
## Exercise 3
- follow the commands laid out, simple stuff
## exercise 4
- everything was working well following the steps, but then my internet crapped out and I no longer have the readme.md fule ro any of the other information i did for exercise 4
- time to go back and do it all again
- not sure what is happeneing again, tried to do the <git status> command then everything dissappeared
- my internet is not working again apparently
- found better internet, life is good hopefully
- ended up deleting all of the files from the exercise from today to start from new
- in 4.2 i do not believe that i made sure to add the readme.md file to the git repository after the statu check
-  made sure to add it this time following the on screen commands <git add readme.md>
- get to the part where I am trying to do the commit
  it says "Changes not staged for commit: modified:    readme.md     no changes added to commit"
- tried moving forward to 4.3 everything still seems to be working
- checked the status of the new branch "branchone" showed that there was nothing else there, added the readme.md file to it
- making the changes now to the readme.md file
- used the git commit line right after saving the readme.md and it seems to have made a commit finally....
- tried doing the same thing again, after making changes to the file, but now it is saying "Changes not staged for commit" again...
- tried to go back to master file, came with error "Your local changes to the following files would ne overwritten by checkout" 
- so i tried to commit the new changes and it said "changes not staged for commit" again
-tried re-saving and commiting again still saying that I cannot commit the changes
- unable to get into the master branch.....
- looked through my old commands and found one to commit by using command <git commit -a>
- this command seems to have worked
- finally back on the master branch
- was able to merge the files with no problem at all, i'm happy
- saved all of the commands that i used to make everything happen up until this point
  
  # Module 2
  
  ## Exercise 1
  - Tried looking up my surname in the database, but came up with 0 Results, so Then I tried using my moms maiden name, which gave me a plethora of results which I can use. 
  - downloaded the results and saved them in the repository
  - documented what I searched for on the DHBox
  
  ## Exercise 2
  - following along on Ian Milligans tutorial for how to get information from a website https://programminghistorian.org/en/lessons/automated-downloading-with-wget#step-two-learning-about-the-structure-of-wget--downloading-a-specific-set-of-files
  -  (-r) means a recursive retrieval, so it goes to the site and follows the links off the site, and downloads them as well
  -  (-np) means it should links, but not beyond the parent directory
  - default takes you to 5 new links from the parent, but can change by (-l 3) which would only make it go to 3
  - (-w 10) adds a 10 second wait between server requests, so you are not clogging up a server
  - you can also limit the bandwidth used (--limit-rate=20k) this allows only 20kb/s
  - you can also mirror a full website with (-m)
  - ran all of the commands together to grab all of the information from the /papers/ section, everything seems to be running well, it is just taking a while
  - everything downloaded correctly, downloaded the history of commands that I have done so far
  - Now getting the information from the war diaries
  - use Dr.Grahams command to set up python directory, then run the script through it
  - all the files seem to be downloaded
  - running command to get all the urls, it is taking some time again, so I wait
  - everything was downloaded correctly, saved commands in war-diary directory
  
  ## Exercise 3
  - Found the information and transcribed it using notepad++
  - tried to view it in explorer and it was just coming up as black text
  - went through the text again to check to make sure everything was closed off, and it all looked fine
  - still only would show up as black text and did not show all of the writing that was transcribed
  - tried to go line by line to figure out what was wrong but still unable to get a colour coded version
  - back to trying it again\
  - tried writing the code line by line, saving and checking to make sure that they work, worked for the first two parts, but when i tried to annotate the person name, it no longer is showing up colour coordinated....
  - tried writing out the code again, did not change anything, but now it works, so I guess that is a good thing
  
  # Module 3
  
  ## Exercise 1
  - If using a text editor to make find patterns, you must always make sure they know it is a regex, usually need to tick a box or something
  - the | means "or" 
  - when looking to replace a word with another, make sure to put spaces before and after the word so that it doesn't change larger words with that letter combination.
  -  \< means the word starts like this \> means the word ends like this
  - () means to search for what is inside the brackets
  - a period .  inbetween letters represents a space that could be any letter
  ### Editing the Text
  http://workbook.craftingdigitalhistory.ca/supporting%20materials/regexex/
  - Have gotten rid of all of the extra text using Notepad++
  - deleted the extra little bits of info between the correspondance dates
  - unable to re-save the file though on the command line it says "error writing texas.txt: Permission denied"
  - just copied the text to put it into a text editor but only ended up having 5 lines copy over
  - used the file from before in the text editor to get rid of the extra wording
  - it seems to be working out now
  - followed the command in the tutorial to put the ~ in front of all the letter texts
  - it all worked out well, time to get rid of the extra stuff
  - put all the lines with the ~ into the index.txt file
  - trying to get the thing to delete the page files using code "sed -r -i.bak'/(,)( [0-9]{4})(.+)/\/g' index.txt"
  - gave response "sed: no input files"
  - looked for a way to fix the problem/looked up the problem online, coud not find any help
  - one of the other students showed me what i was doing wrong in the code and changed it to "sed -r -i.bak 's/(,)( [0-9]{4})(.+)/\2/g' index.txt"
  - proceed to remove the ~ from the text afterwards " sed -r -i.bak 's/~//g' index.txt "
  - proceed to change the to in the file to "," sed -r -i.bak 's/(\b to \b)/,/g' index.txt
  - then to make sure that you get all of the extra "," out open the file in text editor
  - copy the file into regexr, and use the code .+,.+,.+,  to highlight where the extra "," are
  - go through and manually delete the extras
  - save file, and switch it for the one in dhbox
  - turn file into csv file with "cp index.txt cleaned-correspondence.csv"
  - boom shaka laka, I did it and didn't go crazy doing it!
  
  ## Exercise 2
  http://workbook.craftingdigitalhistory.ca/supporting%20materials/open-refine/ 
  - Downloading open refine to the computer
  - first opened the .csv file in openRefine, it was not in columns
  - took that file opened it in excel and resaved it as an excel file, then when opening that file in open refine, it had the columns
  - going through clustering the names using the nearest neighbour method
  - putting different numbers in for Radius and Bloc Char
  - had to manually go through a couple names and edit them
  - changed the sender and receiver names to source and target so that I could use the information on a  different interface
  - exported them
  - Opened the file in Palladio
  - there appears to be a few people who send letters to multiple people
  
  # Module 4
  
  ## Exercise 2
  - copied Dr. Grahams Scotland Newspaper text into DHBox
  - saved file
  - download file to my own computer
  - Download topic modelling tool from Github
  - used the topic modeller, and set it to model 10 topics
  - with only 10 topics, it did not make much sense
  - changed it to 30 topics and ran the system again, this time being given a more understandable outcome
  - doing it in this way allowed for a more comprehensible way of understanding the document, without reading all of it
  
  ## Exercise 6 
  -Using voyant tools
  - open up the webpage and paste the following link to have information to work off of https://raw.githubusercontent.com/shawngraham/exercise/gh-pages/CND.csv
  - tried loading it multiple times, but it kept on crashing on me
  - not exactly sure why, I tried using different browsers, but was still unable to get it to work without crashing
  
