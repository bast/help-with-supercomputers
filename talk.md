class: center, middle

# When and how to ask for help with (super)computers

## Radovan Bast [@\_\_radovan](https://twitter.com/__radovan)

## Slides: https://bit.ly/help-with-supercomputers

UiT The Arctic University of Norway

---

# Outline/topics

- What kinds of help are available for different levels of work

- When to ask for help

- How to write support requests so that you get quick and useful answers

- How to create reproducible examples

- The value of growing calculations and simplifying problems

--

## Goals

- The goal is to .emph[improve our experience] when solving issues.

- We as staff should also create guides for staff and provide training for staff
  in how to support users. .emph[A lot of improvement is needed].

---

# About me

.left-column60[
- [CodeRefinery](https://coderefinery.org/)
- Worked in research (theoretical chemistry) in France and Sweden

- Worked in HPC and support in Sweden and Norway

- [Research software engineering](https://nordic-rse.org/)

- Teaching programming

- Helping researchers with computing and programming

- Part of the [Sigma2/NRIS](https://documentation.sigma2.no/) team (Norway)
]
.right-column40[
<img src="img/avatar.jpeg" style="width: 60%;"/>
]

---

# Credit

- This talk has borrowed some points from
  "How to Get Help and Ask for Software" (B.-H. Mevik)
- R. Darst, E. Glerean, J. Suvilehto, and [CodeRefinery community](https://coderefinery.zulipchat.com/) for discussions and ideas
- https://documentation.sigma2.no/getting_help/support_line.html
- https://scicomp.aalto.fi/help/
- I have spent some time on both sides (research and support)

.cite[Images from https://deathgenerator.com/ by [@Foone](https://deathgenerator.com/)]

---

# Where to ask

- Colleagues
- "Garage"/ Q&A session
- Search engine
- Chat
- Issue tracker (email opens a ticket): problem with a computer or a program you didn't write
- Research software engineers: problem with a code you wrote or want to change
- Mailing list
- Forum
- Stack Exchange


## Different levels of help

- Asking for advice
- Asking to get something done for you: installation, scaling, programming

---

class: center, middle, inverse

# Who is on the other side?

## There is a human being on the other side

---

# There is a human being on the other side

## Good to remember for those answering:

- It is not easy to ask for help
- Person asking for help has perhaps 20 years less experience
- The person on the other side has perhaps spent weeks on this problem and waited for days/weeks for your answer
- We always need to .emph[be respectful]


## Good to know for those asking:

- Staff may be on rotating support duty every few weeks
- They don't know "everything"
- They may not be spending all their work time on the supercomputer either
- They may not know you
- They may not have context

---

# I remember the answer to my first ever technical email request

I wrote a very long email motivating why I would benefit so much from getting access to code X


### Answer:

```
hi,

I guess what you meant asking in-between all those paragraphs was:
"can I please get the code X?"

Yes! Here it is :-)
```

---

# Ticketing system/ issue tracker

.left-column60[
- Typically 10-30 new requests per day
- A new email opens a "ticket"
- Each new ticket gets a new .emph[number]
- Reply to email/ticket is filed under the same number
- .emph[Tickets/issues have owners] but owners can change
- The first thing we see is the .emph[email subject] (or issue thread title)
]
.right-column40[
<img src="img/rtfm.png" alt="comic of somebody calling to get help" style="height: 350px;"/>

.cite[https://xkcd.com/293/, CC-BY-NC]
]

---

.left-column70[
# Subject

- "Problem" is not a useful subject
- "Why is my job crashing?" is better
- .emph[New problem? New ticket/issue/thread/email]
- Same problem? Reply to email/thread and keep ticket number


## Give us context

- Username (we can find it out but takes few minutes of "boring" work)
- Explicit paths (`/cluster/home/myself/somepath`)
  better than implicit paths ("you can find it in my home folder", `~/somepath`)
- Which machine?
- Which software?
- Which research field?
- Tell us about your environment (anything special in your `.bashrc`?)
- Sometimes text better than screenshot
- Sometimes attachment better than screenshot
]
.right-column30[
<img src="img/zelda.png" alt="image saying: I AM ERROR" style="height: 200px;"/>

.cite[https://deathgenerator.com/#zelda2]
]

---

# Formulate your question

- .emph[Has it ever worked?] (If so, what has changed?)

- .emph[What are you trying to accomplish?] Your ultimate goal, not current technical obstacle.

- .emph[What did you do?] Be specific enough to be reproducible - copy and paste exact commands you run, exact output messages, scripts, inputs, etc.

- .emph[What do you need?] Do you need a complete solution, pointers to get started, or should we say if it will take too long and we recommend you think of other solutions first?

.cite[taken from https://scicomp.aalto.fi/help/]

---

# When to ask for help

- Do not hesitate to ask for help and in doubt ask.

- But the helper will appreciate if you spend more than 2 minutes on the problem before asking.


## Those helping:

- Don't forget that the person asking may not know yet how to look for solutions before asking. Help them by showing how.

- Instead of sending a URL to a documentation/solution or checklist, start with
  empathy, work together through checklist, show them what you have tried and
  what you have found.

- Asking checklist questions can make users feel that they are annoying the help desk person.

---

# Tell us what you have tried

- Has it stopped working? Has it ever worked?
- Does it always fail this way? Or only sometimes?
- .emph[Have you tried to isolate/simplify the problem?] How? (more about this later)
- Please check documentation and web
- But sometimes web is "wrong" so don't hesitate to ask

---

.left-column40[
<img src="img/want.jpg" alt="tell me what you want what you really really want" style="height: 200px;"/>
]
.right-column60[
# The XY problem

After http://xyproblem.info/:
- User wants to do X
- User thinks that Y is a way to solve X
- User tries Y and hits a problem
- .emph[User asks for help with Y]
- After much interaction it becomes clear that the user really wants help with X,
  and that Y wasn't even a suitable solution for X

### Ask early when you only know X and haven't tried Y yet
]

---

# "Reverse XY problem"

- Staff answers what users ask for but doesn't go deeper.
- Reason: issues can get closed faster, which appears good.

.cite[thanks to Richard Darst for pointing this out]

---

# Example request

```
hi,

I am user "johndoe" on the cluster Saga [a cluster in Norway]
and since this morning I can't log in anymore.

I have tried to log into Fram and Betzy [other clusters] and this works.

I use ssh keys to log in and the error that I get since this morning is:


    $ ssh saga

    johndoe@saga: Permission denied
                  (publickey,gssapi-keyex,gssapi-with-mic,password,hostbased).


thank you in advance for help/advice on how to solve this,
  John Doe
```

### What do you like about this request?

---

# Another example

```
hi,

I am not sure I wrote to the right support line but what I am looking
for is a virtual machine where we can install a PHP web server with a MySQL database
behind it.

What we have in mind is to set up a service where we can share the data from
our recent study (the data can be fully public). It's about 2000 records so
it's not much data. And we would like to create a web frontend where people
can search through and plot our data.

Looking forward to hearing from you whether this is possible and what you think
about our approach,
  Jane Doe
```

### What do you like about this one?

---

class: center, middle, inverse

# First time on a new machine?

## Please do not start immediately with a 16-node and 40-hour calculation

---

# How to grow your calculation

- Start with a short 5-minute run on 1 core

- Then try more cores on the same node

- Then try going beyond one node

- Then increase the system size and make your calculation longer

### Discuss the advantages of this approach

---

# Create a small reproducible example

.left-column50[
### Job script

- Please make the example fail as early as possible (this requires some work on your side)
- Tell us how long it takes to failure
- Is the failure reproducible or random?
- If it fails after 2 seconds, do not request 48 hours
- .emph[All dependencies loaded in your script]
- Avoid loading dependencies in `.bashrc`
- Attach all necessary files
]
.right-column50[
### Interactive job

- .emph[Provide all commands from login to the problem]
- Please make the example as short as possible
]

---

# Why small example?

- Making the example smaller often simplifies the problem

- This process can help identifying the reason

- Reduce the number of possible reasons

- Shorter example is easier to debug and does not queue "forever"

--

### Next time you are unsure whether it's the machine or "you"?

- Run the small example

- If it suddenly stopped working or runs slower, you know it's probably the machine

- Now you can send us the example so that we fix the machine

---

# You are not alone

- Approach .emph[research software engineers] near you

- Pop into a "garage" or Q & A help session and say hi

- You are probably not alone experiencing this problem

- Your question is not stupid

- Many people really enjoy helping

- It is also OK to write when something *is* working well

### These slides: https://bit.ly/help-with-supercomputers
