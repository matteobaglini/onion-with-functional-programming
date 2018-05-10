## Onion Architecture
with 
## Pure Functional Programming 
sauce

---
### Who am I?
- developer since 2001
- technical trainer/coach
- wannabe entrepreneur
![doubleloop](assets/doubleloop.png)

+++
## Big thanks to
![FP BO](assets/fp-bo.png)

+++
## Big thanks to
![Avanscoperta](assets/avanscoperta.jpeg)

---
## Talk target?
Combine the benefits of two good ideas:
- Pure functional programming
- Onion architecture

---
## The lab rat

The birthday greetings kata by Matteo Vaccari
http://matteo.vaccari.name/blog/archives/154

Code:
https://github.com/xpmatteo/birthday-greetings-kata

+++
## Scala edition

https://github.com/matteobaglini/birthday-greetings-kata-scala

+++
## Kata Purpose

To **learn** about the ~~hexagonal~~ onion architecture, which is a good way to **structure an application**, and how to shield your domain model from external apis and systems.

+++
## Problem (1/3)

Write a program that:
1. Loads a set of employee records from a flat file
2. Sends a greetings email to all employees whose birthday is today

+++
## Problem (2/3)

The flat file is a sequence of records, separated by newlines.
```
last_name, first_name, date_of_birth, email
Doe, John, 1982/10/08, john.doe@foobar.com
Ann, Mary, 1975/09/11, mary.ann@foobar.com
```

+++
## Problem (3/3)

The greetings email contains the following text.
```
Subject: Happy birthday!

Happy birthday, dear John!
```
with the first name of the employee substituted for `John`.

+++
## Ingredients

This kata can be done in two ways:
1. Hard way: **refactor the code** one tiny step at time until the code is *clean*. 
2. Simple way: implements the logic **from scratch**.

we pick the hard way, because refactoring is funny! :-)

+++
## let's add pure functional programming to the game!

+++
## Hard and FP way

**refactor the code** one tiny step at time until the code is *clean* and *pure*. 

+++
## Let's see the beast

+++?code=https://raw.githubusercontent.com/matteobaglini/birthday-greetings-kata-scala/94fd4db04fdaa8e8d705500241e1fe5eb2c3568b/src/main/scala/it/kata/birthday_greetings/BirthdayService.scala&lang=Scala
