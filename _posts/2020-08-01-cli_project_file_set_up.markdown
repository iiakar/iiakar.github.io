---
layout: post
title:      "CLI Project File set up"
date:       2020-08-01 20:06:24 +0000
permalink:  cli_project_file_set_up
---


While working on my CLI project, for some reason I had very difficult time setting up the files with require_relative. After browsing some videos to figure out how to do it and after taking some notes, I wanted to write a short description of some points that could make your life easier.  

You can see my project here[https://github.com/iiakar/premierleaguetable]. 

 In this repository, there are three classes. CLI, Scraper, and Team that shows Premier League soccer teams ranking in the program. 

For easy review, I made the files without the code and took a screen shot of it. 
 
https://ibb.co/NLcVG2N

In this case .rb file extension is for running code in Ruby. 

One of the key points to do is to name your main file under library and the file that will hold the names of the other classes the same. 

In my files, it's the 'leaguetable'. If you are using Bundlr to generate your gem, it will do it for you automatically with the name you specify when you make the gem. (for example: bundle gem leaguetable). 

The first thing to do is to add a shebang line in your console file. This will tell the editor, the language you use. In this case it is Ruby. 

https://ibb.co/nbW1Yvs

As you can use, we also use require_relative '../lib/leaguetable' without any extensions (like .rb for Ruby) to load the files.

https://ibb.co/VW0McKw

After requiring '../lib/leaguetable' in your Console file in your Bin folder, you can type the name of all your classes inside the first file under the library. 

Even though we required all the files without an extension inside the Console, since we named the main library and libraryfile with .rb extension the same name, the editor will still read it.

Just to see if our set up is working, I added some text each class to see if prints to the screen when we run our program from the console. 

https://ibb.co/yp7zn0x

https://ibb.co/tZ5RnYC

https://ibb.co/vvpsXQ5


Now let's run the bin file. 

Once you are in the bin file, you can type 'ls' to see the list of the files. Then 'ruby file_name' to run the program since with shebang line, we specified the language we are gonna use. 

https://ibb.co/GknGN40

Just to consolidate everything, it's Console calling one file name, files having classes or codes inside them, then using require_relative with all the file names inside a single file under library. 

https://ibb.co/Hz4TYwP

https://ibb.co/Pwd67Rq

https://ibb.co/pzgVrV7

