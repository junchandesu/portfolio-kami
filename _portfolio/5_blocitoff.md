---
layout: post
title: Blocitoff
thumbnail-path: "img/blocitoff.png"
short-description: Build a self-destructing to-do list application.

---

{:.center}
![]({{ site.baseurl }}/img/blocitoff.png)

## Explanation
[Bloccitoff](http://bloccitoff-junko.herokuapp.com/) will aim to keep to-do lists manageable by automatically deleting to-do items that have not been completed after seven days. The hypothesis is that if the to-do item is not important enough to be completed in seven days, it doesn't belong on your to-do list. Here is [Github](https://github.com/junkodesu/bloccitoff "Follow on GitHub")

## User Stories

1.  sign up for a free account by providing a user name, password and email
2.  Sign in and out of Blocitoff
3.  see my profile page
4.  create multiple to-do items
5.  Seed the development database automatically with users and to-do items
6.  mark to-do items as complete and have them deleted
7.  see how old a to-do item is
8.  my to-dos should be automatically deleted seven

## Utilized Tools

*   The Devise gem for authentication
*   Three Models: User, Item, ToDo
*   The Faker gem to generate fake data for users and items
*   Ajax to delete to-do items without reloading the page.
*   distance_of_time_in_words helper method to display the number of days since a certain day
*   custom rake tasks to delete expired to-do items
*   automate the customed delete Rake task to run each day

## Conclusion

This ToDo list is a simple, clean application and I would love to use it. Most of the tools were familiar except for customes rake and cron jobs I created manually. I would need to play around the desgin to make it looks fun to use it.

<script>
  (function(i,s,o,g,r,a,m){i['GoogleAnalyticsObject']=r;i[r]=i[r]||function(){
  (i[r].q=i[r].q||[]).push(arguments)},i[r].l=1*new Date();a=s.createElement(o),
  m=s.getElementsByTagName(o)[0];a.async=1;a.src=g;m.parentNode.insertBefore(a,m)
  })(window,document,'script','//www.google-analytics.com/analytics.js','ga');

  ga('create', 'UA-69982922-1', 'auto');
  ga('send', 'pageview');

</script>