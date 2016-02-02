---
layout: post
title: "Les Enumerables"
date: 2015-10-11 14:37:44
categories: lesson
---
<img src="{{ site.baseurl }}/images/pic02.jpg">

Wow, what a week. Methods, methods, methods!

This week, I'm going to be talking about a really interesting and powerful tool called an **Enumberable** method. Specifically, I'm going to be explaining the <code>.map</code> method.

Before I can explain what <code>.map</code> will do for you, I'll have to explain what iteration is and what it does for collection objects.

Collection objects are simply objects that contain collections or lists of other things. These would be objects such as arrays, hashes, sets, and ranges. With iteration, we can run code over (or iterate over) each element of the collection object. This in itself is an immensely powerful feature of programming in general, allowing us efficiency and letting the computer do all the heavy lifting. Let's take a look at an example:

<code>array.each { |i| i + 1 } </code>

What this is saying is: "for every element that's in the array, add one to it." It also works by taking one element at a time, running the code in the curly braces, and spitting it back out.

From there, we can drill one level deeper on what an Enumerable method is. An enumerable method is one that is shared across multiple collection objects. Technically, Enumerable is a module included in all collection objects by default, and it allows for the use of iteration methods, specifically <code>.each</code>. In fact, one of the requirements for Enumerable to be included in a class, is for the <code>.each</code> method to be defined!

Now that you understand a little better about what iteration and what Enumerables are, it becomes much easier to grasp what the Enumerable method <code>.map</code> will do for us. The <code>.each</code> method and <code>.map</code> methods are actually very similar, so understanding <code>.map</code> will just be adding to what we already know about <code>.each</code>. Where <code>.each</code> will iterate over an array or hash and return the values of our array or hash with the new results, <code>.map</code> will collect those results into a brand new array object! This allows us to create a non-destructive method for changing our collection object and RETAINING those changes in a new array. Amazing, right? <code>.map</code>'s syntax works the same way as <code>.each</code>, but let's look at an example:

<code>array = [1, 2, 3]</code>

<code>array.each { |i| i + 1 }</code>

<code>y = array.map { |i| i * 1 }</code>

In this example, <code>.each</code> will return the output of the block of code as performed on each element of the array, but the original array elements are untouched. However, with <code>.map</code>, we've actually created an entirely new array, which we've assigned to <code>y</code>. Now that you understand these concepts, go forth and code!
