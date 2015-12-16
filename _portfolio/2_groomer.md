---
layout: post
title: Groomer 
thumbnail-path: "img/groomer.jpg"
short-description: Groomer is the online reservation application. Junko's very first own project.
---

{:.center}
![]({{ site.baseurl }}/img/groomer.jpg)

## Explanation

[Groomer](https://fuji-pet-salon.herokuapp.com/) not only introduces Fuji Pet Salon but also includes the reservation system for the customer online at [http://otakudaisuki.com](http://otakudaisuki.com). Junko's very first application of her own choice. Here is [Github](https://github.com/junkodesu/groomer "Follow on GitHub")


## Problem

This is a free project I have worked with my own idea. There is no set instruction how to follow building a project step by step. I had to start from the brainstorm to publish with my own idea pretty much. 

## Solution

-With Bloc and mentor's suggested design tools for wiresframes(via  balsamiq),  database design(via google drawings), brainstorming(via exmind), I was able to come out from blank idea to organized planning stage at least.
-For the front end design, I have found the downloadable html/css/javascript/boostrap template for a simple web-site that took care of the index page to 
-As I started to build the app, I have realized that I needed to add some table to join two tables due to the necessity of the multiple dog ids for each appointment based on the current clinet's need for groomer business.
-Fullcalendar, drag-n-drop jQuery plugin, was included successfully to choose the available appointment date based on the availabliity and business days by clicking the white colored date but it was not shown only on Safari browser. Inspect Element spotted the code break and the issue was solved.


## Accomplishment
I struggled with the procedures that I have never done but I have self-taught but I have done following!

* Four tables with each association rule
* Fullcalender gem
* Google Map gem for rails
* Registered domains and push the app to web hosting server to publish
* Precompile the app on production environment
* Action Mailer is set to send the confirmation email through Sengrid



## Conclusion

I am more confidence to build a new application from the scratch by planning to publish it on line. I can not wait to get involved in the next project.

<script>
  (function(i,s,o,g,r,a,m){i['GoogleAnalyticsObject']=r;i[r]=i[r]||function(){
  (i[r].q=i[r].q||[]).push(arguments)},i[r].l=1*new Date();a=s.createElement(o),
  m=s.getElementsByTagName(o)[0];a.async=1;a.src=g;m.parentNode.insertBefore(a,m)
  })(window,document,'script','//www.google-analytics.com/analytics.js','ga');

  ga('create', 'UA-69982922-1', 'auto');
  ga('send', 'pageview');

</script>