Title: The Inception of PeerLibrary
Date: 2013-09-17 04:20
Category: assignment
Tags: peerlibrary, open access
Slug: tchen-assign1
Author: Tony Chen
Summary: The story behind building the PeerLibrary project

October 2012
------------
It was Connor's 20th birthday and there was a low key absinthe gathering at his apartment. At the time, I recently withdrew from classes at UC Berkeley for an indeterminate amount of time to start a data infrastructure company in San Francisco. This was when I first met Rodrigo, Spencer and Nicolai - new friends of Connor whom he met at the Berkeley Student Co-op Casa Zimbabwe. Rodrigo and Spencer were hacking on an open source collaborative multitracking recording app for Android devices called Radiotape. Nicolai was taking a course on music and cognition and was thrilled about his plans for his final project. Our interests immediately aligned and we talked about the latent potential for open source technology to shape society. We made plans to collaborate in the near future.

December 2012
-------------
I reconnected with Mek, a former co-worker. We met at a hipster-infested coffeehouse in SoMA to catch up on our latest projects. Mek was working on [Waltz](https://github.com/mekarpeles/waltz), a python application framework for "designing web apps in 3/4 the time" based on the minimalist web.py stack. This conversation was pivotal in helping me realize the power of the open source development and the self-enhancing nature of the collaboration model. I relocated to Vancouver for a month to take some time off from my daily duties at my startup to reevaluate how I can contribute to this open source world. I got exposed to development communities of peer-to-peer tools such as cryptocurrencies (Bitcoin, Namecoin) and encryption software (PGP, Tor). Naturally, I was drawn to the underlying theories behind each new technological discovery and spent my hiatus reading academic literature on said topics. I remember jumping through many hurdles to obtain an economics paper because I no longer had JSTOR access as a non-student. It dawned on me that the academic publishing model was broken and access to scientific research and scholarly literature is a problem I took for granted. I made a commitment to dedicate my new few months (or years!) to respond to this problem.
 
January 2013
------------
I return to Berkeley with a few ideas I wanted to implement and met with Rodrigo and Connor along with Rishi Sharma, an eccentric electrical engineer with a flair for signals processing. Rodrigo was finalizing his codebase for Radiotape and Rishi was writing software for his EEG. That night also coincided with the news of the death of Aaron Swartz which sparked a pertinent conversation on open access both as a political and software movement. We decided to draft an "Open Access Manifesto" and eventually disseminate it across all major research institutions.

There was another low key absinthe gathering at Casa Zimbabwe, this time for Rodrigo's birthday. That night, Rodrigo and I discussed the potential for building version control software for academic and public policy documents. I was recently inspired by Germany's decision to host their [legislative documentation](https://github.com/bundestag/gesetze) on Github and thought this could extend to public research and democratic deliberations. It turned out that Rodrigo and I independently formulated these ideas in the past and have already started their nascent implementations. This was how [PeerLibrary](http://github.com/peerlibrary) was born. Over the following days we attended a symposium held by Lawrence Lessig and later a talk by Daniel Ellsberg which solidified our views on transparency, open access and decentralizing information.

We immediately started coding a prototype for PeerLibrary and indexing millions of open access articles. At the time, the main contributors were Nihil (a talented cryptoanarchist bit pusher with a panache for axiomatic set theory), Rodrigo and I. In the same week, we took our conversation about PeerLibrary to the Internet Archive. Mek introduced us to folks who work there and we demo'd our ambitious idea of the future of scholarly collaboration to Brewster Kahle and his colleagues as well as some friends from Noisebridge. The meeting was a success and convinced us to continue building and expanding PeerLibrary's funtionality.

February 2013
-------------
Concurrently, Rodrigo, Connor, Rishi and I were feeling a little mischievous and started writing data extraction scripts to compile *.edu email addresses from the public directories of major research universities and institutions. Our targets included: Harvard, MIT, CalTech, Stanford, UC Berkeley, UCSF, Yale, Princeton, Columbia, UCLA, National Institutes of Health and NASA. Our intention was to disseminate a document of which its contents called for the liberation of research literature to the public. This was actually pretty fun (we ran into some problems when scraping Harvard Medical School because the email addresses were encoded as jpegs so we ran OCR to extract the text from the images) and was quite a distraction from our development of PeerLibrary.

This was also the month that the [Open Access Initiative](http://oa.berkeley.edu) was founded. At the time the members consisted of the contributors of PeerLibrary and our immediate group of friends. We had plans to get the attention of the Academic senate to get a system wide open access policy passed.

March 2013
----------
Running into some obstacles in building a scalable search engine for millions of article titles, Rodrigo and I decided to reach out to the community for some help. Mek who had experience in building infrastructure for search engines was consulted. At the time the PeerLibrary prototype was an Express node.js application on top of a Redis document store. At around that time, Rodrigo also was in communication with Mitar, a CS PhD student originally from Slovenia who was working on software tools for collaborative decision making. He was also working on an annotation engine for Mozilla's pdf.js, a pdf viewer in javascript. He wrote some interesting code that detected blocks of paragraphs in a pdf document for annotation. As most of the articles we were dealing with were in pdf format, we felt Mitar had the answer to a pressing technical problem Rodrigo and I had for a while. At that moment, Mitar joined the PeerLibrary team and became one of the most active contributor to date.

April 2013
----------
From my south side Berkeley apartment, Rodrigo and I launched a campaign calling for Berkeley and fellow institutions to adopt open access policies. The email addresses we scraped in early February were delivered an urgent message with a link to a petition on the Open Access Initiative website. Within a day we gathered thousands of signatures from students and prominent faculty members. Now we got their attention, we made plans to hold a public forum on the future of open access scholarship on campus.

PeerLibrary was going radical changes at the time. Mitar pushed for a complete rewrite of the codebase from node.js to Meteor - a web framework built on top of node.js for developing real-time, reactive web apps. At first I was apprehensive about the switch given that Meteor was still in its infancy compared to other more documented and active frameworks, however I came to realize the full advantages of Meteor as a software stack for rapid prototyping and development. Concerned about how many real-time concurrent connections would scale, Mitar also became a contributor to Meteor and began porting many useful node packages that were being used in PeerLibrary and deployed them on Meteor.

May 2013
--------
The Open Access Initiative held their inaugural public forum featuring panelists Michael Eisen (Prof. of Biology and Founder of the Public Library of Science), Molly Van Howeling (Prof. of Law, former President of Creative Commons). The take away from this meeting was that open access policy is neither sufficient nor necessary for open access scholarship. The real issues we should be focusing on is how we can build platforms that facilitate a culture where research literature and materials are shared.

June 2013
---------
Two thirds of the PeerLibrary of development team went on a walkabout in Brazil. No code was committed during this period.

July 2013
---------
After a month hiatus, I met with Mitar at a hackathon at the Meteor headquarters. PeerLibrary has gone through some backend changes when I was gone and I had a lot to catch up. in 24 hours, the PeerLibrary search engine was completely rewritten to support real-time instant search queries. The user interface also went through some radical changes. We demo'd PeerLibrary at the end of the hackathon and our project won in the "most impact" category. We scheduled a dinner with Matt deBergalis (founder of Meteor) to talk about the future of PeerLibrary and the Meteor framework.

Present (September 2013)
------------------------
Currently PeerLibrary is active and growing. At the time of writing, it is being presented at the [Open Knowledge Conference](http://okcon.org/2013/09/12/okcon-2013-guest-post-peerlibrary-open-scientific-knowledge/) held in Geneva. 


added Comments Thomas 11/6/2013 (see commit description)
