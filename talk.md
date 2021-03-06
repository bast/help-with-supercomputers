background-image: url(img/title.png)

---

## About me

.left-column60[
- [CodeRefinery](https://coderefinery.org/)
- Worked in research (theoretical chemistry) in France and Sweden

- Worked in HPC and support in Sweden and Norway

- [Research software engineering](https://nordic-rse.org/)

- Teaching programming

- Helping researchers with computing and programming

- Part of the Sigma2/Metacenter team (Norway)
]
.right-column40[
<img src="img/avatar.jpeg" style="width: 60%;"/>
]

---

# Motivation

## This talk is about writing support requests so that you get quick and useful answers

### Hopefully this is a useful guide
### Hopefully it does not come across as "do this, don't do that"

---

# About this guide

We can solve almost anything for you, but if you don't follow these steps then
.emph[your experience] will be much worse.

We as staff should also create guides for staff and provide training for staff
in how to support users. .emph[A lot of improvement is needed].

---

# Credit

- This talk has borrowed some points from
  "How to Get Help and Ask for Software" (Bjørn-Helge Mevik)
- Richard Darst and [CodeRefinery team](https://coderefinery.org/) for discussions and ideas
- https://documentation.sigma2.no/getting_help/support_line.html
- https://scicomp.aalto.fi/help/
- I have spent some time on both sides (research and support)

.cite[Images from https://deathgenerator.com/ by [@Foone](https://deathgenerator.com/)]

---

class: center, middle, inverse

# Who is on the other side?

## There is a human being on the other side

---

# There is a human being on the other side

## Good to remember for support staff:

- It is not easy to ask for help
- Person asking for help has perhaps 20 years less experience
- The person on the other side has perhaps spent weeks on this problem and waited for days/weeks for your answer
- We always need to .emph[be respectful]


## Good to know:

- Staff is on support duty every few weeks (sometimes 2 or 3 weeks/ year)
- They don't know "everything"
- They may not be spending all their work time on the supercomputer either
- They may not know you
- They may not have context

---

# Ticketing system

.left-column60[
- Typically 10-30 new requests per day
- A new email opens a "ticket"
- Each new ticket gets a new .emph[number]
- Reply to email/ticket is filed under the same number
- .emph[Tickets have owners] but owners can change
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

- Username (we can find it out but takes few minutes)
- Explicit paths (`/cluster/home/myself/somepath`)
  better than implicit paths ("you can find it in my home folder", `~/somepath`)
- Which machine?
- Tell us about your environment
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

- Staff answers what users ask for but do not think deeper about what the user
  really needs

.cite[thanks to Richard Darst for pointing this out]

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

---

# Create a small example for you

- Something that runs in 5 minutes
- Where you know the result and the timing


### Next time you are unsure whether it's the machine or "you"?

- Run the small example
- If it suddenly stopped working or runs slower, you know it's probably the machine
- Now you can send us the example so that we fix the machine

---

# Summary and recommendations

- When facing a problem, spend few minutes on it before writing the email
- But also don't hesitate too long before asking
- You can install most software yourself - we are happy to show you how
- Remember XY problem
- Grow calculations
- Create a small example for you
- Make your problem examples short and reproducible

### These slides: https://bit.ly/help-with-supercomputers
