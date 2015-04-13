title: "Node.js, AWM, CODEHERO and the Open Source Madness"
date: 2014-12-18 07:37:02
tags:
- node.js
- codehero
---

The last time I wrote something here I was in the middle of my thesis to obtain my bachelor&rsquo;s degree in computer science AND planning my wedding with the most special person I know. Now that I&rsquo;m graduated and married I have some time to tell what I&rsquo;ve being doing all this time (not related to my principal job, that&rsquo;s mostly Salesforce stuff).

<!-- more -->

My good friend and thesis partner [Oscar](https://twitter.com/oscarvgg), convinced me to learn Node.js, the trendy Javascript framework, to code our thesis project, which was based on a total of 4 interconnected systems. In the end we made 3 of them on Node.js (2 cloud applications hosted on Heroku and 1 local server inside a Raspberry Pi) and 1 iOS application. 

After finishing our great work I was not done with Node.js just yet, I wanted more, something to contribute to the open source community, something useful that people could use, something I would use. Enter [Alfred](http://www.alfredapp.com/), one of my most used apps, the customizable and extensible handyman for the Mac that becomes super powerful by installing workflows made public by benevolent developers around the world. But how good is a tool if all the contributions that make it so wonderful are scattered across the web? That&rsquo;s when my software OCD started to kick in and I started to imagine how great it would be if all workflows were versioned and located in a centralized repository just the way [Homebrew](http://brew.sh/) and [npm](https://www.npmjs.org/) works.

Then I discovered [Packal by Shawn Rice](http://www.packal.org/), the answer to my Alfred prayers, a centralized and searchable place where developers could publish their work in a versioned fashion so all Alfred related workflows could have a home together. There were still 2 issues that concerned me:

1\. As for open source obvious reasons, only authors of the workflows could add their own work to the Packal repository. This means many great workflows are still out there laying on an unknown Github repository or on the 11th page of Alfred forums waiting for someone to find them the hard way.  

2\. Workflow management process is still manual except for updating it. Such a wonderful solution needs a CLI to interact with, imagine npm with just npmjs.org.

That&rsquo;s when I decided to work on a Node.js CLI program to interact with Packal so it behaves the way I always imagined. Then [AWM](https://github.com/jonathanwiesel/awm) was born, lots of progress was made on this tool to support the most common use cases, yet there&rsquo;s still work to do and sadly I have little time to spend on it right now. As of now, 2 important features (install and upgrade) need serious improvement so the tool becomes what I&rsquo;ve being dreaming, if someone wish to help finish it that would be awesome, if not, I hope I find some time to finish it and hopefully people would find it useful. 

It always bothered me that a CLI tool such as this would need a fundamental dependency to work such as Node.js, it should be a binary, that&rsquo;s when I started to think on learning Go before starting this adventure. However, my Node.js hunger was too big, and I just kept going with it.

I&rsquo;m still Node.js hungry, even after all the discussion between developers and Joyent that caused a forking of the Node.js project giving birth to [io.js](https://github.com/iojs/io.js), I hope to make some great commits that make people happy sometime soon, either on AWM or any other great open source product that deserves to be shared with the community.

For those worried about [CODEHERO](http://codehero.co/), I&rsquo;m sorry to say that is abandoned right now. It was a really fun project, I loved showing people to do the thing a find cool, we even [migrated the whole site from Wordpress to Jekyll](https://github.com/codeheroco/codehero-static) to have a faster, prettier and much more reliable website but we never deployed it. In the end it was really time consuming and the revenue was not what we were expecting from our work, the little revenue we earned couldn&rsquo;t be collected since the checks never arrived to Venezuela so the site was mainly maintained from our pockets and the readers&rsquo; donations, on top of that our jobs, thesis and other commitments stacked up so one by one we decided to stop posting and the site fell to abandonment. The site&rsquo;s still online and the existing knowledge is there, so feel free stop by in times of need, although some things may have changed for some courses, like many changes from Express 3 to 4 for example. <span>I must say that I often felt a deep feeling of satisfaction for the simple fact of people entering the site and being thankful for the content we shared.</span>

To all open source backers and developers out there I congratulate you and admire you, the things you do, from the smallest fix or &ldquo;+1&rdquo; on an issue, to the greatest first stable release, that is what makes a good software, contribution and collaboration. 
