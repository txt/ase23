  <a name=top><br>
  <p align=center>&nbsp;<a href="/README.md#top">home</a> ::
  <a href="/docs/syllabus.md#top">syllabus</a> ::
  <a href="https://drive.google.com/drive/folders/1ZFn6H8-4kx5uP34bpFgIFonkz9Tw3nYM?usp=sharing">groups</a> ::
  <a href="">chat</a>  ::
  <a href="/LICENSE.md#top">&copy;&nbsp;2023</a> <a href="http://menzies.us">Tim Menzies</a><br>
  <a href="/README.md#top"><img width=600  
     src="/etc/img/ase23.png"></a></p>
  






# How to Make Software More Useful?


<img align = right width=500 src="https://i.pinimg.com/originals/2c/97/b4/2c97b421c756a19468b58546202160e1.jpg">


"Computers are useless ...   
... They can only give you answers."     
- Pablo Picasso[^0] 


How can we reply to Picasso ? How can we assure him that we do not just blindly use software?
But instead we are using it to look at the world from  multiple perspectives, then build
models that are nuances combinations of many points of view?


Well, software engendering is often about build tools that some community can use.
How to other disciplines use their tools?


Astronomy builds tools. E.g.
Astronomers learn how to (e.g.) make lenses.
   But once that is done,
then they those lens to peer out into the universe around us.


So now that SE can build tools, perhaps
our next
challenge is to use software as a lens to explore the world around us:


- with least effort
- yielding most insight.


But how?
How can we design technology to help us ask better questions about the world?


<img align=right src="/docs/img/simon.jpg" width=400>


