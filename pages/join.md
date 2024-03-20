---
title: Joining the Laboratory!
description: Well begun is half done.
background: /assets/images/kaist.jpg
permalink: /join
---

Thank you for your interest in joining our lab! 
This document contains all the information you need, so please read it thoroughly before proceeding.

## Application Procedure

- **Feel free to contact [Jeehoon]({{ site.baseurl }}/jeehoon.kang).** 
  There are no barriers to reaching out to Jeehoon, such as GPA or experience. 
  You can also connect with Jeehoon through [comments](https://www.fearless.systems/#contact)!

- **Create an email account in the format `{firstname}.{lastname}{prefix}@kaist.ac.kr`** (if you're a KAIST student).
    + Ideally, `{prefix}` should be empty. If taken, add a random number, like `{firstname}.{lastname}42@kaist.ac.kr`.
    + Set up a "virtual mail" at <mail.kaist.ac.kr> > Upper right-hand gear > Settings > Mail > Virtual Mail > Add Mail.

- **Complete the [Google Form](https://forms.gle/CX1fqaev1ed5i6ZQ6)**.

- **Schedule a 30-minute Google Meet meeting with Jeehoon.**
  Create a Google Calendar event and invite [jeehoon.kang@cp.kaist.ac.kr](mailto:jeehoon.kang@cp.kaist.ac.kr). 
  Check [Jeehoon's calendar]({{ site.baseurl }}/jeehoon.kang#calendar) for his availability.

- **Email Jeehoon at [jeehoon.kang@kaist.ac.kr](mailto:jeehoon.kang@kaist.ac.kr)**.
  + Use your `{firstname}.{lastname}{prefix}@kaist.ac.kr` email (for KAIST students).
  + Inform Jeehoon that you have submitted the Google Form and scheduled a meeting.

- **Read this entire document** while awaiting a response from Jeehoon.


## Requirements

- **All new graduate students must complete at least two of the following before joining the lab**:
    + Homework from [KAIST CS420: Compiler Design](https://github.com/kaist-cp/cs420). Lectures are on YouTube; questions can be asked in the course repository's issue tracker.
    + Homework from [KAIST CS431: Concurrent Programming](https://github.com/kaist-cp/cs492-concur). Lectures are on YouTube; questions can be asked in the course repository's issue tracker.
    + Exercises from [Software Foundations](https://softwarefoundations.cis.upenn.edu/) Volumes 1 and 2.
    + Studying the [Corundum](https://github.com/corundum/corundum) open-source FPGA-based NIC.

- **Undergraduate interns are highly encouraged to join the lab**.
  Use the internship to experience lab life. 
  Ideally, complete **at least one** of the above tasks before joining. 
  This will allow you to start research projects immediately upon joining.


## General Advice

Welcome to the lab! Here are my insights on research and work in general.

### What is Research?

> "Research is what I am doing when I don't know what I am doing," Wernher von Braun

Research is defined by its tentativeness in every aspect, from motivation to methods, evaluation, and goals. During research, the final outcome is often unknown. This uncertainty leads researchers to frequently encounter:

- **Failures**. Not knowing exactly what you're doing means frequent failures. It's essential to be mentally resilient to handle this frustration. Over time, small successes can accumulate, contributing to papers and eventually a thesis.

- **Changing Plans**. As your understanding evolves, so will your goals. Consider your goal as an ever-moving target; the current version is merely the best approximation of the eventual outcome. Goals should be balanced: not too concrete to be inflexible to changes, yet not too abstract to lack direction.


### Management Principles

Despite the inherent uncertainty in research, our lab aims to minimize tangential uncertainty. Not all uncertainties are productive; for example, confusion about schedules or communication hinders progress. However, exploring uncharted areas is essential in research. We distinguish between these types of uncertainty, aiming to reduce the former while appropriately managing the latter.

To reduce unnecessary uncertainty, we enforce a few communication rules. These rules help prevent misunderstandings. For instance, we have guidelines about nighttime communications in chat applications to avoid potential tension. Our policy is to allow night-time mentions, but responses are only required during working hours. We strive to keep the number of rules minimal to ensure they are easy to follow.


### Communication

#### Asynchronous Communication

- **Prioritize asynchronous communication**: This means the recipient is not obliged to respond immediately. If something can be communicated this way, do so as soon as possible. For example, if you need Jeehoon to review a document, send it to him right after completion instead of waiting for a meeting. Address his feedback promptly and inform him once it's done.

- While defaulting to asynchronous communication, ensure timely responses. Aim to reply to messages within 15 minutes during work hours.

- Before requesting a synchronous meeting (either face-to-face or online), prepare and share a meeting agenda. This agenda should clearly state the meeting's purpose, such as reporting progress, seeking advice, or casual conversation. List all discussion points at the start for better meeting organization.

    + Meetings may be canceled if an agenda is not provided.
    + For discussions involving a document, share it at least 12 hours before the meeting to allow time for review. Share it even if incomplete to enable early feedback.


#### Volume

- **Post brief updates in the [daily log](https://cp-chat.kaist.ac.kr/#narrow/stream/16-daily-log) at 10am and 3pm every day**. These updates should outline your plans and achievements for the day.

- **Arrange a minimum of one 15-minute meeting per week with Jeehoon**. These meetings can cover various topics, including research, coursework, or teaching assistant duties.


#### Discussion

- **Never pretend to understand something when you don't.**
  By doing so, you miss the chance to (1) gain new knowledge; and (2) delve deeper into problems that could lead to significant research topics.
  Embrace your lack of knowledge.
  Remember, it's okay not to know everything; don't worry about others judging you for it.
  + Avoid affirming or denying something if you're uncertain.
  + Be honest if you don't understand something.
  + It's encouraged to admit, "I don't get it" or "I don't know that."

- **Stay true to the essence of the discussion.**
  Express your agreement or disagreement openly; if you like or dislike something, say it.
  However, avoid turning discussions into a battle to win. Research is collaborative, not competitive.
  Start by summarizing your point (e.g., "I think this idea might not work generally") and then provide evidence for your argument (e.g., "For example, consider this code: ...").

- **Keep your cool in heated discussions.**
  Research and creative work thrive on diverse, sometimes conflicting, perspectives, leading to intense discussions.
  However, it's important to keep emotions separate.
  Although challenging, strive to maintain a level head.

- **Summarize and share notes from discussions immediately** in the relevant project stream on Zulip.
  For example:

        ## discussions
        - Method A may fail due to reason B. (Is B relevant?)
        - Let's try Method C first.
        - Also, exploring Method D could be beneficial.

        ## action items
        - Jeehoon: reach out to the authors of Method D.
        - Kyeongmin: assess the significance of B, and document the shortcomings of A in GitLab.
        - Seungmin: start implementing C and plan the next meeting.

  Always provide a balanced summary, even for ideas you disagree with.


#### Reliability

- **Regularly communicate key information to collaborators.**
  Adequate communication is vital for progress in research.
  Your current challenge might already be addressed by others, so keep everyone updated on your work.
  While excessive communication can be a burden, it's usually harmless and can be proactively managed.

- **Respond to feedback and action items without fail.**
  When you receive feedback, either address it or provide a reasoned counterargument.
  If you're unable to complete action items by their deadline, notify your team as soon as possible.
    + This doesn't mean you must always meet deadlines perfectly. Research can be unpredictable, and it's normal to encounter delays. The key is timely communication.
    + Being reliable in this aspect allows others to trust you with responsibilities. Unreliability, such as missing feedback or action items, burdens others with additional tracking and management.


#### Writing and Speaking Skills

- **Strive for clarity and directness in communication.**
  Instead of a sequential explanation like "A leads to B, which leads to C," use a direct approach: "C is the result, due to B, which is caused by A."

- **Learn from Dr. Derek Dreyer's resources on effective communication**:
    + [How to write papers so people can read them](https://people.mpi-sws.org/~dreyer/talks/talk-plmw16.pdf), PLMW@POPL 2016.
    + [How to give talks that people can follow](https://people.mpi-sws.org/~dreyer/talks/talk-plmw18popl.pdf), PLMW@POPL 2018.
    + [How to write papers and give talks that people can follow](https://people.mpi-sws.org/~dreyer/talks/talk-plmw17icfp.pdf), PLMW@ICFP 2017.

- **Apply Derek's CGI model** in summarizing papers or drafting proposals.
  Evaluate the context, gap, innovation, strengths, and weaknesses of papers and proposals.
  For guidance, refer to [this example](https://docs.google.com/document/d/1W8coma11JFp0JIaVqFnZYkEa0sBkgZ1ijTSh6j8c_Gw).


## Tools

For detailed information about our tools, please refer to the [dedicated document]({{ site.baseurl }}{% link pages/tools.md %}).


## Completion

Before joining the lab, double-check that you have completed all the listed action items.
Once you join, notify Jeehoon via a direct message on Zulip.
