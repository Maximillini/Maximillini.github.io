---
layout: post
title:  "Assume the Position"
date:   2015-09-25 14:37:44
categories: update
---
<img src="{{ site.baseurl }}/images/css.jpg">
Ah, CSS and positioning. Brace yourselves.

So today we're talking about the position property in CSS; what they are and what they do. As someone who presumably is unfamiliar with the concepts of positioning, my condolences, because they can be an exercise in frustration.

There are four values to choose from with the position property, and each one does something considerably different. But to understand what each one does, it's necessary to briefly explain how CSS works. When you create a CSS stylesheet to apply to an HTML document, it basically considers most elements of your document to be a 'block.' These blocks (usually text), without any added markup, will simply sit on top of one another. What's crucial to understand however, is that each of these block elements affects the position of the rest. If you have 3 block elements in a column of text (say 3 divs for instance), and the middle div is removed, the page will collapse and the bottom-most block will move upward to meet the top-most block. With that in mind, we can now understand how position affects where these blocks end up.

Static is the simplest to understand and achieve. By default, static positioning is automatically applied, and as stated above, will cause block elements to sit on top of one another as normal. In fact, because it's the default value for all HTML documents, you won't have to type a single character to apply static positioning. Thanks HTML! The only problem is that this is probably going to get boring pretty quick. We can fix that though.

Relative is an interesting position value, because it allows you to more precisely place the block on the page. Using relative positioning, you can specify where on the page it should appear using the 'top,' 'bottom,' 'left,' and 'right' properties. The thing to remember here is that you're telling the block to position itself relative to its normal starting position. It's infinitely useful for when you want an element to appear in a very specific place on the page. Like static, blocks with relative positioning will still affect other blocks, so it's possible for things to get messy quickly.

Absolute is where things start to get a little tricky. Remember all that business about blocks and affecting one another? Yeah, absolute positioning throws that out the window. With absolute positioning, a block element will essentially be ignored by all the other ones. Use with caution, as this can cause an epic traffic jam of block elements that end up on top of each other. The other important thing to remember is that this element will be positioned relative to the first ancestor (an element that the current element is nested inside of) that has been assigned a position value. Basically, if you've given an earlier element that this one fits into, the current element will position itself relative to that one.

Fixed is the last of the positioning values, and it is a bit different from the rest. Instead of either affecting or not affecting other blocks, an element with fixed positioning will follow any scrolling along the page. This is very useful for creating nav bars and anything else you might want to stay with the user on a long page.

Now that you know what the position property is, and the main differences between the four essential position values, you're most of the way to developing a great looking site. Go get 'em!