Now, better [design](design) a means  better exploration of more options.
[Herbert Simon'96](https://monoskop.org/images/9/9c/Simon_Herbert_A_The_Sciences_of_the_Artificial_3rd_ed.pdf) tells us:


> "It is true that humanity is faced with many problems. It always has
been but perhaps not always with such keen awareness of them as we have today.
We might be more optimistic if we recognized that we do not have to solve all of
these problems. Our essential task (a big enough one to be sure) is 
simply to _keep open the options for the future_ or 
perhaps even to **broaden them** a bit by creating
new variety and new niches."


Simon is adamant about the implications of our choices:


> "Our grandchildren cannot ask more of us than that
we offer to them the same chance for adventure, for the pursuit of new and
interesting designs, that we have had."


Returning to Picasso, as witnessed by his own self-portraits (shown top-right), his methods matured dramatically over this lifetime.
Picasso felt that we do not see an
object from one angle or perspective, but rather from many angles
selected by sight and movement. As a result of this belief, his cubist style [^0]
became about _how_ to see an object or figure rather than _what_ the
artist was looking at.


<img align=right width=150 src="https://artofquotation.files.wordpress.com/2019/05/b5b5518c-606c-4eb0-aa2b-090d6dcf5ac0.jpeg?w=816">


Similarly, I'm suggesting here that we should change automated software engineering such that it reflects more
on _how_ it builds models.
Not just just build things and change things. Susan Sontag once said 


> "The only interesting answers are those that destroy the questions."


But also for reviewing more options along the way. If that  seems a little vague to you,
then I'll repeat using the language of high-church SE theory. Don't worry if you the following paragraph makes no sense
to you. By the time I'm done with you, you will be surprosed at just how easy is the following.


I advocate for metamorphic testing of requirements models,
informed by theorem proving, multi-objective optimization, and data mining (specifically, semi-supervised learning).
In that seaerch, XXX basi. also, extensio tests. what is missing. repoteroty grids
The computational complexity of this search will be reduced by a cycle of depth-bound stochastic fuzzing and keys (small variabes that control
the rest).


<br clear=all>


## Answer0: Who Cares? I'm  not here to study philosophy. 


> "I'm a software engineering. All I care abut is bracket matching.
Tell me a few tricks about
data miners, optimizers, and theorem provers
which  I can add to my resume."


To which I say: Why not both?


- Data miners, optimizers, theorem provers are algorithms.
- Algorithms make choices. Choices have consequences. Don't you know how to control those consequences?
- If you don't reflect on how to use software to make better choices, are you making worse software [^1].


For example, here are the choices (and consequences of those choices) inside a nearest neighbor classifier. Suppose this
classifier 
is about "who gets selected for  months of body-destroying chemotherapy and its associated nausea and wretchedness?".
Which choice would you want? And if we just optimized for accuracy, would we find that choice?


- Each blue dot is a classifier configured
at [random](random) from those space of options. 
- The x-axis show how many classifications were correct. 
- The y-axis shows the ratio
of false alarms for men and women in this data. 


<img align=center src="/docs/img/nn.png" width=800>


## Answer1: Who Cares? This is not my problem


Exploring questions like "what leads to false alarms for women" is not a question for engineers.  That is someone else's
problem.


- Maybe not. [Nobel'77(xxxx


## Answer2: Time to act! The house is on fire!


This is absolutely everybody's  problem. All hands on deck. 
There is some bad sh*t going down.


- Automatic recidivism models are more likely to 
[falsely label black defendants as future criminals](https://www.propublica.org/article/machine-bias-risk-assessments-in-criminal-sentencing)
 at twice the rate as white defendants.
- Widely-used facial recognition software that predicts characteristics, such as gender and age, has a 
[much higher error rate for dark-skinned women compared to light-skinned
men](https://news.mit.edu/2018/study-finds-gender-skin-type-bias-artificial-intelligence-systems-0212)
- Amazon’s ML software to offer same-day delivery to prime
users became [biased against black neighborhoods](https://www.businessinsider.com/how-algorithms-can-be-racist-2016-4)
- Google Translate, the most popular translation engine in
the world, [shows gender bias](https://www.science.org/doi/10.1126/science.aal4230). 
“She is an engineer, He is a
nurse” is translated into Turkish and then again into English
becomes “He is an engineer, She is a nurse” [27].
- For more examples, see 
[Kugler'22](https://cacm.acm.org/magazines/2022/4/259390-technologys-impact-on-morality/fulltext) or
[Rudin,'19](https://arxiv.org/pdf/1811.10154.pdf) or
[Gebru'19](https://arxiv.org/pdf/1908.06165.pdf) or
[Nobel'18](https://www.biblio.com/9781479837243).


## Answer3: "We" (i.e. engineers) can never solve this


Wrong to confuse social problems with technical problems.


According to [Noble'77](https://www.google.com/books/edition/America_by_Design/LBYlAV6VmpwC?hl=en&gbpv=0),
t'was ever so.
Technology has always been selected to favor the ruling elite.
ogy and, as such, they are selected to 
In
this view, algorithms are as inherently as bad (racist, sexist, extremist, misinforming) as anything else selected by their social context.
Hence there is no value in fixing algorithms until we first fix the
society that selects and deploys them [^2]


<img align=left width=150 src="/docs/img/otherhand.jpeg">


We (engineers) caused the problem. We are responsible. We need to take action. 


<br clear=all>


> "Technical decisions end up shaping the choices we make about how to present ourselves, 
which in turn shapes how we view ourselves and other people."...   
"Social media platforms can serve us content that enrages or
depresses us, making it more (or less) likely we will take immoral
actions based on our feelings. These platforms also can be used by
[bad actors to take immoral actions more easily](https://youtu.be/9gzo-1jK-TA?t=2)."    
"The same functionality that allows moral choices also enables immoral ones, as 
Facebook whistle- blower Francis Haugen told the U.S. Congress. Haugen testified in 
October 2021 that Facebook knowingly served content containing hate speech and misinformation 
to its users, since that increased engagement. Some of the users receiving that content then 
decided [to](to) speak and act in hateful ways, which caused mental and physical harm to others. 
In one scenario, Haugen said, the company's technology was even used to fan the flames of genocide in Myanmar, 
literally costing lives."   
-- [Kugler'22](https://cacm.acm.org/magazines/2022/4/259390-technologys-impact-on-morality/fulltext),


[Guzmin'22](https://www.biblio.com/book/i-never-thought-way-how-have/d/1461892240)


[Davis'22](https://www.nytimes.com/2022/03/07/books/review/i-never-thought-of-it-that-way-monica-guzman.html)


[Kolker'22](https://www.nytimes.com/2022/03/08/books/review/sandy-hook-elizabeth-williamson.html)


[Ekins'20[(https://www.cato.org/survey-reports/poll-62-americans-say-they-have-political-views-theyre-afraid-share)


Answer6: the question is pointless, there is nothing I can do anyway.  To which I say 


- you never know less you give it a go
- there is no choice. [Kate Starbird demands that we must](https://www.youtube.com/watch?v=9gzo-1jK-TA&t=3218s)


“If there’s one question I want to persuade you to ask more often, it’s ‘What am I missing?’”


[^0]: From [MFA
Masterworks](https://news.masterworksfineart.com/2018/10/31/pablo-picasso-and-cubism#:~:text=In%20collaboration%20with%20his%20friend,how%20he%20achieved%20this%20goal.):
"Pablo Picasso pioneered the Cubism movement, a revolutionary style
of modern art that Picasso formed in response to the rapidly changing
modern world.   Picasso wanted to emphasize the difference between
a painting and reality.Cubism involves different ways of seeing,
or perceiving, the world around us. He felt that we do not see an
object from one angle or perspective, but rather from many angles
selected by sight and movement. As a result of this belief, Cubism
became about _how_ to see an object or figure rather than _what_ the
artist was looking at."


[^1]: Just as ["All lives can't matter until black lives
matter"](https://www.youtube.com/watch?v=Pu2LOSGbNpg), so to will
all  designs miss important matters until we learn "how to find
what matters."


[^2]: And such social-level fixes are going to need a  lot of work
from a lot of people.  e.g. [on page 179 of
Nobel'18](https://www.biblio.com/9781479837243). such fixes are
listed as "decoupling of advertising and commercial interests from
the ability to access high-quality information on the Internet”,
“suspend the circulation of racist and sexist material that is used
to erode our civil and human rights”; and require that all search
results be annotated to symbolize e.g. pornography (in red), business
or commercial material (in green), entertainment (in orange), etc.


