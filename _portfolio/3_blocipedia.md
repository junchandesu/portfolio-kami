---
layout: post
title: Blocipedia
thumbnail-path: "img/blocipedia.jpg"
short-description: Blocipedia allows users to create their own wikis and share others by their choices with SaaS

---

{:.center}
![]({{ site.baseurl }}/img/blocipedia.jpg)

## Explanation

[Blocipedia](https://junko-bloc-blocpedia.herokuapp.com/) is a great way to collaborate on community-sourced content. Whether the wiki is for a hobby or work-related project, you will build an app that lets users create their own wikis and share them publicly or privately with own collaborators. 

## Problem

There are Two problems that I have faced on this applications.
Integration of Stripe(Online payment process) into my apps and the collaborater to a specific user for others' private wikis.

## Solution

As the process to implement Stripe gem,
1. Configure the env variable 
2. Charge controller creates Stripe object with the encrypted card info and amount to send and send to the registered key in Stripe.
3. Changes the User status to premium, which allow the users to create either private or public wikis
4. Once a user choces to downgrade to standard user, private wikis turned to public wikis

Deppenging on the user status, authorization is changed and the wiki can be see with the restriction.
Scope class give each user permission to see public wikis ,public & own private wikis, public and own/other permitted private wikis or all by adding specific wiki in an array.

## Accommplishment
* Sign up page with Devise gem
* Three tables : User, Wiki, Collaborater
* Stripe is used for credit card payment process
* Markdown is allowed to Wiki's body attribute
* Collaborater table joins Wiki and User tables to add/delete collaborate for private wikis

## Conclusion

My first time to include the credit card payment system was exciting. It waw very simple one transaction task but it was exciting to see how API can be implemented on my own application.

<script>
  (function(i,s,o,g,r,a,m){i['GoogleAnalyticsObject']=r;i[r]=i[r]||function(){
  (i[r].q=i[r].q||[]).push(arguments)},i[r].l=1*new Date();a=s.createElement(o),
  m=s.getElementsByTagName(o)[0];a.async=1;a.src=g;m.parentNode.insertBefore(a,m)
  })(window,document,'script','//www.google-analytics.com/analytics.js','ga');

  ga('create', 'UA-69982922-1', 'auto');
  ga('send', 'pageview');

</script>