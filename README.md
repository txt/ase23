<a name=top><br>
  <p align=center>&nbsp;<a href="/README.md#top">home</a> ::
  <a href="/docs/syllabus.md#top">syllabus</a> ::
  <a href="https://docs.google.com/spreadsheets/d/1YHZPRLfchksx541yaojJE_loOh2g4FaVKtrVcquoYIw/edit#gid=0">groups</a> ::
  <a href="https://discord.gg/FYwfQuNzPB">chat</a>  ::
  <a href="/LICENSE.md#top">&copy;&nbsp;2023</a> <a href="http://menzies.us">timm</a><br>
  <a href="/README.md#top"><img width=600  
     src="/etc/img/ase23.png"></a></p>





<table width="100%" border=0 align=center>
<tr>
<td></td>
<td align=center width=300><img           src="/etc/img/lectures.gif"></td>
<td align=center width=300><img  width=64 src="/etc/img/time.png"></td>
</tr>
<tr>
<td></td>
<td align=center><b>Lectures</b></td>
<td align=center><b>Timetable</b> </td>
</tr>
<tr>
<td width=500>

<p>
This subject is a peek under the hood of 
   under the hood of data mining, optimization, theorem proving and all the other tricks of automated software engineering.

<p>
This is a project-based class where students will use any scripting language they like  to build and extend their own AI tools for software engineering. 
 500 level students will work in groups.

<p>Topics covered: 
 scripting;
 clustering;
 optimization;
 data mining;
 theorem proving;
 requirements engineering;
 discretization  ;
 explainable AI, ;
 statistics for experimental algorithms,;
 hyper parameter optimization;
 deep learning

<p>Grading: 21% homeworks, 40% exams; 36% for large end-of-term project.

<p>Textbook: none


</td>
<td valign=top  xwidth="100px">

<!-- -------------------------------- -->
<dl>
<dt>
Lectures:
<dd>
Jan11&nbsp;:&nbsp;<a href="https://github.com/timm/tested/blob/main/docs/onFishing.md">fishing</a><br>
Jan18&nbsp;:&nbsp;<a href="https://github.com/timm/tested/blob/main/docs/onScript.md">script</a><br>
Jan25&nbsp;:&nbsp;<a href="https://github.com/timm/tested/blob/main/docs/onData.md">data</a><br>
Feb1 &nbsp;:&nbsp;<a href="https://github.com/timm/tested/blob/main/docs/onCluster.md">cluster</a><br>
Febs8 &nbsp;:&nbsp;<a href="https://github.com/timm/tested/blob/main/docs/onOptimize.md">optimize</a><br>
Febs8 &nbsp;:&nbsp;<a href="https://github.com/timm/tested/blob/main/docs/onOptimizeExamples.md">optimize(e.g.s)</a>
<br>
Feb15 &nbsp;:&nbsp;<a href="https://github.com/timm/tested/blob/main/docs/onRe.md">req.eng</aa><br>
Feb22 &nbsp;:&nbsp;<a href="https://github.com/timm/tested/blob/main/docs/tbd.md">...</a><br>
Mar1 &nbsp;:&nbsp;<a href="https://github.com/timm/tested/blob/main/docs/tbd.md">...</a><br>
Mar8(wed)&nbsp;:&nbsp;mid-term,&nbsp;4:30</a><br>
Mar15 (break)</a><br>
Mar21&nbsp;:&nbsp;<a href="https://github.com/timm/tested/blob/main/docs/tbd.md">...</a><br>
Mar28&nbsp;:&nbsp;<a href="https://github.com/timm/tested/blob/main/docs/tbd.md">...</a><br>
Apr4&nbsp;:&nbsp;project review</a><br>
Apr11&nbsp;:&nbsp; <a href="https://github.com/timm/tested/blob/main/docs/tbd.md">...</a><br>
Apr18&nbsp;:&nbsp;no lecture<br>
<dd>
</dl>


<!-- -------------------------------- -->

