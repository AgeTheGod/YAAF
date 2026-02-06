---
title: Importance Of Names 
---

I had many conversations over the years about the importance of giving things meaningful names.

A lot of articles have been written about Nameing Standards and most of the rules are pretty simple...

-   Use descriptive names
- use alphanumeric charactyers only
- avoid abbreviations
- avoid acronyms
- be concise
- avoid repetition

... which are all obvios guidelines (but definitely not "_rules_" as such) that may be loose and woolly but most people should generally understand what's required. 
Occasionally there are some non-obvious technical rules thrown into a naming standard such as...

-   should be less thatn 30 characters long
- names are case insensitive

... that might or might not make sense depending on your background and the lanuguages you're most familiar with.

However these guidelines tell us what we should be aiming for and provide a general indication of what a "_good name_" should look like but crucially do not answer the more fundamental question : **Why do we care so much about what it's called anyway?**

i could get seriously philosophical about this question. There are whole branches of Lingistics that deal specifically with the "**Naming of Things**", e.g. Nomenclature and Onomastics to name but two, and zillions of books about the significance of **Language as a Cultural Tool**.

The Linguists assertion that **Language Drives Culture** may be a bit contentious and certainly many Sociologists would contend that it's really the reverse and **Culture Drives Language** but both generally agree that the expressiveness of a language has a direct correlation to the maturity of a Society or Culture that uses that language.
The expressiveness of a Data or Information Model is a real.ization of this.
It forms the basis fpr an Information Process Culture and he Classes and Attribvutes and RElationships it defines form the vocabulary for what can be discussed and it's through specialization and type hierarchies that we capture the numances of dioffernt kinds of things and catalogue the variations. 
We then give each variation a distinct name so that we can refer back to it later.

In fact a Naming Standard is itself a bit of a misnomer and should really be a "Nouning Standard" (I hust invented that word) because when we create a model of some subject area we're really talking about the grammatical symbols we're going to use to signify some class of thing i.e. the Proper Noun we're going to use to summarie the general characteristics of each distinct Class we want  to discuss and, by implication, the things we do not want to discuss go unnamed.

However this is a good background reading for the discerning Information Arxchirect and useful in a pin-heads debate but a fat load of use in the practical aspects of creating a "Good Data Model".

Over the years I modelled all kinds of disparate subjects areas. I've modelled Road Networks & Street Furniture; Residential Buildings; Customer Contacts; Predicted Booking Demand; Commercial Air Conditioning Systems; Financial Market Instruments & Prices; Comapny Accounts; TV Licencing; Aircraft Configurations; the Taxonomy of the Natural World; Weather Statistics and a whole bunch of other things.

All of them were good models from a texhnical perspective...

-   they all accurately reflected the things of interest in the subject area
- the rules being defined in the model were the rules agreed with the business stakeholders
- there were no obvios logical flaws in what was being dfined
- they were implementable (very, very important)
- and **everything in the model had a good name** (or so I thought) that conformed to whatever naming standard I was working with at the time

Yet some of these models were very successful (if I say so myself) and some were abysmal failures (tomy regret) but, being an arch navel-gazer, I learnt something from all of them and drew conslusions aboput why the successful ones were really "good" and the unsuccessful ones were really "bad" and most of them were somewhere in between.

In pretty much every case I put the success or failure down to the Names of Things described in the model. The successful ones used the "**Right names for the target audience**" and the unsuccessful ones used the wrong names.

The worst case of this I had was BBC TV Licencing when it was contracted out by the BBC to a 3rd party consortium. When I jpined the project the consortium already had a Logical Data Model that they were using for application development and featured all the classic classes seen in many data models e.g. Product, Customer, Address etc.

The problem was that the model had not been signed off by the customer (the BBC) and nobody I talked to from the BBC understood the model or the terms defined in it in any of their spoken or written communbications.

They used terms such as Licence, Responsible Party, Licensable Site because these were the terms used in the actual legislation written by the UK Government and used by the BBC for the previous 50+ years ofg licencing TV's in t he UK.

So I gutted the Logical data Model and pretty much started again using the Class Names and Terms that the BBC themselves used. That was easy and after a onth of intensive discussion they finally signed the :DM off as fit for their purpose.

Now, the knock-on consequences was that there was no correlation between the new LDM and the software that had already been built and, once I created the Database Schema from the LDM, no correlation between the software classes and the database schema tables. Also every specification produced by the Business Analysts in discussion with the BBC had to be translated by the development team into the Classes and Attribute names they had already embedded in their software.

This was a real pain in the nether region and all because the initial model was using the wrong names fropm the primary target audience.

That for me illustrates the practical aspects of giving things a "good name" when developing a data model.

1.  Wherever possible always use the nams that the business stakeholders themselves use to refer to something - if they call it a Licence then don't call it a Product and then argue that all Licences are just a kind of Product anyway.
2. Once you have an agreed model then only refer to something using the agreed terms exactly as stated in the model - the model is the extent of the vocabulary that should be required to discuss all information of interest.
3. Let the model and its vocabulary stand on its own two legs - by all means provide definitions, description and examples but, like a good book, the data model should be consumable by a reader without the author always being present to explain what the opwrds mean to a knowledgeable reader.

If you can't achieve the last one then the model will most likely fail in its purpose.

##  Verbalization

A side-point that's a sure fire test on the usability of any names is teh "verbalization" test so go and talk to someone about the model and hear what it sounds like when spoken out loud in a conversation.

The emphasis on "talking" is inentuonal because "good names" should be easy to use in conversation.

A long time ago one of the books I read on Information Modelling discussed the importance of "verbalization" when developing an Information Model. Quite simply, conversations about something are quite difficult if

1. Something doesn't have a name that can be easily pronounced literally as written  
2. names of two different things in the same domain sound the same
3. the names as spoken are very different to the names as written

So the suggestion in that book was that all verbal conversations abput he information in the model should use the terms **exactly as defined** and then it'll quickly become apparent what those terms should be.

The reasons for this are psychological because...

1. Conversations, especially with very busy people, tend to be short and to the point
2. It takes time to get the words out so people don;t want to use a lot of words when naming something i.e. avoid long compound names
3. Most people think faster than they can talk so it really messes up a train of thought if someone can't get the words out fast enough. (Unless you thoughts naturally meander all over the place like mine do.) 

The verbalization approach to identify or produce "meaningful names" is something I regularly recommend to people for all kinds of reasons and this is just another one.



