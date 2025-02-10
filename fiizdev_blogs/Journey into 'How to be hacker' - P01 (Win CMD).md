![[Pasted image 20250207211736.png]]


I remember someone asked me how to hack, and how to start hacking, previously in this blog [WHOAMI.dll](https://fiizdev.com/blog/post/WHOAMI.dll) I talked about my 9-10 years of experience on what I did, starting in hacking path is not something for people that have limited knowledge in using a computer as someone has only been using their computer for watching movies, you tube, and using Microsoft words because you need to do practical stuff a lot like remembering what commands to enter, or what button to push. For me actually, anyone can be a hacker if they love to explore how stuff works and how you can take advantage of that stuff or exploit it. But in hacking, there is a lot of stuff and a lot of things that you can explore, for example, there's hacking in networking, hacking in software and hardware, hacking in communication, etc. For this journey, I'll be guiding you on how to start hacking.

## Open CMD and simple command

What do you need? Well, what you need is to get comfortable with CLI/Terminal/CMD, this stuff you gonna be using a lot. CLI/Terminal/CMD is software in almost every device such as computers, servers, mobile phones, WIFI routers, etc. Most tools for hacking are using Terminal for you to interact, Terminal is just software that you enter a command and get text output on the Terminal or command your computer to do some cool stuff, let's try this simple command if you are using windows:

- first, you need to run CMD, `WINDOWS key` + `S key`
- then you type '`cmd`'
![[Pasted image 20250207195823.png]]

- you will see this software show up on your search, just click it
- when you click it, this window will show up
![[Pasted image 20250207195926.png]]

- start typing `ipconfig`, and click enter!
- there you are voila! You are now a hacker!
![[Pasted image 20250207200445.png]]

What you are looking at is the output of the command about your computer network interface, it shows IPv4 Address & Default Gateway, these two are important when someone asks you "What is your computer IP Address" You'll gonna give them an IPv4 Address. Each computer that is connected to a network for example Wireless router will be assigned with its IP address, some network needs to be assigned IP Address & Gateway Address manually.

So what is Gateway Address? It is your router IP Address, any network packets/traffic/data from your computer will go through into this Gateway or your router and your router will send it to your ISP and will be passed to its destination then the output data will back to your computer.
![[Pasted image 20250207201416.png]]

## Echo!

Let's go back to the terminal, let's type something on your CMD, and try this :
```cmd
echo hello, world!
```

![[Pasted image 20250207201627.png]]

You just make your computer to say something! Congrats!, so what that command does is just 'echo' or 'print' something into the terminal whatever you put after 'echo'. 

## dir!

So you wonder what 'C:\\Users\\zeus>' is? That is the location where you are right now inside your computer. 'C' is your SSD/HDD letter, usually C is the main storage, most software is installed/put inside this storage including your Operating System which is Windows files. '\\Users\\zeus' is the location or folder. Try typing this command:
```cmd
dir
```

![[Pasted image 20250207202821.png]]

What you just type and see here is a list of most of the stuff inside your current location, form the output of the command you can see 'drive C', 'Directory', dates, time, and numbers. The 'drive C' shows you what drive are you currently on, 'Directory' also tells you where are you right now in the CMD, and dates, times, and numbers are the stuff that will make you dizzy to look at right now but it is ok don't worry about it.

So the `<DIR>` that you see is telling you that is a directory/folder, after `<DIR>` is the name of the folder example '.android' or '.ssh', so the thing that does not have `<DIR>` is a file but it got numbering? And that is the size of the file, after the size of the file is the name of the file, so dates and time are just telling you what time and date this folder or files are modified or created. What is `.` and `..` ?...


| Column 1              | Column 2              | Column3               | Column 4  | Column 5  |
| --------------------- | --------------------- | --------------------- | --------- | --------- |
| Date modified/created | Time Modified/created | if `DIR` means folder | file size | file name |


## Change DIR..

Now you know how to list down stuff inside a folder, let's do navigation here I will explain what `.` and `..` are, when you navigate from one folder to another folder usually you just click on it, here just type, the command to navigate inside CMD is `cd` basically means 'change directory', let's navigate into your 'Desktop' folder, type this:
```cmd
cd Desktop
```

When you enter that command you realize this thing has change:
![[Pasted image 20250207205002.png]]

That means you just successfully navigated into your Desktop folder, you can type the `dir` command to see what is inside your desktop folder, but how are you gonna go back? Well here is what `..` is, basically it means the directory before where you are right now, to go back to your previous folder you can type this:
```cmd
cd ..
```

If you're on the root or the first folder of your drive `\` when you type `dir` you won't see `.` or `..` on it because you're already at the first folder of your drive, here is the example:
![[Pasted image 20250207205744.png]]

## Open a file

When you want to open a text file, you will use your notepad. Right? To see what is inside the text file or any file, well you can do that using your CMD, you can use the `type` command to do that but you won't be able to edit the file like using Notepad. Here try this `type` command:
```cmd
type <filename>
```

`<filename>` you should replace it with a file name, if you don't know what file to see, try using the `dir` command and look for a file that has numbering on the left, here is the example:
![[Pasted image 20250207210517.png]]

## END :D

Alright we are done here with the basic commands for CMD, i hope you learn some stuff using CMD, next blog we will escalate to the next level using Linux, don't worry about that if you're using Windows 11/10 It easy to install

