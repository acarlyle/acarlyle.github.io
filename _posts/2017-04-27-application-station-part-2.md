---
layout: post
date: '2017-04-27 21:03 -0400'
author: Alec
published: true
categories: UMW
excerpt: ''
meta: ''
---
## Human Computer Interaction 

It's been a few weeks since we've taken on the task of building the College of Education Application Station, but there was a problem.  We had no interface.    


### Usability Study

In order to remedy this problem, each member on our team conducted an [independent usability study]({{ site.url }}/documents/Usabilitystudy_alec.pdf).  The project required an intuitive dashboard to navigate, so I choose to focus my study on the admin dashboard.  An admin needed some sort of method to view and export all of the submitted applications.  How does one go about designing this to be intuitive?

### The Prototype



![usstudy.png]({{site.baseurl}}/img/usstudy.png)

I choose to go with a minimalist approach.  Thankfully, I recieved some helpful comments on my prototype from my focus group.  Their collective suggestions included:

* Deleting and Exporting forms should be on separate tabs
* Selecting individual lines is confusing
* It's unclear what the tabs mean


### The Finalized Software

In order to address this feedback, I added a home page to the admin dash to clarify what each tab means:



![adminhome.png]({{site.baseurl}}/img/adminhome.png)



And here is the final version of the Export Application interface:



![exportdash.png]({{site.baseurl}}/assets/exportdash.png)



If I had to create this interface again, I would create the table using Bootstrap checkboxes.  It's apparent to everyone that you can check a checkbox; it may not be clear that you can click on an individual row of the table.


### Up Next

A rundown of the finalized College of Education Application Station.
