# Single Page Site Starter

This repo contains starter code for building your single page web site. 

The code here is shown in stages that walk through the process you might follow to if you were building a single page site from scratch. 

# Step 0 - index-0.html

The first step is define a subject and content, then divide the content into sections. 

For the subject you can think about your single page site similar to writing an essay. You'll have an introduction, supporting topics, and a conclusion. 

The difference between the web site and and essay is the website will have pictures and be lighter on text content. 

In [inde-0.html](index-0.html) I've used the boilderplate HTML code along with a series of sectional tags to outline the content. 

```HTML
<main>
	<nav id="nav"></nav>
	<section id="banner"></section>
	<section id="topic-1"></section>
	<section id="topic-2"></section>
	<section id="topic-3"></section>
	<footer id="contact"></footer>
</main>
```

# Step 1 - index-1.html

In this stage I've added content and structure to each section. 

# Step 2 - index-2.html

This step adds a few styles to get the page to display as a series of sections in a single scrolling page. 

```CSS
body {
	margin: 0;
}
```

This block removes the default margin from the body element. Without this you'll a small gap around the edge and your content won't reach the edge of the page. 

```CSS
nav, main > section {
	overflow: auto;
}
```

Margins on elements like h1 and p extend outside their containers. This creates gaps between sections. This rule removes those gaps. Try commenting this out and viewing the code in the browser. 

```CSS
main > section {
	min-height: 100vh;
}
```

I wanted each section to be as least as tall as the size of the window. This rule says the minimum height should be 100% of the view height. 

`vh` is a unit that represents a percent of the browser window. `100vh` is 100% the height of the window. 

```CSS
#nav {
	background-color: #FF3B30;
}

#banner {
	background-color: #26B63E;
}

...
```

These rules apply to each content section through the unique ids assigned to each. Here a different  background color was applied to each section to make them standout. 

# Step 3 - index-3.html

This step takes look at the nav bar. I added some real content and renamed the links and ids for the sections. 

To divide the nav bar into two parts ocupying opposite sides you need two child elements. 

```CSS
#nav {
	display: flex;
	justify-content: space-between;
	align-items: baseline;
	...
}
```

Here I used `align-item: basline` to align all elements on the baseline. This way all of the text "sits" on the same line. 

In the example the right side of the nav is a ul with four items. Use flex again to align these list items in a row. 

```CSS
nav ul {
	display: flex;
	list-style: none;
}
```

The links should have a little more space. 

```CSS
nav ul a {
	padding: 1em;
}
```

# Step 4 - index-4.html

In this step you'll look at one section with a background image and some text content in the center. 


# Step 5 - index-5.html

Creating cards...

# Step 6 - index-6.html

Using max-width and %...

# Step 7 - index-7.html

Create two columns with flex...

# Step 8 - index-8.html

Style the form and footer...