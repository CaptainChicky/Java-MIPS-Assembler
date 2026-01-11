## What is this?
This is a Java **M**IPS assembly **a**ssembler and **r**untime **s**imulator, or as a shorthand, "MARS".

It, well, allows you to simulate running MIPS assembly without actually needing the CPU/hardware to do it lol. Nothing more to be said tbh.

Off we go into the wild blue yonder,<br>
Climbing high into the sun;<br>
Here they come zooming to meet our thunder,<br>
At ‘em now, Give 'em the gun!<br>
Down we dive, spouting our flame from under,<br>
Off with one helluva roar!<br>
**We live in fame or go down in flame. Hey!**<br>
**Nothing'll stop the U.S. Air Force!**

<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/c/c1/F-22_underside.jpeg/960px-F-22_underside.jpeg" />

Brilliant minds fashioned a crate of thunder,<br>
Sent it high into the blue;<br>
Valiant hands blasted the world asunder;<br>
How they lived God only knew!<br>
Boundless souls dreaming of skies to conquer<br>
Gave us wings, ever to soar!<br>
With scouts before and bombers galore. Hey!<br>
Nothing'll stop the U.S. Air Force!

Even though it's pretty useful and can be used as an IDE, I highly do not recommend doing it as so, just stick with your favorite IDE and copy/paste code into here to assemble and run. For example, VSC with a MIPs formatter and highlighterwhateveritscalled 🥱

Java is truly, truly, the worst language ever.

˖ ݁♬⋆.˚𝄞. Небо над водой, над рекою белый дым, <br>
Ходят кони к водопою утром ранним. <br>
С неба звёзды отражаются в воде, <br>
Да ковыль-трава, ой да, вся в росе.
 
Заберу с собою я землицы горсть, <br>
Пусть она в чужой стране меня спасёт. <br>
В БожьемOn kauniina muistona Karjalan maa, <br>
mutta vieläkin syömmestä soinnahtaa, <br>
kun soittajan sormista kuulla saa, <br>
Säkkijärven polkkaa! ♫⋆｡♪ ₊˚♬ ﾟ.

