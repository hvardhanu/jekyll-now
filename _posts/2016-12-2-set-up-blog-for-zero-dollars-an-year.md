---
layout: post
title: How to setup a blog for about $0 an year.
---

The power of static content is yet to be harnessed in the world of web development. Dynamic server based systems that have millions of line of code defining business logic solve most of the complicated problems, but they are a very inefficient way of solving simple problems, like serving textual content. 

Why do you need a compute to serve a collection of text, that people just read? What is the role of business logic in this case? The answer is nothing. Churning our copies of text that does not change should be a simple case of serving content from a _HTTP server_. Not a case for an _application server_. As there is no application here. Just a web page, a simple website.

So without the fancy setup, any static content website shoud be served from storage directly. Why not? That is what httpd i.e. apache webserver does. Picks up index.html and serve. So as the setup is simple, the cost should be low as well? Infact the cost should be close to zero. As the cost of the storage capacity that holds the static webpage is essentially very low. In fact zero. Do you know how much 100MB cost? The asnwer is not even worth thinking about.

So if you want to setup a close to zero cost blog, or website you need to ensure that you dont need any crazy business logic. You can create crazy business logic websites, but they will incrementally become more expensive. But I will argue that even crazy business logic websited will not need a compute or an application server. Why? well lets try to unravel this.

Any web site has three major componenents:

* Static content
* Business logic
* Data

Data combined with business logic gets you static content in different configurations. This is often called _dynamic content_. Business logic is often written in recursively encapsulated entities called application servers. That are a set of concentric boxes containing the logic written by some very smart developers. Now what if we think a little out of that box, and put this encapsulated business logic upfront in Javascript? And for data, what if we store and retrieve it from _SaaS_ databases using API calls made in the same Javascript? This API call could be made to a _NoSQL Database_ that is not our problem, i.e. not owned by us, but somebody else's problem. We pay this service provider for his kind services. The same Javascript now pulls the data mixes it with business logic and decides to make calls to appropriate static content and creates views on the browser.

Makes Sense? 

What about security? You may ask. Well if you want security because you are transmitting credit card numbers then I assume you are making some money. If you are making money then why are you reading this blog post? spend some moolah and buy a good CMS. For all other purposes if you need safety and security then get a SSL certificate and use HTTPS. Period.

I think there are plenty of websites which are doing this and reducing costs. You should try doing this too.

I am doing this with this blog, Hosting it on GitHub pages on Jekyll based template. and linking it to my Domain. So the only thing I am paying for is my domain. I write my blog like I used to write code, pulling, upating pushing and I am loving markdown.

It's simple, its so Zen like and biggest of all it's dirt cheap.

Read More about Jekyll here [link](https://jekyllrb.com/)
