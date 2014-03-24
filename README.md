act_styleguide
==============

Many Greenpeace offices are now (March 2014) starting to use Engaging Networks, and so a new webpage template was made for them to use for landing pages and conversion/thanks pages on act.greenpeace.org: "Plain Responsive Page Template (https/http)".

## Design limitations

Engaging Networks campaign pages are made in a few steps, one of which is a drag-and-drop design step to put key page elements in place like form fields, the campaign story, photos or video players and a call-to-action headline. It's important that you use two columns on both the landing page and thanks/conversion page, and that on the left column there is only one design element ("Story - Tiger Manifesto" in the example below). 

![2-column design for Greenpeace Tiger Manifesto page](http://i.imgur.com/xS7gqBV.png)

## Demo

[Greenpeace Tiger Manifesto](https://act.greenpeace.org/ea-action/action?ea.client.id=1844&ea.campaign.id=26367)

![Golden Rectangle over Tiger Manifesto page](http://i.imgur.com/EYioAoX.png)

### Golden rectangle
If you can keep the Call To Action to just a title and four lines max, you should find that the web form begins right in that Golden Rectangle sweet spot.

### Footer
The page footer includes a mission statement and copyright notice on the left, and a row of website links on the right, with lots of (fresh green) white space all around.

![Mission statement](http://i.imgur.com/eUyJdft.png)

## Based on a standard CSS boilerplate

The page design is based on [Skelton CSS boilerplate](http://getskeleton.com/). The [layout.css file](https://act.greenpeace.org/ea-campaign/action.retrievefile.do?ea_fileid=38501) is the only one you should need to edit. The CSS classes beginning with ".ea" are required to style the Engaging Networks form elements. Everything above and below the ```<div class="container">...</div>``` can be edited in the html. Engaging Networks fills in what's inside that DIV, so if you want to edit it, you'd better get out your javascript.

## The grid should keep things balanced-looking

### 16 column, 960px horizontal grid: 
Skeleton provides a great 960px grid, made of 16 columns. You'll notice in the layout.css file that the Engaging Networks classes .eaLeftColumnContent and .eaRightColumnContent have column widths of 520px and 400px on standard desktop screens, then 420px and then 300px as the viewport gets narrower. Those widths correspond to the standard ".nine" and ".seven" columns in Skeleton.

### 5px vertical grid: 
All elements should have a height which is a multiple of 5px (like line-height 20px, or margin 5px, but not padding 8px). The only exception to this for now is the main image in the on the left (.eaLeftColumnContent img), which to keep it responsive with the page design and not lose the image's aspect ratio, has a variable height and width=100%. If anyone can sort this gracefully with javascript, it would be much appreciated! :-)

## Pages come with jQuery 1.7.1
Please take note that Engaging Networks will include jQuery 1.7.1 for their form validation scripts and things like that, so you don't need to include it again. Also, it's good to stick to jQuery (or plain vanilla javascript), and not include any other javascript frameworks.


