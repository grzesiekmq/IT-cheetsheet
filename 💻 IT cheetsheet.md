# 💻 IT cheetsheet

©️ by grzesiekmq 

[grzesiekmq - Overview](https://github.com/grzesiekmq)

![cat in front of laptop.png](%F0%9F%92%BB%20IT%20cheetsheet%20c0dd2114a0f64f6ebd6ce9b43d54a3eb/cat_in_front_of_laptop.png)

image generated with 

[Craiyon, formerly DALL-E mini](https://www.craiyon.com/)

---

Table of contents

---

# Computer Science

Computer science?
What's that, no it's not fixing computers. It's something more. Computer science is a very broad term, it consists of many fields: artificial intelligence (AI, very popular lately), programming (also popular), computer networks, databases (designing a database is not an easy task), operating systems, web design, information systems, computer graphics and more.
As you can see, you can't be a computer scientist, it would mean that you know it all, and this is unrealistic, the term programmer, graphic designer and other specific positions are more suitable

# Web usability

Web usability refers to the usability of websites and web applications, so a specific application. It mainly focuses on simplifying their use, placing important elements in the right places to ensure intuitiveness, and the aspect of multi-accessibility, the latter of which is related to the ability to use virtually any type of device (desktop computer and mobile device, i.e. smartphone, tablet, etc.), so you can see on the site that there is a transition between two versions, the "primary" version and the mobile version.

## **Nielsen's ten heuristics**

****Associated with the concept of web usability are Nielsen's so-called ten heuristics. Heuristics according to Nielsen are a general rule based on experience, they are not a specific guideline for usability:
1. show the status of the system.
2. maintain compatibility between the system and reality.
3. Give the user full control.
4. Stick to standards and maintain consistency.
5. prevent errors.
6. Allow choice instead of forcing memorization.
7. Provide flexibility and efficiency.
8. Ensure aesthetics and moderation.
9. Provide effective error handling.
10. Take care of support and documentation.

**As for the status of the system**, the user should be given feedback within a reasonably short period of time, i.e. where he is now, what is happening in the system, for example.

**Compatibility** between the system and reality consists in such a mapping of elements of reality to virtual ones that this compatibility is achieved. In addition, this heuristic requires using natural language and avoiding the language of the system.

**Full control** must take into account the fact that a user can mistakenly select the wrong function he wanted (e.g., delete message), but can undo an action fortunately, so confusing operations should be far enough apart to eliminate a possible unwanted action. "Reverse" and "execute again" functions should be introduced.

**Sticking to standards** refers to conventions that help maintain an intuitive user experience.

Maintaining **consistency** applies to links (e.g., a link should be highlighted in blue and underlined), headings (highlighted in such a way that they are bold and larger than the body text, allowing content to be scanned) and forms. Moreover, all subpages must look identical, which is in line with the "stay on the page" principle.

**Preventing** errors, it is better to build a reliable site than to display the best error messages. Implementing an option to confirm the selection before the action is initiated should also be considered.

**Selecting** is better than remembering because it minimizes user memory usage. Using a drop-down list works better than filling in a text box.

**Flexibility** and efficiency are intended to streamline the tasks performed.

Implementing an **advanced** view allows additional features to appear. The website should be adapted for inexperienced (beginners) and experienced (experts) users. The functionality of the most common actions is a good idea.

**Aesthetics** and sanity are other heuristics to consider. Beware of using inappropriate phrases. The length of the message text should not be exaggerated, so use minimalism.

**Displayed** errors must not be represented by error codes, instead they must be written in human-understandable language. Effective error handling means precise wording, indication and resolution of the problem.

**Support** and documentation. The ideal case occurs if documentation (which should not be extensive) is not necessary. However, today's sites, due to their extensiveness, require help and documentation. The selected information for a specific task must be easy to find in a help search engine and should consist of steps to follow.

## Response time

In addition to the ten heuristics, the site's response time is important, theoretically varying between 0.1 seconds and 10 seconds. Above 10 seconds, you should signal that the page may load in a moment and tell the user to wait.

# XML

Extensible Markup Language is a meta-language (a language for creating other languages) containing metadata (data information), easy to implement, interoperable with HTML, elements are defined by the user (that's why it is extensible). Tags consist of elements and attributes. There is only one main element in an XML document, the other elements must occur once or more. Attributes, on the other hand, consist of a name and a value (enclosed in apostrophes or quotation marks). Proper nesting of tags is important. The language is used in electronic data exchange. The document must be syntactically correct (each element must have an opening and closing tag, and the name of the element must be the same in the opening and closing tags), otherwise an error/error message will be displayed and the content will not be displayed in the browser. Comments (they must not be in tags!) can be created using the opening set of symbols "<!--" and the closing "-->". An example of a created comment:

```xml
<!-- This is a comment in XML -->
```

Comments are not processed by the XML processor.
A document type declaration can be created by typing:

```xml
<?xml version="1.0"?>
```

The above document type declaration specifies the XML version used. The declaration must be at the beginning of the document. An example of the opening and closing tag of the car element with its content:

```xml
<car>BMW</car>
```

# banner blindness

It means that users do not pay attention to content that looks like ads, banners, etc. The best solution is to simply abandon them, as they provide no benefit.

# Market Basket Analysis

In a nutshell, Market Basket Analysis involves examining the shopping behavior of consumers.
There are association rules associated with basket analysis.
The following relationship is given:
beer → chips
It follows that a consumer who buys a beer product may simultaneously purchase a second product, which is chips. These products will be bought together because there is a strong relationship between them.

## Characteristics of basket analysis

Basket analysis data is characterized by:

- Very large number of records
- Sparsity
- Heterogeneity

Related to the **first** characteristic is the fact that one million transactions are carried out per day.
**Sparsity** refers to the fact that each shopping cart contains a small number of products.
**Heterogeneity** of data means that customers who have different tastes tend to buy specific products belonging to a certain subset.
 

## indicators

One of the methods of data mining is basket analysis. Association rules are indicators used to measure consumer behavior.
The following indicators are associated with basket analysis:

- support
- confidence

### Support

Support is defined by the **probability** of the product of sets A and B, i.e. the quotient of the number of transactions (a set of products) containing items from sets A and B to the number of all transactions. In other words, it is the percentage of transactions containing data from sets A and B.
support=P(A∩B)=(number of transactions containing A and B)/(number of all transactions)
For example, if a set A such that A={beer}, a set B such that B={chips} and s(A∩B)=s({beer,chips})=90%, where s(A∩B) is the support for products from sets A and B, it follows that a customer will buy beer and chips with a probability of 90%.

### Confidence

Confidence indicates the accuracy of a rule, it is defined as the quotient of the number of transactions (set of products) containing items from sets A and B to the number of transactions containing items from set A.
confidence=P(B│A)=(P(A∩B))/(P(A))= =(number of transactions containing A and B)/( number of transactions containing A)
For example, if the set A={beer},B={chips} and c(B|A)=70%, where c(B|A) is the confidence for the set B provided there is a set A, it follows that among customers buying beer, 70% of them will buy chips.
 

## applications

Basket analysis is not only applicable to the food industry. It can be applied to many other areas:

- medical diagnosis
- protein sequences
- data inventory
- customer relationship management (CRM)
- IT operations analytics
- appropriate library shelf layout
- fraud detection
- online merchandising

### Medical diagnosis

Basket analysis in medical diagnosis is used to help doctors when treating patients. Diagnosis is not an easy process because it produces uncertain test results and makes data from the learning sample noisy. Basket analysis identifies symptoms that occur together. Let I_1 denote one symptom.
T={I_1,...,I_n}
A transaction (denoted by T, a set of elements) in this case is a medical case. When treating a patient, the symptoms are the elements of the transaction (medical case).

### Protein sequences

A lot of research has been done related to proteins. As a result, it is believed that protein sequences are not random. With the help of association analysis, it is possible to identify relationships between amino acids found in proteins. Each protein has a three-dimensional structure. Let I_1 stand for one amino acid.
T={I_(1,)...,I_n}
In this case, the protein is a T-transaction, and the amino acids are the elements of this transaction.

### Census data

The census provides statistical information about the population. Let I_1 denote the indicator collected.
T={I_(1,)...,I_n}
In this case, the statistical area is a transaction T, and the collected indicators are the elements of this transaction.

### Customer relationship management

Customer relationship management is a rich source of data to help look for customer preferences in order to improve the association of customers with relevant products. The use of basket analysis can detect changes in customer behavior based on customer profile and sales data.

### Operations analytics in IT

Basket analysis comes in handy in day-to-day IT operations in detecting significant changes and alerts related to each other.

### Proper arrangement of shelves in the library

The proper arrangement of shelves with categories is important because it allows readers to more easily access a shelf next to another shelf based on a similar category. Basket analysis can be used in looking for links between categories, e.g. if a shelf contains the anthropology category, the shelf next to it should be the shelf containing the Oceania category.

### Fraud detection

Claims fraud can be detected by identifying suspicious links in claims analysis. Let I_1 denote the person being cheated.
T={I_(1,)...,I_n}
In this case, the claim is a transaction T, and the cheated individuals are the elements of this transaction.

### Web merchandising

Merchandising is a marketing technique designed to make people familiar with new or existing products and increase sales through advertising and other activities.
Web merchandising refers to the ways in which products are made available and purchased online. A clickstream is a collection of user sessions when visiting a website. A session is a sequence of pages visited by a user. Let I_1 denote the user's session.
T={I_(1,)...,I_n}
In this case, the collection of sessions, i.e. the stream of clicks, is a transaction T, and the sessions are the elements of this transaction.

In summary, basket analysis is used to check consumer shopping behavior and can be applied in many other areas outside the food industry.

# EDI (electronic data interchange)

Definition: 

> "Transfer of structured data using accepted message standards from computer to another computer using electronic means."
> 

EDI is affecting paper saving (reducing costs), easy flow of documents provides efficiency and in the long run is much cheaper.

# Business Continuity Planning

BCP (business continuity planning) is an important aspect concerning the continuation of operations in the event of natural disasters, erroneous intentional or accidental human activity, and technical failures, BCP is related to conducting IT risk analysis

# ERP

ERP and ERP II information systems (this should be given special attention, enterprise resource planning systems , connecting them to the Internet initiates the supply chain and B2B (Business to Business) and B2C (Business to Customer) strategy, and transforms from ERP to ERP II having a CRM solution (see post on CRM), thanks to the World Wide Web in the case of ERP II, external stakeholders can "join" the organization, ie. customers and suppliers, in general, investing involves risk, especially in IT, when the financial result is satisfactory has a positive value, but this is not a 100% probability, because the risk of investment is inherently unpredictable, you do not know whether a particular investment will bring a profit or will fail, as a result, the possible bankruptcy of the company, other aspects are the limitation of redundancy meaning a single way of entering data into the system and the multi-modularity of the systems, they have a significant impact on the formation of efficiency, because in the first case everything is well organized, while in the second it is divided into specific modules: Cash Bank (a module related to information on cash flow, financial status, revenues, costs, receivables, liabilities, the ability to generate financial statements), Invoices (issuance of a receipt, sales invoices, purchase invoices, pro forma, advance, RR, internal sales and purchase, corrective), Trade (contains identically what the Invoices module, additional capabilities are warehouse management), Retail (retail sales), CRM (customer relationship management, i.e. adding contacts containing customer data, scheduling meetings and tasks in progress and completed, customer service procedures, automatic invoice generation, support of company e-mail boxes, commercial offers), Document Flow (collection of electronic documents and their grouping), Service (for companies providing various services), Tax Ledger (bookkeeping to settle with the tax authorities), Commercial Ledger (full accounting in the company, chart of accounts), Fixed Assets (record of fixed assets, depreciation plan), Accounting Office (simplification of tasks for accounting offices), Human Resources and Payroll (human resources and payroll in the company, minimization of making mistakes, thanks to automation of processes), BI Analysis (advanced performance of Business Intelligence analysis allowing to support decision-making processes of the company and to compare data, in order to save time, i.e. work more efficiently),

Manager's Dashboard (managers have 24-hour access from anywhere to various types of reports, analysis, such as ABC, XYZ and others); in addition, the purpose of these systems is to provide a competitive advantage, better organization and relevant information, going further these systems through the power of the Internet allow two-way communication of business with the customer, are user-friendly, affect the reduction of the cost of their administration, access to information is facilitated, does not require frequent technical assistance, which reduces the time of implementation of processes (such as. ordering of selected products), the systems also support the organization in achieving high standards of customer fit, implementing them requires a pre-planned, well-taken decision to invest in ERP as a factor of success and future efficiency),

# CRM

Customer Relationship Management (CRM systems), business applications designed to facilitate the task of acquiring and building customer loyalty, it can also be understood as a strategy to develop, retain and obtain maximum value from the customer, hence more customers generate greater financial benefits, which affects the ability to purchase additional hardware and software, to improve efficiency; CRM also indirectly serves to hire new employees and conduct training.

# Feature Driven Development

FDD (Feature Driven Development) - is a feature-driven development, a combination of project management and software development, the main goal is the business process of delivering a complete and importantly working product in each iteration, important is the continuous cooperation with the user and quality management aspect, FDD contains small units called features or in IT terminology functionalities, the issue here is that features can be implemented in a larger system, but the condition is that they must be tested, moreover, correct. In addition, when there are a lot of features they are classified into a set of features (from feature sets), there is a later process of integration of these sets, resulting in a finished solution, in this case a computer program. It has a disadvantage, it is difficult to control the scope of work of a single employee of the project team. The methodology is similar to the previously mentioned Scrum, which also ensures the generation of positive business value for the organization.

# Agile

In this type of approach, distinctive features such as:
small size of project teams
competent members
creation of innovation
extensive documentation is not required
no communication problems
no hierarchy
direct communication
flexibility
cost-effectiveness
versatility
adaptation to a dynamic environment
ensuring competitive advantage

creativity of the team
self-organization
minimization of risk???

As you can see, the features are very many, and it's even almost ideal for us, because they are the advantages themselves, I'm not saying that there are no disadvantages, I focused on presenting the idea itself, rather than presenting the advantages and barriers. Hidden among the advantages were the benefits of the approach used.

One more thing, what are the types of Agile methodologies?

Agile (soft) methodologies:
Scrum
DSDM
FDD
XP (from eXtreme Programming)
AUP
Crystal
Lean Development

# Scrum

Scrum is a project management methodology widely used around the world in agile software development, but not only, it works well in general as a tool for any project work, it ensures the identification and prioritization of the work required, there is a so-called sprint, which is an iteration of two to four weeks, in other words, a course associated with the phased development of a product, there are two stages: the sprint planning meeting, and at the end a sprint review, to assess the progress of the work and continuous improvement.  In addition, the Scrum methodology involves people on the team in daily morning meetings.  The key roles found in this type of project tool are:
The Product Owner, a person with specific business needs, responsible for the requirements), the Scrum Master (aka Master, facilitates the team's work, reducing obstacles) and the Scrum Team, which is the team charged with executing the project in each iteration of the run.

# Kendo UI

![Untitled](%F0%9F%92%BB%20IT%20cheetsheet%20c0dd2114a0f64f6ebd6ce9b43d54a3eb/Untitled.png)

Kendo UI, a library for creating user interface, for example, unlike Bootstrap, we can use OData. Kendo UI can be integrated with jQuery, AngularJS, Angular, React, Vue.
It includes various components, a simple one such as button, also an advanced one, that is grid (grid), very cool I liked it. Bootstrap is based on CSS, JS also a little, in Kendo UI there is something more, you can write object-oriented, thus the code is clean, as I said you can use OData, there will also be built-in animations. I recommend it, I put it on frontendigest, my Facebook fanpage, for a reason. Interestingly, I had not heard of this library before

Explanation Bootstrap is a CSS framework, and Kendo UI is a library for UI

# VR, AR, Mixed Reality

VR, virtual reality, AR, augmented reality and still mixed reality.
That is, virtual, such as on a quasi, augmented, for example, on a smartphone in addition to the real image we have added, for example, dinosaurs, such an effect when we turn on the camera so-called AR effect, and mixed is a mixing of VR with AR.

# Custom ROM

Custom ROM, or custom ROM, is such a software / operating system, more of a mobile overlay, which has a custom skin, but not only that, everything has custom, you can customize the battery performance, well increase the mAh it can't, in general you can set it as you want, that is, personalize it. What's the deal with that? ROMs can be flash (uploaded), ported, that is, from device to device.
Examples of Custom ROMs:

CyanogenMod,
Amzen,
AOKP,
MIUI (the one I loaded on my Goclever, had everything in Chinese).

Custom ROMs are best uploaded after warranty

# Sublime Text 3

![Untitled](%F0%9F%92%BB%20IT%20cheetsheet%20c0dd2114a0f64f6ebd6ce9b43d54a3eb/Untitled%201.png)

Sublime Text 3
An advanced text editor, unfortunately paid, it has cool features, such as, I guess that's what you can call it, line babeling, multi-line marking and other bits and pieces.
What's cool about this editor?
Package Control, that is, you can install plugins, code beautifiers, linters, formatters. But still, there are default things in VS Code that you don't have in Sublime, such as a built-in debugger

# Packt pub - free learning

![Untitled](%F0%9F%92%BB%20IT%20cheetsheet%20c0dd2114a0f64f6ebd6ce9b43d54a3eb/Untitled%202.png)

Free learning, or daily free IT ebook from Packtpub
We log in, if not we create an account on Packtpub and keep track of free e-books every day, but after some time they repeat like tazos with pokemons :), or stickers from the World Cup
All the time this "free learning" is not there you have to track because there are some periods, after some time there are no free books, and then there are, and I guess it is better to have legally than to pay even with €30 :O
I, for example, already have 100+ of these ebooks, not paying is as beneficial as possible :)

# Why did I start a Twitter account?

![Untitled](%F0%9F%92%BB%20IT%20cheetsheet%20c0dd2114a0f64f6ebd6ce9b43d54a3eb/Untitled%203.png)

I started Twitter to:
observe interesting people from the frontend, backend, follow technological trends (CSS Grid, GraphQL, Static Site Generators, and more, there really is a lot of it)
Join, by the way, the #100DaysOfCode, i.e. coding at least 1 hour a day, challenge succeeded :)
Well, and now it looks like to also join the #100daysofblogging challenge
As I've noticed whether it's Facebook or Twitter, social media in general allows you to explore new things, not just contacts, etc., unlike in Google when you want to search for something you already have to know the keyword, well if you don't know, how do you search? Therefore, with the help comes exploration or there discovery, so if someone says that you waste time on Facebook or Twitter, they may be wrong
That is to say, most importantly, social media is not necessarily a waste of time, sometimes it is an investment when you follow the news whether frontend or backend or devops, IT in general

# Cordova CLI

![Untitled](%F0%9F%92%BB%20IT%20cheetsheet%20c0dd2114a0f64f6ebd6ce9b43d54a3eb/Untitled%204.png)

First of all, I did not write that it is Apache Cordova. What is this Cordova?
It is such a platform for building just hybrid mobile applications, about these I wrote a little on the 

**hybrid mobile apps** below.

 Okay then, once we know what Cordova is we move on. Now what the mysterious acronym CLI is all about. That's from Command Line Interface, or command line interface. What does it give you? The ability to create a project in such a way that we already have a starter, cool no :) ?
Commands in cmd start with cordova well and unfortunately you have to repeat it cordova, but the up-down arrows on the keyboard come in handy. You will find commands such as build, run, create, platform add, emulate (preceded by cordova of course)
But for cordova to work you need to install it via npm, the node.js package manager
This is done by the command 

`npm i -g cordova`

Once we have that, you still need to install node.js, so once we have that the commands are already working then now a bit about the commands
build is used to build the application
`cordova build`
run, we can run the application on the device
`cordova run <platform name>
cordova run android`
create, which means we create a project
`cordova create <pathname>
cordova create MyApp`
platform add, we add the platform (Android, iOS)
`cordova platform add android`
emulate, run on the emulator, well here you need to have Android Studio add the target, that is, what version of Android a little fun
`cordova emulate android`
So yes we use create, platform add, build, and then emulate / run
That's it in a nutshell. As if someone gave up, I recommend PhoneGap Build instead of Cordova
I still recommend after the build, that is, once we have the .apk, to use the BlueStacks emulator

# hybrid mobile apps

Have you wondered why you play with Java, Swift to write a simple application, just use HTML, CSS, JavaScript and you have it done.
Only, the problem is that hybrid applications are inefficient, for example, as if you wanted to make a game such as Tomb raider, but in a mobile version, well, you would already have to write a so-called native application, but as it is to have a business application completely hybrid applications can handle it.
And what are hybrid mobile applications?
Mobile applications are known, and hybrid applications are like a mule, that is, a cross between a donkey and a horse, suppose the donkey is web (internet) applications, (of course I am not criticizing, I am giving as an example), and the horse is native applications.
So hybrid applications are the future, maybe because they only require web technologies.
Interestingly there are few job offers of hybrid application programmer, that's it :)

# Artificial intelligence - cookies from Google

![Untitled](%F0%9F%92%BB%20IT%20cheetsheet%20c0dd2114a0f64f6ebd6ce9b43d54a3eb/Untitled%205.png)

![Untitled](%F0%9F%92%BB%20IT%20cheetsheet%20c0dd2114a0f64f6ebd6ce9b43d54a3eb/Untitled%206.png)

Artificial intelligence bakes cookies :o ?

Well, it may not be out yet, but the idea is interesting, what exactly is going on, Google taught AI for 2 months to bake cookies, and as it is in machine learning, at first it did not work, with the next attempt it was better, but still not in terms of taste, only shape, and the situation is that the cookies are not yet what they are supposed to be, that is tasty, but what is to be expected. What you can conclude from this is that it's the idea that counts, for example, when creating an app, you need to focus on the idea, and only later, how it should work, refine, above all plan, a good plan is the key to success. You just need to look for inspiration, look at what application of the app does not yet exist

  

# Additional

😓 uff as you see this only scratches the surface.
Here are some ideas/concepts which you can write about:

TypeScript

PWA

Why MOOCs have power

Linux Mint

Visual Studio Code

yarn

Static Site Generators

Aurelia

GitLab

code review

clean code

design patterns

best practices

JIRA

TopShelf

MEAN

NativeScript

Electron

D3.js

Blockchain

LAMP stack

AWS

IoT

Big data

Cloud computing

code playground

Postman

GraphQL

CSS Grid

Spring

Covalent

WebSockets

WebAssembly

three.js

Onsen UI

Ionic

PubNub

Cylon.js

Cycle.js

RxJS

LaTeX

Machine learning

Data warehouses

real time databases

OData

WebGL

Lazy loading

MiUI

LineageOS

Eclipse IDE

IDE

OOP

SOLID

DRY

TDD vs BDD 

Lean

Unity

TensorFlow

Flow

Code obfuscation

CORS

Performance

Testing

Jasmine

Karma

Mocha

Chai

#100DaysOfCode

Sinatra

Rails

FP

NLP

SVM

Deep learning

Chat bots

AI

data mining

Material design

XSS

OAuth 2.0

2FA

RabbitMQ

Doctrine

ORM vs ODM

Headless browsers

Markdown

RWD

AJAX vs PJAX

Server-side rendering

DOM

Shadow DOM

Virtual DOM

SPA

JSON

RSS

Sass

ES6

npm

DevTools

HTTP

SQLite

MariaDB

Cassandra

Bitbucket

Spaghetti vs Ravioli vs Lasagne code

WatchDog

BlueStacks

StackOverflow

Sololearn

Enki

ROS

Raspberry Pi

BitCoin

Deep web

Web scraping

SquareSpace

GUI

Computer vision

Code golf

Reverse engineering

R

React Native

RPA

B2B

E-commerce

E-business

UX

PenTesting

Docker

CI

CD

Jenkins

Travis CI

VSTS

TFS

Kotlin

Kali Linux

Phalcon

.NET

Salesforce

BI

Recommendation systems

Software engineering

Automatic image recognition

Virtualization

Ansible

Flask

Scala

PowerShell

vim

pip

yum

nuget

WireShark

Metasploit

Xamarin

Hadoop

MapReduce

Kubernetes

Babel

Lua

Moment.js

Mongoose

nginx

Redis

SVG

YAML

Twig

webpack

Internet archive

composer

Hungarian notation

NetBeans

Codeblocks

Assembly

COBIT

ITIL

waterfall model

FileZilla

Winscp

command line

terminal

GIS

Firebase

Canvas

WebStorage

NoSQL

Regular expressions

Android Studio

RxJava

Dagger

Maven

Grunt

Gulp

Reactive programming

Service Workers

.

.

.

and of course more don’t know how many, but this is **not infinitely** many (there must be some finite set of concepts)

**Thanks for reading**

And one more **note**:

 you reading this for your **own** responsibility.

This text is not verified, but I’m not ChatGPT, so I can’t pretend to be very experienced researcher as is the case with ChatGPT, 
so you can also write about ChatGPT, Transformers, GPT, language model, etc.

Keep learning and good luck 🍀

and don’t forget to star this repo on github:

IT-cheetsheet

[https://github.com/grzesiekmq/IT-cheetsheet](https://github.com/grzesiekmq/IT-cheetsheet)