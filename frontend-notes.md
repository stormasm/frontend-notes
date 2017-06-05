Front End Notes
---------------

These are my notes about front end projects I have worked on.  

# Introduction

I started
out designing front ends written in Java that ran both on the desktop and
in the browser using
[applets](https://en.wikipedia.org/wiki/Java_applet).

I have been developing front ends using Javascript since 2005.  
I was an early user of
[Jquery](https://jquery.com/) which was released a year later in 2006.
When
Node.js came out in 2009 that is when things picked up for me.  And
the first Javascript framework I used in earnest was
[Backbone.js](http://backbonejs.org/)

In the past I worked with
[Marionette](https://marionettejs.com/), the Backbone Framework,
and the simple application I developed can be found in my
[Github repo](https://github.com/stormabq/jobs).

[Here is a demo of the application](http://stormabq.github.io/jobs/)

I also worked for a software company in Buenos Aires, Argentina where I worked on front end development for a Spanish Language learning site.  While living in Los Angeles I worked at Caltech as a researcher in the Biology department where we developed
[CRdata](https://github.com/seerdata/crdata),
a Ruby on Rails front end to back end AWS jobs that ran Stem Cell Experiments.  The first version of the software which I also wrote was developed in Python using
[Django](https://www.djangoproject.com/).  At the time, we were using
[Protovis](http://mbostock.github.io/protovis/)
for our graphs and visualization, the precursor to
[Mike Bostock's popular Framework D3](https://d3js.org/).  

When D3 was released in February of 2011 I was living in Argentina but continued developing with D3 for various UI projects I was working on at the time.  Since that time I have also done extensive work with D3, but its been about 4 years am I am not currently up to speed again on D3.  Instead, the
[Dgraph team](https://dgraph.io/)
is using
[Vis.js](http://visjs.org/)
to do all of their rendering of the nodes and edges of the data returned from the Graphql query.

# Current Ideas

The front end project I am working on now, which is still in development has to do with saving off visualizations of subgraphs that are returned from a larger dgraph query.  Imagine a fairly large graph of data that gets returned when you query for one node and all of its children in a large dataset.  What you want to be able to do is save off sections of the graph for visualization and analysis reasons.  For now, the dgraph team only returns the whole graph, and then to visualize the subgraph you have to send in another query.  But I am working on the ability to click on one of the nodes in the subgraph and then just see that data and save it off as its own json datastructure.

# Angular

I did some development work in
[Angular.js](https://angular.io/)
after finishing up several projects in Backbone.js.  Once I started using Angular I no longer worked with the Backbone.js framework.  I felt that Angular took me to the next level, and gave me the tools I needed to further develop the concept of a Single Page Application.  But with it came the complexity.  The beauty of Backbone.js was its simplicity, small code base and the ability to wrap your head around the concept at hand.  You could even study the Backbone.js code base and fairly quickly come up to speed on how it works.  Angular is highly complex, with lots of moving parts, and understanding intimately how Angular works could take weeks of work.  Whereas Backbone.js could be understood in days.

Then two things happened to derail Angular from its rockstar status.

1. Version 2 was written in Typescript
2. React started to get traction

At the time of this writing React has over 68,000 stars on Github and Angular has 56,000 stars.  Granted a new repo was created for Angular 2 and that repo has more than 24,000 stars.   

# React

When
[React](https://facebook.github.io/react/)
was originally released in 2013 I was spending most of my time developing backend API systems, and when I was doing front end development I was happily using Angular.  But in the past year, when a project came up to do work on the front end I decided to try out react.  I can't say that I am blown away by React, but I am happily using it and the ecosystem is clearly solid.  The thing I do like about React is the simplicity of it.  Because it only deals with the View part of the UI, there are clearly not as many moving parts as Angular.  The downside is that, the view code is embedded inside the Javascript's file **render** method, and that to me is not perfect.  But for now, I am happily developing using React, and coming back up to speed on all of the CSS that needs to be used to make the UI look correct.  But I will admit that I am **NOT** a fancy UI designer and the UIs I design are very simple.  So having an excellent designer on board for me to work with is clearly important for sophisticated web applications.


# Graphql

For the past number of years I have been designing and building large scale API systems that use REST api endpoints.  Tools like Swagger are helpful for managing and automatically documenting the actual REST schemas that can then be generated for the different language implementations.

Recently, Facebook introduced the concept of
[Graphql](http://graphql.org/)
which is now starting to gain some traction.  It "changes the game" so to speak in how we think about and build out APIs to back end services.  Now instead of designing many different endpoints for different types of data, we are able to incorporate our complete data model into one schema that we can then query against very similar to an SQL query.  We now have a defined Query Language that uses JSON requests to get at the data which is then returned in JSON as well.

# Relay
