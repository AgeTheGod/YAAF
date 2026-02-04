#   The Importance of Names

I had many conversations over the years about the importance of giving things meaningful names.

A lot of articles have been written about Naming Standards and most of the rules are pretty simple...

-   Use descriptive names
- use alphanumeric characters only
- avoid abbreviations
- avoid acronyms
- be concise
- avoid repetition

... which are all obvious guidelines (but definitely not "_rules_" as such) that may be loose and woolly but most people should generally understand what's required. 
Occasionally there are some non-obvious technical rules thrown into a naming standard such as...

-   should be less than 30 characters long
- names are case-insensitive

... that might or might not make sense depending on your background and the languages you're most familiar with.

However, these guidelines tell us what we should be aiming for and provide a general indication of what a "_good name_" should look like but crucially do not answer the more fundamental question : **Why do we care so much about what it's called anyway?**

I could get seriously philosophical about this question. There are whole branches of Linguistics that deal specifically with the "**Naming of Things**", e.g. Nomenclature and Onomastics to name but two, and zillions of books about the significance of **Language as a Cultural Tool**.

The Linguists assertion that **Language Drives Culture** may be a bit contentious and certainly many Sociologists would contend that it's really the reverse and **Culture Drives Language** but both generally agree that the expressiveness of a language has a direct correlation to the maturity of a Society or Culture that uses that language.
The expressiveness of a Data or Information Model is a realization of this.
It forms the basis for an Information Process Culture and the Classes and Attributes and Relationships it defines form the vocabulary for what can be discussed and it's through specialization and type hierarchies that we capture the nuances of different kinds of things and catalogue the variations. 
We then give each variation a distinct name so that we can refer back to it later.

In fact a Naming Standard is itself a bit of a misnomer and should really be a "Nouning Standard" (I just invented that word) because when we create a model of some subject area we're really talking about the grammatical symbols we're going to use to signify some class of thing i.e. the Proper Noun we're going to use to summarie the general characteristics of each distinct Class we want  to discuss and, by implication, the things we do not want to discuss go unnamed.

However this is a good background reading for the discerning Information Architect and useful in a pin-heads debate but a fat load of use in the practical aspects of creating a "Good Data Model".

Over the years I modelled all kinds of disparate subjects areas. 
I've modelled Road Networks & Street Furniture; Residential Buildings; Customer Contacts; Predicted Booking Demand; Commercial Air Conditioning Systems; Financial Market Instruments & Prices; Company Accounts; TV Licencing; Aircraft Configurations; the Taxonomy of the Natural World; Weather Statistics and a whole bunch of other things.

All of them were good models from a technical perspective...

- they all accurately reflected the things of interest in the subject area
- the rules being defined in the model were the rules agreed with the business stakeholders
- there were no obvious logical flaws in what was being defined
- they were implementable (very, very important)
- and **everything in the model had a good name** (or so I thought) that conformed to whatever naming standard I was working with at the time

Yet some of these models were very successful (if I say so myself) and some were abysmal failures (to my regret) but, being an arch navel-gazer, I learnt something from all of them and drew conclusions about why the successful ones were really "good" and the unsuccessful ones were really "bad" and most of them were somewhere in between.

In pretty much every case I put the success or failure down to the Names of Things described in the model. The successful ones used the "**Right names for the target audience**" and the unsuccessful ones used the wrong names.

The worst case of this I had was BBC TV Licencing when it was contracted out by the BBC to a 3rd party consortium. When I joined the project the consortium already had a Logical Data Model that they were using for application development and featured all the classic classes seen in many data models e.g. Product, Customer, Address etc.

The problem was that the model had not been signed off by the customer (the BBC) and nobody I talked to from the BBC understood the model or the terms defined in it in any of their spoken or written communications.

They used terms such as Licence, Responsible Party, Licensable Site because these were the terms used in the actual legislation written by the UK Government and used by the BBC for the previous 50+ years of licencing TV's in the UK.

So I gutted the Logical data Model and pretty much started again using the Class Names and Terms that the BBC themselves used. That was easy and after a month of intensive discussion they finally signed the :DM off as fit for their purpose.

Now, the knock-on consequences was that there was no correlation between the new LDM and the software that had already been built and, once I created the Database Schema from the LDM, no correlation between the software classes and the database schema tables. 
Also every specification produced by the Business Analysts in discussion with the BBC had to be translated by the development team into the Classes and Attribute names they had already embedded in their software.

This was a real pain in the nether region and all because the initial model was using the wrong names from the primary target audience.

That for me illustrates the practical aspects of giving things a "good name" when developing a data model.

1. Wherever possible always use the names that the business stakeholders themselves use to refer to something - if they call it a Licence then don't call it a Product and then argue that all Licences are just a kind of Product anyway.
2. Once you have an agreed model then only refer to something using the agreed terms exactly as stated in the model - the model is the extent of the vocabulary that should be required to discuss all information of interest.
3. Let the model and its vocabulary stand on its own two legs - by all means provide definitions, description and examples but, like a good book, the data model should be consumable by a reader without the author always being present to explain what the words mean to a knowledgeable reader.

If you can't achieve the last one then the model will most likely fail in its purpose.
