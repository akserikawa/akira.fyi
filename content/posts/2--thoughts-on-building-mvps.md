+++
title = 'Thoughts on building MVPs'
date = 2023-10-11T03:01:00+02:00
draft = false
showtoc = true
+++
>Disclaimer: It's 3:01 AM so I might say some stupid things. Sorry not sorry.

## Introduction
Countless books and blog posts have been written about agile product development and MVPs.
Here are my thoughts after building my fair share of them over the years.

### MVPs? What's that?

Let's start with some definitions:
> A **minimum viable product** (MVP) is a version of a new product that allows a team to collect the maximum amount of validated learning about customers **with the least effort**.

Another one, spot on 🎯
> The MVP is a product with **enough features** to attract early-adopter customers and **validate** a product idea **early** in the product development cycle. In industries such as software, the MVP can help the product team **receive user feedback as quickly as possible** to **iterate** and **improve** the product.

I've highlighted some of the key concepts above, but If I had to reduce these points into one, I would choose the term *speed*.
To me, MVPs are all about shipping fast.

## Speed matters the most
How fast can you ship it? I'm talking from the very first line of code to production.  
I've seen teams spend months on these so called "MVPs"... Heck, even more than a year! That's 11 more months than ideal.
And that's because they forgot what the "M" stands for.

## But... what does "Minimum" even mean?
In software, *minimum* should mean *good enough*. It **does not** mean *perfect*, nor *fully tested*, and it definitely does not mean *scalable*.
If your team (including them managers 🙄) share the same expectations, you will be able to actually ship something in due time (to market) - see what I did there?  
IMHO, one month of full time effort should be enough to build something that *kind of works* and let's you validate your idea.  
Also, MVPs might break easily, and that can be a good thing.  
You spent very little resources on it to validate something and what better proof than having more users than you can handle?

## No more nice-to-have's + What do our users really need?
Having a lot of ideas to make an awesome product is fun. But when you've had your fun for a while, throw them into the pit a.k.a backlog.  
At early stages, focus on what your users really need from your product.  
Do not build nice-to-have's. Don't let them stop you from your goal.  
You will be have plenty of time to build them if the product becomes a success.  
Spoiler: [there's a big chance it won't be that way](https://www.embroker.com/blog/startup-statistics/).  
So always have your main goal in mind and take the easy route whenever possible.

## Identify your domain ASAP
This is a rather hard thing to do at early stages of a product but there's a chance most of the stuff you'll spend time building is better solved by outsourcing it.  
I'm talking landing pages/admin UI templates, notifications/mailing/payments/observability services, all things infrastructure, etc.  
I've seen companies build their own solutions for these to "cut costs"... cringe.  
Don't waste any time on that stuff. Just google existing solutions for your problem and pay for the convenience.  
Once you have a clearer understanding of your business domain, that is, where most of your revenue comes from, you can focus on building something of your own.

## Boring technology > Hype
End users very rarely care about tech.  
Unless you're building a product for other developers, you should not give a single fuck about it and choose the tech stack you're most productive with.  
The one that let's you ship fast and one that ideally makes hiring easy when the team scales.  
In my personal case, it's PHP+Symfony. Many others use Java+Spring or Python+Django... you get the picture.
Stuff that's been battle tested for decades. Boring? Sure.

Would it be cooler if you used a combination of Rust, K8s, serverless functions plus a frontend at the edge or whatever the hyped tech is by the time you read this?  
Who cares... if by the time you manage to learn all that new stuff you've already missed time to market?
Let other devs waste their time criticizing your tech choices while you keep building.

## Don't get too distracted by "best practices" in the industry
Just return HTML > JavaScript.

Pushing to the main branch > whatever gitflow.

Zero CI/CD unless it's managed by your cloud provider.

Some even go as far as "No Git > Git", but that's way too savage for most of us.

## Avoid microservices like the plague
You don't have the time nor the resources to manage a product with microservices. Not even AWS themselves use them, lol.  
Build a monorepo and throw everything in it. Try to separate the concerns when possible but don't worry too much about coupling code because... 👇 

## MVPs should be disposable
Many startups don't get this right. Unless your MVP has great foundations, this means, you just scraped and ducktaped all the puzzle pieces together, throw it in the trash once there's enough revenue. Seriously though, do not keep building new features on it!  
You will be happier and this will save you tons of money years down the line if you don't let that big ball of mud grow.

## Final thoughts
MVP is an overused term.  
Gather feedback from users as early as possible.  
Take Time to market seriously. Especially nowadays with the rise of AI... competition is fiercer than ever.  

See ya on the next one! ☮️