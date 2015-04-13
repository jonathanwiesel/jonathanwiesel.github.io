title: "Mule ESB / Mulesoft express deployment as Tomcat service"
date: 2012-09-14 23:57:00
tags:
- work
---

Last month in the office we where trying to deploy our Mule application as a service to Tomcat in a server. We tried several tutorials out there involving wrapping it in a web application, .WAR files and a lot of stuff that didn&rsquo;t work quite well for us.

<!-- more -->

We managed to deploy a Mule application in a express and simple way that it was almost too easy to be true:

- Download [Mule standalone](http://www.mulesoft.org/download-mule-esb-community-edition "Mule").

- Unpack it in the server&rsquo;s location of your desire. 

- Place your zipped Mule application in the /mule-standalone/apps directory.

- If you have any kind of JDBC connector .jar, place it in the /mule-standalone/lib/mule directory.

Now you&rsquo;re ready to run your application, go to  /mule-standalone/bin and you can do
./mule

And stopping it using Crtl-C.

Or you can manipulate it as a daemon using instead
mule start/stop/restart

You&rsquo;re done.

You now have your Mule application running in a standalone instance of Mule ESB that uses its own Tomcat instance. You won&rsquo;t need to install or customize a Tomcat server because Mule standalone will get one up for you.

BTW this installation method* was a product of experimentation and a lot of trial and error, and it could not entirely work for you, so please feel free to tell your opinions and/or experience.

*(courtesy of Ricardo Sampayo, great programmer, you can contact him through his twitter [@ricardo_ven](http://twitter.com/ricardo_ven "Ricardo S")). 
