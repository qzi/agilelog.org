---
title: "Reading XP 3C: Card Conversation Confirmation"
date: 2022-03-20T20:57:41+08:00
url: /agile/reading-xp-3c-card-conversation-confirmation/
categories:
- agile
summary: 学习scrum 3C时发现来源XP 3C, 在Rachel Davies的《Agile Coaching》书里面也有提到，看到这篇文章其实很短，所以想来慢慢划重点方便以后我重读
---

Origin from: https://ronjeffries.com/xprog/articles/expcardconversationconfirmation/

学习 Scrum 3C 时发现来源于 XP 3C, 在Rachel Davies的《Agile Coaching》书里面也有提到 Ron Jeffries 的 3C ，看到这篇文章其实很短好读点，所以想来慢慢划重点方便以后我重读

3c Card Conversation Confirmation 

The XP Circle of Life helps keep projects alive. A key aspect of this cycle is the Acceptance Test. Acceptance Tests are critical to communication among team members, especially between customer and programmer.

In *Extreme Programming Installed*, we describe the four elements of the XP “Circle of Life”: the on-site customer, working with the programmers, uses the planning game to select user stories to make up the most valuable small releases. Critical to this cycle are the user stories.

User stories have three critical aspects. We can call these Card, Conversation, and Confirmation.



## Card

User stories are written on cards. <u>The card does not contain all the information that makes up the requirement. Instead, the card has just enough text to identify the requirement, and to remind everyone what the story is.</u> The card is a token representing the requirement. It’s used in planning. <u>Notes are written on it, reflecting priority and cost</u>. It’s often handed to the programmers when the story is scheduled to be implemented, and given back to the customer when the story is complete.

这段是我体会比较深，就是有关Story AC 和 Specification 之间还是有区别，一个完整的Story并不体现需求的全部信息, 这回应了有些人对于Story究竟该写多细的问题

## Conversation

The requirement itself is <u>communicated from</u> customer to programmers <u>through conversation</u>: an *exchange* of thoughts, opinions, and feelings. This conversation takes place over time, particularly when the story is estimated (usually during release planning), and again at the iteration planning meeting when the story is scheduled for implementation. <u>The conversation is largely verbal（口头，非书面）, but can be supplemented with documents.</u> The best supplements are examples; <u>the best examples are executable</u>, We call these examples confirmation.

这段提到 Story 本身并不是一个需求闭环，它是一个识别并诱发澄清需求的非书面语媒介，所以细化需求单靠 Story 本身是不够的，可以委之于补充材料，但是最好的补充材料是Working Sofeware。

## Confirmation

No matter how much discussion or how much documentation we produce, we can’t be as certain as we need to be about what is to be done. The third C in the user story’s key aspects adds confirmation that we sorely need. This component is the acceptance test.

At the beginning of the iteration, <u>the customer communicates to</u> the programmers what she wants, by telling them how she will confirm that they’ve done what is needed. <u>She defines the acceptance tests</u> that will be used to show that the story has been implemented correctly.

<u>Teams who are not yet very experienced with these ideas often want to try use cases, spreadsheets showing calculations, sketches of proposed window layouts, even multi-page documents looking much like conventional specifications.</u> These may be useful in rare cases, but looking back over the years I have almost never found this kind of document to be ideal. Even for quite complex situations, confirmation using examples, preferably automated, works better. You may find some paper or computerized details to be valuable, but in my experience, they are more likely to slow you down. I’d suggest starting with card, conversation, confirmation, and adding in other documents only if they are clearly needed.

The programmers implement the story, and they also implement the acceptance tests. Some teams build tools that let the customer enter the tests herself, and other teams have QA people or testers who help with the job. But one one way or another, the acceptance tests get done.

At the end of the iteration, when the story is done, the programmers show the customer that the story is done, confirming success by showing that the acceptance tests run correctly.

The confirmation provided by the acceptance test is what makes possible the simple approach of card and conversation. When the conversation about a card gets down to the details of the acceptance test, the customer and programmer settle the final details of what needs to be done. When the iteration ends and the programmers demonstrate the acceptance tests running, the customer learns that the team can, and will, deliver what’s needed. The confirmation, in terms of acceptance tests, is what keeps the Circle of Life turning. And the Circle of Life … that’s what keeps your project alive.



Copyright Notice of my own part only in this page are licensed under [BY-NC-ND](https://creativecommons.org/licenses/by-nc-nd/4.0/deed.en) except the part of Ron Jeffries
