HTML+CSS Tutorial
=================

###Who

I'm Cassidy.  I'm a current student in computer science and I've been teaching myself HTML, CSS, and other web programming and scripting for over 8 years.
And I want to teach you now.
Because you're good looking.
And because it's useful.

###What

In this tutorial, we'll start from the very beginning.  You don't need to know anything about HTML and CSS to start.  I'll include some tutorial files for you to play with and check out.

###When

Now.  Or whenever.  I'm not planning on taking this down anytime soon.  But you are only limited by your own schedule.  Or set free by it.  Whatever.

###Where

On a computer.  Here.

###Why

Because this stuff is important.  Whether you're a business person formatting your emails, an aspiring web designer wanting to get your feet wet, or just someone who is interested and hasn't tried any sort of coding, scripting, or programming before, **HTML and CSS are an essential part** of your learning curve.

##Let's Go.

###Editors

So the first thing you'll need is an editor to edit your jazz.  There's tons of options out there.

- [Notepad](http://en.wikipedia.org/wiki/Notepad_(Windows)) (that's right, the stupid thing that comes on your PC) - This is about as basic as you can get.  It's totally okay if you want to use this, but I recommend one of the editors below just so you can see code highlighting (which will help you out later on).  But, if you want to be a purist, this'll work just fine.
- [Aptana Studio 3](http://aptana.com/) - This is what I typically use.  It's fairly easy to navigate, you create projects in it and it supports standard web projects, PHP, and Ruby.  If you're a beginner that probably means nothing to you.  Anyway, a decent choice.
- [Sublime Text 2](http://www.sublimetext.com/2) - This is a pretty popular option, and for good reason.  Very clean interface.  Once you can navigate it (learning curve isn't that big), it's pretty dreamy.  Like your face.
- [Notepad++](http://notepad-plus-plus.org/) - This is just one step up from Notepad.  But it's pretty dece.  Code highlighting is in it, and nothing else too fancy, which is what I like about it.

There's a bunch of others [listed here](http://en.wikipedia.org/wiki/List_of_HTML_editors), I just listed the ones I've used and liked!

###HTML Tag Structure

Here is a barebones HTML page, about as simple as you can get.  You can open it up in the Structures folder in the file part1.html.  If you were to open the file in your favorite browser (which you can do, go ahead), you'll see a plain webpage with the title "My Website" and the words, "Hello, World!" written on the page.

	<!doctype html>
	<html>
		<head>
			<title>
				My Website
			</title>
		</head>
		<body>
			Hello, World!	
		</body>
	</html>

So, what are we looking at here?
HTML consists of these things called tags, which are names written between `<` and `>` characters, like `<sometag>`.  All tags (with just a few exceptions that we'll talk about later) have a matching closing tag, which has the same name as the opening tag, except that it contains `/` after the first `<`, like `</sometag>`. 

For example, `<html>` is one tag and the closing tag for it is `</html>`, same with `<head>` and `</head>` and `<body>` and `</body>`, and so on.  You get it.
The opening and closing tags together are an *element* (which also includes everything written in it).  For example, `<title>My Website</title>` is one element.  The text inside an element, in the title case, `My Website`, is called the *content* of an element.

Tags organize your page and tell the browser what your page consists of.  There's tons of tags out there, some that you may never use.  
Here's some lists of tags if you really care to see all of them at this point:
- [HTML Dog Tag List](http://www.htmldog.com/reference/htmltags/)
- [W3Schools Tag List](http://www.w3schools.com/tags/default.asp)
- [Quackit HTML Tag List](http://www.quackit.com/html/tags/)

So, if you look at our example, you can also put tags inside other tags (like we did with the `<title>` tags inside the `<head>` tags).  This is called *nesting* elements.
In this case, we would say that the `<head>` *contains* the `<title>`.  Sometimes when you have a lot of nested tags, it's hard to keep track, so you have to format your code with spacing, as shown.  Typically, inner tags are spaced more than their outer tags (just as `<title>` is indented further than `<head>`).

Let's take a look again at part1.html in the Structure folder.  You'll notice that the first line has `<!doctype html>`.  Every HTML document and website has to have this special tag, as it tells the browser what language we're using.  This is one of those special tags I mentioned that doesn't need a closing tag.

On the second line, you can see a `<html>` tag.  Everything in the website is contained by this tag, and the last line of your entire document will always be `</html>`.

Inside `<html>`, there are two elements: `<head>`and `<body>`. Contained in `<head></head>`, we will put all kinds of information for the browser that the user doesn't necessarily need to see.  For now, we just have `<title>`. The content of `<title>` will be used for the name of the tab of the browser, and also by search engines. 

On the other side of the planet, we have `<body></body>`.  Everything visible to the user is contained in these tags.  Right now, all that consists of is "Hello, World!"  Let's change that for fun.  Replace "Hello, World!" with your own text in your favorite HTML editor, and then open the page in the browser.  Neat!

###Structuring text

Let's get juicy.  We're going to talk about some new tags for structuring your text.  Because you're not going to want just one kind of text throughout your whole website, right?

Check out part2.html in the Structure folder.  The tags that we'll be talking about here are `<h1>`, `<p>`, `<ul>`, and `<li>`.  Open the file in the browser to try and understand what the heck is going on. 

Now, let's talk about it.

First, we have `<h1>`, which adds a *heading* to our website.  Basically, a heading is just text with a bigger font.  But still.  Important. We'll soon learn how to adjust any and all font sizes, but not yet.  Just know that your headings should be in `<h1>` tags.  Also, if you have a smaller heading, or *sub-heading*, you could use `<h2>`, which is smaller than `<h1>`, but bigger than regular text.  You can keep going with more numbers until you reach `<h6>`, with each heading a bit smaller than the previous.  Try adding some subheadings underneath our current heading!

Next, we have `<p>` tags.  `<p>` adds a *paragraph* of text to our website, which are blocks of text that have some space before and after them.  Edit the text in the paragraphs given, and add your own to see what I mean!

And finally, we have `<ul>`.  `<ul>` means a bulleted list (also known as an *unordered list*), where every `<li>` is an item in that list (called a *list item*). But what if you want a numbered list?  You could change `<ul>` to `<ol>` (and don't forget its closing tag), it's that simple!  `<ol>` is an *ordered list*, which has numbers instead of bullet points, and that is truly the only difference.  Add some list items (`<li>`) to the list (make sure you stay inside the `<ul> tags`), and then change your `<ul>` tags to `<ol>`!

## Wut
That's right, I haven't written the whole tutorial yet.  Be patient.  I have to get my ducks in order so I can astound your face.
