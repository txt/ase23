# How to Make Computers Smarter/

<img align = right width=500 src="https://i.pinimg.com/originals/2c/97/b4/2c97b421c756a19468b58546202160e1.jpg">

"Computers are stupid......    
They can only give you answers"       
-- Pablo Picasso[^0] 

Can we make techniogy to help us ask better questions bout the world?

## Answer0: I not here to study philosophy. 

I just want
to learn abut data miners, optimizers, and theorem provers

To which I say:
- Why not both?
- Data miners, optimizers, theorem provers are algoritms.
  Algorithms make choices. Choices have consequences. Don't you know how to control those consequences?
- And you don't reflect on the broader picture, are you actually introducing bugs into your automated software?
- So if you don't reflect on how to use software to makde better choices, are you making worse software [^1].
  For example, shown ehre are the chocies inside a nearest neighbor classifier. Each blue dot is a classifeir confirgured
at random from those space of options. The x-axis show how many classifications were correct. THe y-axis shows the ratio
of false alarms for men and women in this data. If this data was about "who must suffer  weeks of body-destroying chemotherapy?",
which choice would you want?

<img align=center src="/docs/img/nn.pdf" width=800>


Answer1: exploring questions like "what leads to false alarms for women" is not a question for technologisits.  That is someone else's
problem.


Answer2: This is absolutely our problem. Our house is on fire and we need do
something about it

- Automatoc Recidivism models are more likely to 
[falsely label black defendants as future criminals](https://www.propublica.org/article/machine-bias-risk-assessments-in-criminal-sentencing)
 at twice the rate as white defen-
dants.
- Widely-used facial recognition software that predicts char-
acteristics, such as gender and age, has a 
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

Answer3: "We" (i.e. engineers) are the wrong people to solve this.
Technology has alsways been selected to gavour the ruling elite.
ogy and, as such, they are selected to [favor the ruling elite](https://www.google.com/books/edition/America_by_Design/LBYlAV6VmpwC?hl=en&gbpv=0)
In
this view, algorithms are as inherently as bad (racist, sexist, extrem-
ist, misinforming) as anything else selected by their social context.
Hence there is no value in fixing algorithms until we first fix the
society that selects and deploys them [^2]


Answer4: We (engieers) cuased the problem. We are responsible. We need to take action. 

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
decided to speak and act in hateful ways, which caused mental and physical harm to others. 
In one scenario, Haugen said, the company's technology was even used to fan the flames of genocide in Myanmar, literally costing lives.   
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
listes as "decoupling of advertising and commercial interests from
the ability to access high-quality information on the Internet”,
“suspend the circulation of racist and sexist material that is used
to erode our civil and human rights”; and require that all search
results be annotated to symbolize e.g. pornography (in red), business
or commercial material (in green), entertainment (in orange), etc.
