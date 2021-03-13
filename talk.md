background-image: url(img/title.png)

---

# Motivation

## This talk is about <support@metacenter.no> and how to use it well

(or replace this email since the points are hopefully valid also for other computing centers)


### Hopefully this is a useful guide
### Hopefully it does not come across as "do this, don't do this"

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

- Person asking for help has perhaps 20 years less experience
- It is not easy to ask for help
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
- The first thing we see is the .emph[email subject]
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
- .emph[New problem? New ticket/email]
- Same problem? Reply to email and keep ticket number


## Give us context

- Username (we can find it out but takes few minutes)
- Explicit paths (`/cluster/home/myself/somepath`)
  better than implicit paths (`~/somepath`)
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

[expand from https://scicomp.aalto.fi/help/]

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
- User doesn't know how to do X, and thinks that Y is a way to solve X
- User doesn't know how to do Y either
- .emph[User asks for help with Y]
- After much interaction it becomes clear that the user really wants help with X,
  and that Y wasn't even a suitable solution for X
]

---

class: center, middle, inverse

# First time on a new machine?

## Please do not start immediately with a 256-core 40-hour calculation.

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

# Requesting software

[here I will write something ...]

[also talk about sudo ...]

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