<u>Shitty ass language, shitty ass classes who teach this language, and shitty ass people who teach said classes.</u> For instance, a certain person who forks the main branch, writes a bunch of unprofessional cringeworthy comments, dubious todos without understanding code structure ("omg there's a null lets write a todo without understnadng the null is acttually accounted for" 🏇😂 and then clog up my linter with todo messages!!!! how fun!!1!!!!!"), blocks he ability to type a certain whitespace character with an annoingyass 50 gorillion character string😂😂😂😂😂god forbid this guy ever touches any code that I have to be near 🥀 (which unfortunaltey i will have the displeasure of experiencing this burden perhaps a multitude of times😂)<br>
But anyhow i suppose it doens't hurt to use this (this as in MIPS asm programming langauge) as a entrypoint into low level stuff, it's meh ig. 🐔😊🤓🥀💔 I\<3✡️I<3✡️I<3✡️I<3✡️I<3✡️I<3✡️I<3✡️I<3✡️I<3✡️I<3✡️ COMPILERS, I LOVE COMPILERS! GREAT GOOD HEAVENS, HAVE YOU TRIED DEVVING FOR GCC???? HOLY COMPILERS!!

Two days ago upon turning off all the lights and sleeping I was caught into a sleep paralysis after telling the dream people that they weren't real which caused me to panic. Eventually I tried waking but got into an SP then felt myself getting touched inappropriately everywhere it made me uncomfortable, all while I had random static noises in my ear coming from the sleep paralysis. Because of this I am now fearful of the dark and get flashbacks whenever I enter a room with the lights turned off.

How do I avoid further Sleep Paralysis?

## Project Structure
I'll include just stuff that is of note, the rest will be ommitted because it's kinda obvious what they are.
```
root
  │   compile.bat                    - Actual compilation script
  │   Mars.java                      - Main entrypoint of program
  │   ALUcontrolDatapath.xml       ─┐
  │   Config.properties             │
  │   controlDatapath.xml           │  
  │   MipsXRayOpcode.xml            │  These files are used during compilation
  │   PseudoOps.txt                 │  and will be part of the compiled program
  │   registerDatapath.xml          │       
  │   Settings.properties           │       
  │   Syscall.properties           ─┘  
  │   java_files.txt                 - Used to track which files to compile
  │   mainclass.txt                  - Used to track main entrypoint to compile
  │   resource_hacker.zip            - Tool to insert image into installer executable
  │
  ├───help                           - Documentation included within the program
  ├───images                         - Images used during compilation
  └───mars                           - Core assembler & simulator engine
      ├───assembler
      ├───mips                       - MIPS instruction set & hardware simulation
      ├───simulator
      ├───tools                      - Extensions/tools MIPS code can interact with
      ├───util
      └───venus                      - GUI/IDE (text editor, windows, menus)
```
Whoever wrote `/help/` (so called "professional" "computer science" people) do **NOT** know how to write proper HTML lmao its an ugly ass mess I cringe when looking at. Viewer discresion is advised.

Here's a toast to the host<br>
**Of those who love the vastness of the sky,**<br>
**To a friend we send a message of the brave who serve on high.**<br>
We drink to those who gave their all of old<br>
Then down we roar to score the rainbow's pot of gold.<br>
A toast to the host of those we boast, the U.S. Air Force!

Off we go into the wild sky yonder,<br>
Keep the wings level and true;<br>
If you'd live to be a grey-haired wonder<br>
**Keep the nose out of the blue!**<br>
Fly to fight, guarding the nation's border,<br>
We'll be there, followed by more!<br>
In echelon we carry on.<br>
**Oh, nothing'll stop the U.S. Air Force!**

<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/4/46/Lockheed_Martin_F-22A_Raptor_JSOH.jpg/1280px-Lockheed_Martin_F-22A_Raptor_JSOH.jpg" />

Minds of men fashioned a crate of thunder,<br>
Sent it high into the blue;<br>
Hands of men blasted the world asunder;<br>
How they lived God only knew! (God only knew, then!)<br>
Souls of men dreaming of skies to conquer<br>
Gave us wings, ever to soar!<br>
With scouts before and bombers galore. Hey!<br>
Nothing'll stop the Army Air Corps!

Trying to actually understand the source code in `/mars/` is substantially difficult tbh. It isn't hard to understand parts of it, but these retards have like broken ass code where they cast actually needed operations onto useless code and retarded java IDE thinks 🐵🧏‍♀️🧏‍♀️🧏‍♀️🤫oo oo we can delete this variable and all isntances of it and does it and then completely fucking breaks the program because the actually needed operations are actually needed. Understanding the code in small chunks (aka as a debugging maintainer on non-self-written source code perspective instead developer-who-wrote-unmaintainable-code perspective) isn't too bad, but try to pierce everything together and it's truly a clusterfuck. At least a general overarching gist isn't too hard to get (which ive also supplied in the diagram above, observe as follows 🤓)

THE AMOUNT OF FUCKING RAWTYPES AND UNCHECKED WARNINGS LITERALLY IS MORE TIMES THAN EPSTEIN HAS BEEN WITH CHILDREN HOLY FUCKING HELL 😪🤮THESE PEOPLE DO NOT KNOW HOW TO USE FUCKING TYPES `ARRAYLIST<TYPEEEEEEE>` WHERE IS THE TYPEEEE?!?!?!?!?!?!?!?!!!!?! GOD FORBID SOMEONE WANTS TO SAVE THEIR EYES FROM THE 844 FUCKING WARNINGS THE JAVA LINTER SHOWS LMAO AND ALSO STOP MAKING VAIRBALES AND IMPORTS YOU NEVER USE HOLY SHIT THERES AT LEAST 5 PER FUCKING FILE OF IMPORTS YOU DONT USE!1!!!!!! PLEASE I BEG!!!

🎶
Калинка, калинка, калинка моя! <br>
В саду ягода малинка, малинка моя! <br>
Калинка, калинка, калинка моя! <br>
В саду ягода малинка, малинка моя! <br>
Калинка, калинка, калинка моя! <br><br>
В саду ягода малинка, малинка моя! <br>
Ах ты! Красавица, душа-девица <br>
Полюби же ты меня! <br>
Ах! Полюби же ты меня!
🎵

## Compilation
I've made it pretty easy, just run `compile.bat`. It will compile all the main source code in `/mars/` and `Mars.java` into a `/compile/` folder. Then it will make a wrapper jar file that contains all the files (so you basically can run it standalone, assuming you have java installed) into `/build/`. After it makes that, it will use WiX to create an executable installer version of the program in `/build/`. It will then delete the `/compile/` dir.

Did you know that if you already have an executable in `/build/`, the WiX will simply append the new executable it's tryign to make on the old one??? Well I didnT1 😴🥱 and i ended up with a file that was 250 mb after compiling it 5 times (in case you can't tell, normal size is 250/5 = 50 MB).

