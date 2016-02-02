---
layout: post
title:  "Buckets of Fun"
date:   2015-10-15 14:37:44
categories: lesson
---

<img src="{{ site.baseurl }}/images/pic01.jpg">

Well I'm delirious from lack of sleep, so that should probably tell you plenty about arrays and hashes.

So first, let's talk about what arrays and hashes are. As you can probably already gather, the easiest way to understand arrays and hashes is as buckets that contain other things. Those things can be any Ruby objects! You want an array of numbers? Piece of cake for an array! You want an array of strings? Perfect! You want to get REALLY crazy and put arrays in your arrays? Go for it, dawg. It works the same way with hashes, which gets even crazier in ways I'll get into momentarily.

Before that, let's just take a quick look at an example:

```
array = [1, 2, 3]
```

Look at that majestic array. This one is fairly simple, but as you can see, it's just a list of integers, 1 through 3. The way that arrays work is that although you can think of the array as a bucket, the contents are a list that follow a sequence. You can refer to the individual contents of the list by referencing the index value. What this means is that everything in the bucket of the array has a number associated with what slot it occupies. The first slot is (seemingly counterintuitively for the layman) labeled as 0, with the next slots being numbered in sequential ascending order from there. So in our example, the number 1 is sitting in index 0, and can be called out individually from the list by referencing my_array[0] in your code. This is where arrays get all their power and usefulness. Now let's look at hashes.

<code>
	hash = { "Jim" => "burger", "Sarah" => "tacos", "Sam" => "salad" }
</code>


Well that's... different. So hashes may look a bit odd at first, but if you can understand that if an array is a list, a hash is a pair of lists, with each item corresponding to one other item in the opposite pair in what are known as keysand values. For example, in the snippet above, you can see that the names are pointing to a food item. In this example, the names are the keys, and the food is the value assigned to that key. The handy little  ```=> ```
notation is an arrow that visually represents this relationship.

Now that you know what arrays and hashes are, we can talk about their applications. The biggest difference between arrays and hashes are obviously the fact that hashes can assign meaning to an object for later recall, wheras arrays are just an ordered list. What this means is that like our example, hashes are good at association of two lists, or creating categories. Since you can assign a key with a value of another list, you can keep track of lists by using category names. You could keep a list of models of car by make, or like above, you could track what people ordered at a restaurant.

That wraps it up for a base understanding of arrays and hashes. Use that knowledge responsibly, and have fun with your buckets!

