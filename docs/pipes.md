  <a name=top><br>
  <p align=center>&nbsp;<a href="/README.md#top">home</a> ::
  <a href="/docs/syllabus.md#top">syllabus</a> ::
  <a href="https://drive.google.com/drive/folders/1ZFn6H8-4kx5uP34bpFgIFonkz9Tw3nYM?usp=sharing">groups</a> ::
  <a href="https://moodle-courses2021.wolfware.ncsu.edu/course/view.php?id=3873">moodle</a> ::
  <a href="">chat</a>  ::
  <a href="/LICENSE.md#top">&copy;&nbsp;2022</a><br>
  <a href="/README.md#top"><img width=600  
     src="/etc/img/ase23.png"></a></p>
  






## Before reading..


Before reading this material, review [these slides](https://swcarpentry.github.io/shell-novice/04-pipefilter/index.html)


## History


Doug McIlroy, Bell Labs’ “Computing Techniques
Research Department” 1986
-   “We should have some ways of coupling programs like garden hose.” 
- "Let programmers screw in another segment when it becomes necessary
to massage data in another way.”
- “Expect the output of
 every program to become the input to another, as yet unknown,
 program. Don’t clutter output with extraneous information.”


Pipes changed the whole idea of UNIX:


- Implemented in 1973 when ("in one feverish night",
wrote McIlroy) by  Ken Thompson.
- “It was clear to everyone, practically minutes after the system
came up with pipes working, that it was a wonderful thing. Nobody
would ever go back and give that up if they could.”
- The next
day", McIlroy writes, "saw an unforgettable orgy of one-liners
as everybody joined in the excitement of plumbing." 


Pipes changed how we think about software


- Not applications
- But tools.
  - Compose the things together, if you
had made them so that they actually worked together. 
  - People went back and consciously put into programs the idea that they read from a list of files 
  -  And  if there were no files they read from the standard input so that they could be used in pipelines.


You've probably all used pipes already. Here we download an install shell script  then pipe it to the `sh` command
(so it runs)


```
curl -s http://example.com/install.sh | sh
```


(By the way, that is a security risk. [Use with care!](https://blog.dijit.sh//don-t-pipe-curl-to-bash))


Examples
- `nroff` is a text formatter (old version of latex)
- `lp` is the line printer
- `col` handles escape sequences that sets up text in 2 columns
- `tbl` is an nroff pre-processor that expresses tables in terms of lower-level nroff commands
- `eqn` is an nroff pre-processor that expresses equations in terms of lower-level nroff commands


```bash
nroff files | col | lp


tbl file-1 file-2 . . . | eqn | nroff -ms
````


Think of pipes as `produce`, `translate`, `filter`, `consume`:


```bash
find /usr/bin/ |                #produce 
sed 's:.*/::'  |                #translate: strip directory part
grep -i '^z'   |                #filter   : select items starting with z
xargs -d '\n' aFinalConsumer    #consume 
```


Note that in the above, the `filters` inside the `pipes` could be written in any language at all, by different teams.


Also, operating systems _love_ pipes since they can run each part of the process as a separate process,
maybe even on different machines (\*)


(\*) That said, there is the data bus / network cost of streaming data between parts of the pipe. 


Dumb and smart way to implement pipes
- Dumb: use disc files  for the spooling in the piles (lots of file I/O)
- Smarter: 
  - use specialized RAM disks to handle the pipe internal memory (much faster)
  - have some buffer inside the pipe
    - start writing to downstream before upstream finishes
    - when the small buffer is small


Advantages:
- Divides one task into N parallel tasks
  - Gives the operating system a better change to help out
- Demands that large problems get divided into big chunks with simple interfaces
  - Project simplification 
- Method to divide human effort (different developers, different parts of the pipe)
- Method  to mix and match between different languages
  - code in different parts of the pipe can be coded in different languages
- Lets you test things, before they finished:
  - You can "mock" upstream component, even before it is fully builds.
  
Disadvantages:


- Carrying complex data between different parts of the pipe. 
- Assumes a one-way flow, here to there
  - Not good for GUI environments where users want to call functions in any order
  - Which makes pipes are more an "under the hood" idea
- Also, I've had problems with pipes and concurrency: sending data off on long retrieval arcs (e.g. from another part of the network)
  - But that's just me