The executable doesn't have an icon, so you can use the included `resource_hacker.zip` to insert an icon like `/images/truemars.ico` into the exeuctable at your discresion.

This program is made for windows only, if you're on mac go fucking kys.

## Dependencies
The .jar file apparnetly Java J2SE 1.5+ SDK runtime. I've been able to run it fine with whatever java SDK i have so as long as you have java you should be fine ig<br>
To compile to executable installer, you need specifically 3.11.x version of WiX. It can't be any other version.<br>
You need to have a brain to be able to double click the compilation script.<br>
You also need to not be cringe aka stop writing MIPS now and go learn real code lmfao 🥱

67 has ruined my fucking life and I can't take it anymore. 

I literally cannot do this anymore. I am at my FUCKING limit. 67. Six. Seven. It started as a joke. Just a funny number. A funny fucking number that a kid did in that damn video. But it kept popping up in my fucking reels. What the fuck is going on? I ask myself. At first, I thought it was funny. But I kept seeing it. Not by the major but it was JUST SIX SEVEN AFTER SIX FUCKING SEVENS. I kept blocking those accounts. Nothing worked. I tried a new account alltogether. It still appeared. I even made a newer account with a VPN. NOTHING. FUCKING. WORKS.

"SIX SEVENN!" Haha. Funny. Right? WRONG. This number has systematically dismantled every single aspect of my already pathetic life.

I'm a father of two kids. They're the ones who's always stuck to their screens 26/7. I tried asking them of how to stop it or at the very least explain what it means. I didn't get a clear answer. Instead, they mimic that blonde fucker's hand movements and kept saying "SIX SEVEN" in the most obnoxious tone possible. I felt like crying.

I lost my six-figure job last week. I tried to ignore this whole six seven bullshit and just go to my job. We were in the middle of the most important meeting in the company's history. The CFO pulls up the quarterly projections. The presentation hits a page that showed a pie chart. I look at the screen. The percentage? 67% out of whatever the fucking topic was. I didn't place it there. I swear I didn't. I swear I remember deliberately putting it as 66% just to prevent this exact scenario.

I didn't mean to do it. It was a reflex. I swear. I slammed my hand on the mahogany table and screamed "SIX SEVENNN" at the top of my lungs. I started laughing hysterically, pointing at the screen yelling "SIX SEVEN! SIX SEVEN! SIX SEVEN" at the board of directors. Security escorted me out while I was still trying to explain the meme to those old wrinkly fuckers.

My career is utterly over. I can't even get hired at a cashier job because I'm fucking blacklisted from the local job market. I have ruined my reputation and I cannot fix it no matter how much I beg for forgiveness.

But it didn't stop there. My wife left me yesterday. We were driving to see her parents. I looked at the dashboard. The temperature outside? 67 degrees. I started sweating. I looked at the speedometer. 67 mph. I started hyperventilating. I couldn't help myself. I involuntarily moved my hands up and down while saying six seven. I pulled the car over on the highway and refused to drive until the temperature dropped to 66 or rose to 68. She told me I need professional help. She took the ring back. I lost the divorce. I lost the kids. I lost all of my money. I'm dirt poor.

I see it everywhere now. My phone battery? 67%. The change in my pocket? 67 cents. The page number in my book? 67. I can’t sleep. I can’t eat. I close my eyes and I just see the number floating in the void. It haunts me. It mocks me. I am a shell of a man, destroyed by a double-digit integer. Is this what god does to his strongest soldier? I can't fucking take it.
# SIX SEVENNNN SIX. FUCKING. SEVEN. 67 67 67 67 67 GOD FUCKING DAMN IT SIX SEVEN SIX SEVEN SEX SEVEN SIX SEVEN SIX SEVENNN SIX SEVENNNN SIX SEVENNNN SIX SEVENNNN SIX SEVENNNN SIX SEVENNNN SIX SEVENNNN SIX SEVENNNN SIX SEVENNNN SIX SEVENNNN SIX SEVENNNN SIX SEVENNNN SIX SEVENNNN SIX SEVENNNN SIX SEVENNNN 