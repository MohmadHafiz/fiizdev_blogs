![[Pasted image 20250207205051.png]]

I remember someone asked me how to hack, and how do i start hacking, previously in this blog [WHOAMI.dll](https://fiizdev.com/blog/post/WHOAMI.dll) i talked about my 9-10 years experience on what i did, hacking is not something for people that have limited knowledge in using computer like someone only been using their computer for watching movies, youtube, and using microsoft words. For me actually anyone can be hacker if they really love to explore on how stuff works and how you take advantage that stuff or exploit it. But in hacking there are a lot of stuff and a lot of things that you can explore, for example there's hacking in networking, hacking in software and hardware, hacking in communication, etc. for this journey I'll will guide you into how to start hacking.

What you need? well what you need is getting comfortable with CLI/Terminal/CMD, this stuff you gonna be use a lot. CLI/Terminal/CMD is software in most every devices such as computers, servers, mobile phone, WIFI router, etc. most tools for hacking are using Terminal for you to interact, Terminal is just a software that you enter a command and getting text output on the Terminal, let's try this simple command if you are using windows:

- first you need to run CMD, windows key + s key
- then you type 'cmd'
![[Pasted image 20250207195823.png]]

- you will see this software show up on your search, just click it
- when you click it, this window will show up
![[Pasted image 20250207195926.png]]

- start typing `ipconfig`, and click enter!
- there you are voila! you are now a hacker!
![[Pasted image 20250207200445.png]]

What you are looking at is output of the command about your computer network interface, it shows IPv4 Address & Default Gateway, this two is important when someone ask you "what is your computer IP Address" you'll gonna give them IPv4 Address. each computer that connected to a network for example Wireless router will be assigned with its IP address, some network needs to be assigned IP Address & Gateway Address manually.

So what is Gateway Address? it is your router IP Address, any network packets/traffic/data from your computer will go through into this Gateway or your router and your router will send it to your ISP and will be pass to its destination then the output data will back to your computer.
![[Pasted image 20250207201416.png]]

let's go back to terminal, let's type something on your CMD, try this :
```cmd
echo hello, world!
```

![[Pasted image 20250207201627.png]]

you just make your computer to say something! congrats!, so what that command does is just 'echoing' or 'print' something into terminal whatever you put after 'echo'. so you wonder what 'C:\\Users\\zeus>' is? that is the location where you are right now inside your computer. 'C' is your SSD/HDD letter commonly C is the main storage, most software are installed/put inside this storage including your Operating System which is windows files. '\\Users\\zeus' is the location or folder. you can try type this command:
```cmd
dir
```

![[Pasted image 20250207202821.png]]

What you just type and see here is list down most of the stuff inside your current location, form the output of the command you can see 'drive C', 'Directory', dates, time and numbers. the 'drive C' shows your what drive are you currently on, 'Directory' also tells you where are you right now in the CMD, and dates, time, numbers are the stuff that you will make you dizzy to look at right now but it is ok don't worry about it.

so the `<DIR>` that you see are telling you that is directory/folder, after `<DIR>` is the name of folder example '.android' or '.ssh', so the thing that does not have `<DIR>` is a file but it got numbering? and that is the size of the file, after the size of the file is the name of the file, so dates and time are just telling you what time and date this folder or files are modified or created. what is `.` and `..` ?...

Now you know how to list down stuff inside a folder, lets do navigation here i will explain what `.` and `..` are, when you navigate from folder to another folder usually you just click on it, here you just type, the command to navigate inside CMD is `cd` basically means 'change directory', lets navigate into your 'Desktop' folder, type this:
```cmd
cd Desktop
```

when you enter that command you realize this thing change:
![[Pasted image 20250207205002.png]]

that means you successfully navigate into your Desktop folder, you can type `dir` command to see what inside your desktop folder, but how are you gonna go back? well here what `..` is, basically it means directory before where you are right now, to go back before your Desktop folder you can type this:
```cmd
cd ..
```

if you're on the root or on the first folder of your drive `\` when you type `dir` you won't see `.` or `..` on it because you're already at the first folder of your drive, here is the example:
![[Pasted image 20250207205744.png]]

when you want to open text file, your will use your notepad? right? to see what inside the text file or any file, well you can do that using your CMD, you can use `type` command to do that but you won't be able to edit the file like using notepad. here try this `type` command:
```cmd
type <filename>
```

`<filename>` you should replace it with a file name, if you don't know what file to see, try use `dir` command and look for a file that have numbering on the left, here are the example:
![[Pasted image 20250207210517.png]]

Alright we are done here with the basic commands for CMD, i hope you learn some stuff using CMD, next blog we will escalate into next level of using Linux, don't worry about that if you're using Windows 11/10 its easy to install 