<td valign=top>
     	Jan19&nbsp;:&nbsp;<a href="https://github.com/timm/tested/blob/main/src/script.lua">hw1</a><br>
     	Jan26&nbsp;:&nbsp;<a href="https://github.com/timm/tested/blob/main/src/data.lua">hw2</a><br>
     	Feb2 &nbsp;:&nbsp;<a href="https://github.com/timm/tested/blob/main/src/cluster.lua">hw3</a><br>
     	Feb9 &nbsp;:&nbsp;<a href="https://github.com/timm/tested/blob/main/docs/onGrid.md">hw4</a><br>
     	Feb16 &nbsp;:&nbsp;<a href="https://github.com/timm/tested/blob/main/docs/onBins.md">hw5</a><br>
     	Mar6 &nbsp;:&nbsp;<a href="https://github.com/timm/tested/blob/main/src/tbd.lua">hw6</a><br>
      Mar8(wed)&nbsp;:&nbsp;mid-term, 4:30</a><br>
     	Mar13 &nbsp;:&nbsp;<a href="https://github.com/timm/tested/blob/main/src/tbd.lua">hw7</a><br>
    	Mar16 (break)</a><br>
    	Apr5&nbsp;:&nbsp;project review</a><br>
    	Apr20&nbsp;:&nbsp;<a href="https://github.com/timm/tested/blob/main/docs/onProject.md">project</a>
        Apr28&nbsp;:&nbsp;exam, 3:30

</td>
</tr>

</table>




## Why?

[mov](https://github.com/timm/tested/raw/main/etc/mov/chaptGPT_lua_kmeans.mov)

> Rahul's first rule: when it is wrong, it so confidently wrong that you cannot tell.

- wrong, on several points
   - security 
   - hard-wired constants that should be adjustable
   - does not support symbolics
   - does not support streaming
   - does not support hierarchy 
   - nothing about connecting clustering to sampling and optimization
   
```
398  {:Acc+ 15.6 :Lbs- 2970.4 :Mpg+ 23.8}
| 199
| | 99
| | | 49
| | | | 24  {:Acc+ 17.3 :Lbs- 2623.5 :Mpg+ 30.4}
| | | | 25  {:Acc+ 16.3 :Lbs- 2693.4 :Mpg+ 29.2}
| | | 50
| | | | 25  {:Acc+ 15.8 :Lbs- 2446.1 :Mpg+ 27.2}
| | | | 25  {:Acc+ 16.7 :Lbs- 2309.2 :Mpg+ 26.0}
| | 100
| | | 50
| | | | 25  {:Acc+ 16.2 :Lbs- 2362.5 :Mpg+ 32.0}
| | | | 25  {:Acc+ 16.4 :Lbs- 2184.1 :Mpg+ 34.8}
| | | 50
| | | | 25  {:Acc+ 16.2 :Lbs- 2185.8 :Mpg+ 29.6} <== best?
| | | | 25  {:Acc+ 16.3 :Lbs- 2179.4 :Mpg+ 26.4}
| 199
| | 99
| | | 49
| | | | 24  {:Acc+ 16.6 :Lbs- 2716.9 :Mpg+ 22.5}
| | | | 25  {:Acc+ 16.1 :Lbs- 3063.5 :Mpg+ 20.4}
| | | 50
| | | | 25  {:Acc+ 17.4 :Lbs- 3104.6 :Mpg+ 21.6}
| | | | 25  {:Acc+ 16.3 :Lbs- 3145.6 :Mpg+ 22.0}
| | 100
| | | 50
| | | | 25  {:Acc+ 12.4 :Lbs- 4320.5 :Mpg+ 12.4}
| | | | 25  {:Acc+ 11.3 :Lbs- 4194.2 :Mpg+ 12.8} <== worst
| | | 50
| | | | 25  {:Acc+ 13.7 :Lbs- 4143.1 :Mpg+ 18.0}
| | | | 25  {:Acc+ 14.4 :Lbs- 3830.2 :Mpg+ 16.4}
```

Now here's nearly the same algorithm, but know we run a greedy search over the splits. When splitting on two distance points  A,B, we peek at the  Y values and ignore the worse half.

```
398  {:Acc+ 15.6 :Lbs- 2970.4 :Mpg+ 23.8}
| 199
| | 100
| | | 50
| | | | 25  {:Acc+ 17.2 :Lbs- 2001.0 :Mpg+ 33.2}
```

- nothing about bias


<img src="https://github.com/timm/tested/blob/main/etc/img/fairness.png?raw=true">


My main problem: cognitive fixation:

"If it was up to current thinking (in the 1920s)  to cure polio. . . You'd have the best iron lung in the world but not a polio vaccine."

![image](https://user-images.githubusercontent.com/29195/211912925-0a9dda23-71d6-4c48-87b0-ebb3bd1eff39.png)

![image](https://user-images.githubusercontent.com/29195/211912983-1cc21e0b-d545-4e08-af3f-bb45d3c21f09.gif)



> Rahul's second rule: you need to know a lot about the code to to make best use of automatically generated code.

This subject:  under the hood of data mining, optimization, theorem proving and all the other tricks of automated software engineering
