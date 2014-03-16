act_styleguide
==============

Many Greenpeace offices are now (March 2014) starting to use Engaging Networks, and so a new webpage template was made for them to use for landing pages and conversion/thanks pages on act.greenpeace.org: "Plain Responsive Page Template (https/http)".

## Demo

[Greenpeace Tiger Manifesto](https://act.greenpeace.org/ea-action/action?ea.client.id=1844&ea.campaign.id=26367)




## Based on a standard CSS boilerplate

The page design is based on [Skelton CSS boilerplate](http://getskeleton.com/). The [layout.css file](https://act.greenpeace.org/ea-campaign/action.retrievefile.do?ea_fileid=38501) is the only one you should need to edit. The CSS classes beginning with ".ea" are required to style the Engaging Networks form elements. Everything above and below the "<div class="container">...</div>" can be edited in the html. Engaging Networks fills in what's inside that DIV, so if you want to edit it, you'd better get out your javascript.

### The grid should keep things balanced-looking

Horizontal grid: Skeleton provides a great 960px grid, made of twelve columns. You'll notice in the layout.css file that the Engaging Networks classes .eaLeftColumnContent and .eaRightColumnContent have column widths of 520px and 400px on standard desktop screens, then 420px and then 300px as the viewport gets narrower. Those widths correspond to the standard ".nine" and ".seven" columns in Skeleton.

Vertical grid: All elements should have a height which is a multiple of 5px (like line-height 20px, or margin 5px, but not padding 8px). The only exception to this for now is the main image in the on the left (.eaLeftColumnContent img), which to keep it responsive with the page design and not lose the image's aspect ratio, has a variable height and width=100%. If anyone can sort this gracefully with javascript, it would be much appreciated! :-)




