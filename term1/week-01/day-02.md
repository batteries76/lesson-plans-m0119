# Day 02 — Terminal & Setup
## Outcomes
The idea is to reveal how the terminal commands work to help them understand a developer environment before installing ruby. This gives the student a good grounding on how to deal with files and folders within the terminal and any of the terminal commands. It isn't essential they remember every command - but they do need to know

## On successful completion of this unit students will be able to:
- use basic commands ```mkdir``` ```cd``` ```touch```
- have a better understanding of the terminal, bash and the file system at a high level
- a brief understanding of SSH (Secure Shell)

## Other topics
- Repeat ideas about getting help, growth mindset, working through procrastination, and emotional intelligence. 
- Consider these things to be sharpening the axe. 

## Guided instructions
- video [How Linux is built](https://youtu.be/yVpbFMhOAwE)
Note: Read Outcomes
Cover: 
```linux
uname 
users #show users
uptime
cal #calendar
whoami #who am i
pwd #print working directory
ls #list directory contents
mkdir #make directory
cd #change directory
touch
which #where is command (file)
file #view file details
```
Good time to talk about "blob" character * and how it finds a file by extension
```
less
more
echo
> #newline 
>> #write 
| #pipe
cat #concatenate files
wc #word count to count text document
mv #move
ditto #copies content form one folder to another
cp #copy
rm #remove
```
The next part with zip is useful to students to who should usually present their work uploads in zip format.
```
zip 
unzip
man #manual
info #information
top #table of processes
kill #kill program
history #show bash history
grep #globally search a regular expression 
date
sleep
nano #small text editor
vim / vi
```
- breifly discuss where the scripts/executables are kept ```cd /var/bin/```
- breifly discuss how all items on a hard drive are either files or folders
- breifly discuss os system folder structure

### Optional

```linux
curl #Client for URLs
ip addr show
wget #web get
```

[Install homebrew](https://brew.sh/)

Install *tree* using homebrew

Have fun with telnet 
```linux
brew install telnet
telnet towel.blinkenlights.nl
telnet rainmaker.wunderground.com
telnet telehack.com
``` 
(run/type eliza for an interactive ai in telehack.com)

### Lastly for fun
- terminal ```say “Thank you for listening”```
- Let students know they will be building their own terminal app
- SSH into your mac from a students computer

### SSH
- If on mac turn on System Preferences > Sharing > Remote Login
- Get ssh address i.e. ```Ruegen@192.168.0.1```
- Open students laptop terminal
- Type ```ssh <address>``` (use -p22 flag if fails)
- add and delete files on desktop from student computer


### Leave off 
Leave these for later sessions

Do not go through ```chmod```
Do not go through ```base64```

## Resources 
[Terminal cheetsheet](https://github.com/0nn0/terminal-mac-cheatsheet)


## Install Ruby
- Install rbenv 1.1.1
- Ruby 2.5.1

## Setup
Even though students may not use all these services in the first 3 weeks it is important to get them prepared early.
- Install [Slack](https://slack.com/)
- Install [VS Code](https://code.visualstudio.com/)
- VS Code demo (extensions, file explorer etc)
- Mac users install [Dash](https://kapeli.com/dash)
- Windows users install [Velocity](http://velocity.silverlakesoftware.com/)
- Linux users install [Zeal](https://zealdocs.org/)
- Signup for [Codepen](https://codepen.io/)
- Signup for [Trello](https://trello.com/)
- Signup for [Figma](https://figma.com/)
- Signup for [Meetup](https://meetup.com/)
- Signup for [Github](https://github.com/)

## Resources
- [GNU Bash](https://www.gnu.org/software/bash/)
- [Unix commands list](https://en.wikipedia.org/wiki/List_of_Unix_commands)
- [Hard Skills/Soft Skills](https://www.youtube.com/watch?v=0FFLFcB9xfQ)
- [Telnet history](https://www.britannica.com/technology/Telnet)

## Challenges
Day 02 - Terminal Stuff
Scott’s challenges
One: Terminal —
Using only terminal, navigate your file system to:
    1. Create a file structure that matches your family tree e.g. a root folder with 2 grandparents, 2 parent directories in each with child folders within those
    2. Create a folder called students. Inside the folder, create a few student text files 'jane.txt', etc
    3. Rename one of the student files to include full names ('jane doe.txt') - note what happens if you try to use a space. How can you get around this?
    4. Delete one student
Two: Running Ruby —
    1. Open IRB from your command line by running `irb`
    2. Try some basic math (1+1 *enter*)
    3. Quit IRB by sending the `exit` command
Three: Running Ruby from a file —
    1. Use terminal to create a new file (e.g. `touch my-cool-app.rb`)
    2. Open the file in your code editor (e.g. `atom my-cool-app.rb`)
    3. Write the same Ruby code (1+1) and save + close the file.
    4. Run the code! We can do this with the `ruby` command. (e.g. `ruby my-cool-app.rb`)
    5. The code runs, but nothing is returned on the screen. Add `puts` to the start of your code and try running the code again! (e.g. `puts 1+1`)
    6. Experiment with some basic ruby!
My Challenges
One: Man —
    1. Google some interesting commands
    2. Use the ‘man’ command to read about the command you have found
    3. Experiment with this command, and its flags
Two: Help —
    1. Repeat the above process, but use the —help flag to get info on the command

## Units
- Terminal & Running Ruby
- Tools & Installation
 
