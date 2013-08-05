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

- Notepad (that's right, the stupid thing that comes on your PC) - This is about as basic as you can get.  It's totally okay if you want to use this, but I recommend one of the editors below just so you can see code highlighting (which will help you out later on).  But, if you want to be a purist, this'll work just fine.
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

And finally, we have `<ul>`.  `<ul>` means a bulleted list (also known as an *unordered list*), where every `<li>` is an item in that list (called a *list item*). But what if you want a numbered list?  You could change `<ul>` to `<ol>` (and don't forget its closing tag), it's that simple!  `<ol>` is an *ordered list*, which has numbers instead of bullet points, and that is truly the only difference.  Add some list items (`<li>`) to the list (make sure you stay inside the `<ul>` tags), and then change your `<ul>` tags to `<ol>`!

###Links

Links are what makes the world/Internet go 'round.  Seriously.  So, let's learn about them.

Links are made with the `<a>` tag, which stands for *anchor*.  

Open up the Tags folder, and add this piece of code after your heading in page1.html:

	<p>This paragraph <a href="http://www.lalalalalalalalalalalalalalalalalala.com/">has a totally awesome link.</a></p>
	
Open page1.html in a browser and click on it!  BEAUTIFUL.

Okay, so let's take a look at this.  First of all, you can see the `<a>` tag there contained in the paragraph.  Beautiful.
But what's that funky milk `href=`?  Well, that syntax called an *attribute*.  Attributes change the way a tag works, and are not visible to the website's user.  You only add attributes to the opening tag, not a closing tag.  Tags can have multiple attributes, for example:

	<tag attribute="value1" attribute2="value2">Content of tag</tag>`

Got it?  Good.  You're so good looking.

So, anyway, the attribute 'href' tells us where the link is going to go when the user clicks on it (and for those curious, it stands for *hyperreference*).  Try adding some more links to the page to different websites!  

Also, one thing you should note:  Links don't have to be in `<p>` tags like I put above.  You could put them in `<li>` tags in a list, `<h1>` tags for a linking header, or completely on their own!

####Adding links to other pages in your website
Let's just say you have a fully functioning website called fakewebsite.com.  You have your homepage and your "Contact Us" page in the same directory or folder.

Normally when a beginner links to different pages on their website, they just make links that look like `<a href="http://www.fakewebsite.com/index.htmL">Home</a>` and `<a href="http://www.fakewebsite.com/contactus.htmL">Contact Us</a>`.

This is okay.  BUT, you can do better.  So, what if you change your domain name to reallyfakewebsite.com?  When you edit your HTML, you'd have to edit every single one of the links to match the new domain.  That's gross.  There is a better way.

When you make a link to a page within your own directory or folder on your website, instead of putting in the whole URL, put in something more like this:

	<a href="page2.html">Click here to go back to Page 2.</a>
	
Paste this line of code into page1.html.  Watch the magic happen.

Now, if you were to change your domain or location of your files, you don't have to change a thing.  Boo yah.

###Other tags

So, you can reference the links that I showed you before if you want to check out some jazzy stuff you can do with your page.  There are some other ones though that you might want to see before we move on to cooler and bigger things.

####Images
`<img>`. Let's just say you want to put an image on your website.  This is probably a good tag to know.  
Add the following to page1.html:

	<img src="http://i.imgur.com/B9q0A.gif" />
	
Open up the page in a browser.  WHOA.  Image!  So, the `<img>` tag is one of those special tags.  First of all, it doesn't have a closing tag.  You just stick in a `/` at the end of the one tag and you're done.  Secondly, it also has a `src` attribute (which is short for *source*), and in the value of that attribute you put the URL of the image (similar to `href` in the anchor tag).

####Line breaks
Let's just say you want to keep all your content in one paragraph `<p>`, but you still want to break it up.

That's easy.

So, there's two special tags here, `<hr>` and `<br>`.  They are *empty tags*, meaning they have no closing tag.

`<hr>` stands for *horizontal rule*, and creates a visible line break.
`<br>` is a simple line break, all it does is split your paragraph up.

Try inserting these in between some of your `<p>` tags to try it out!

####Tables
Tables are really cool.  They can also be a bit confusing.  Open up tables.html (in the Tags folder) in a browser to check out the example table I made for you there.

There's several tags for tables, but the essential ones are `<table>`, `<tr>`, `<th>`, and `<td>`.  Look at tables.html in your editor.

We're going to make our own table again on this page.  You can delete the one I made for you, or just make one underneath the current one there.

So, to create a table, you start with the `<table>` tag.  Simple enough.
	
This will contain all the parts of your table.  Sometimes, tables have a `border` attribute that will equal some value for the thickness of the table's border.  Go ahead and add one so it looks like this:

	<table border="1">
	</table>
	
Boom.  Let's add some more.

The next tag we're gonna check out is `<tr>`, which is for a *table row*.  Easy peasy.  So, let's add 3 `<tr>` tags to our table.

	<table border="1">
		<tr>
		</tr>
		<tr>
		</tr>
		<tr>
		</tr>
	</table>
	
And finally, we have the actual cells of the table.  There are two types of tags for this, `<th>` (*table header*) and `<td>` (*table data*).  As their names indicate, the former is for the header of the table and the latter is for all of the data in the table.

In our first set of `<tr>` tags, add 4 `<th>` tags, and in the second and third `<tr>` tags add 4 `<td>` tags.

	<table border="1">
		<tr>
			<th></th>
			<th></th>
			<th></th>
			<th></th>
		</tr>
		<tr>
			<td></td>
			<td></td>
			<td></td>
			<td></td>
		</tr>
		<tr>
			<td></td>
			<td></td>
			<td></td>
			<td></td>
		</tr>
	</table>
	
Alright!  Our table is all set up.  We have a table with a `border=1` attribute, 3 rows, and 4 columns.  Let's populate it with data so you can see a proper application of the `<table>` tag:

	<table border="1">
		<tr>
			<th>Item</th>
			<th>Quantity</th>
			<th>Rate</th>
			<th>Cost</th>
		</tr>
		<tr>
			<td>Candy</td>
			<td>10</td>
			<td>$.50</td>
			<td>$5.00</td>
		</tr>
		<tr>
			<td>Toothpaste</td>
			<td>2</td>
			<td>$3.00</td>
			<td>$6.00</td>
		</tr>
	</table>
	
Open the page in a browser and check out your work.  Nice job!  I'm truly impressed.  Go eat something good and fattening.

One other fun thing you can try playing with are the `colspan` and `rowspan` attributes.  If you add `colspan="2"` (or `rowspan`, or any other number) into a `<th>` or `<td>` tag, the cell will expand past their cell size.  For example, `<th colspan="2">` will give you a table header that spans 2 columns, and `<td rowspan="3">` will yield a cell that is the height of 3 rows.  Jazzy!

You can also nest tables, but I won't get into that right now.  If you want to play around with the code, try adding some `<tr>` and `<td>` tags inside your current `<td>` tags.  MaGiCal ThInGs.

###Making Things Gorgeous The Wrong Way

So, your website right now looks pretty bland, and that's normal.  But, we want a website that is hot, sexy, ravishing, and powerful.  Yes, that's right, we want a website just like you.

So first, I will show you the wrong way to style your pages.  You might ask why, but trust me, if you learn in this order, you'll understand HTML attributes a lot better, and then when you move on to CSS your mind will explode with joy.  Explode.

####Colors

Alrighty.  Let's get frisky.  Open up the Styles folder and the file style1.html.  You might notice that this file is pretty bland right now, but that's what we're gonna fix.  Be patient, my grasshopper.

Add this line of code in the `<body>` somewhere below the header tags (I made a lot for fun... you can change them if you want): `<p style="color: red">This text is hot like my body</p>`

Oh man.  Load that baby in a browser.  WHAT.  MAGNIFICENT.  COLOR.

The first thing we'll look at is the `style` attribute.  You can style all kind of things in that, from colors to widths to heights to borders to weights.  But for now, let's just talk color.

So, you might wonder, "what the heck how does that work can I just type any color in that space where red is?"  And the answer is no.  You can type a ton of colors there, like `blue` and `yellow` and `cyan` and `magenta`, but you can't just say `oasisorange` or `electricwhite` and hope that that'll work.

How do you get a specific color of your liking?  Well that's when you use RGB or HEX colors.  This is kind of a pain to grasp, it took me a little bit, so I'll explain it as simply as I can:  RGB stands for Red, Green, and Blue.  You can have the values 0 to 255 in each to form pretty much any color in existance.  Whoa.  The way to form an RGB code similarly to the one above is simple: `style="color: rgb(255,0,0)"`.  In this example, there's 255 reds, 0 greens, and 0 blues.  So, it's all red.  Boom, simple enough.
Now HEX colors is very similar.  It consists of the hashtag sign `#`, and then 6 *hexadecimal digits*, which are 0123456789ABCDEF, with F being the highest digit.  Like RGB, the first two digits of HEX are reds, the second two digits are blues, and the third couple of digits are greens.  So, to write the same color code above, you'd do `style="color: #FF0000"` to get red, because you have FF for reds, 00 for blues, and 00 for greens.  Simple?  Simple.  

Don't worry, you won't have to come up with RGB and HEX colors yourself.  There's plenty of websites and programs and color pickers out there to help you with that.  Here's a few:

- [Color Picker](http://www.colorpicker.com/)
- [HTML color codes and names](http://www.computerhope.com/htmcolor.htm)
- [HTML Color Codes](http://html-color-codes.info/)
- [HTML Color Picker](http://www.w3schools.com/tags/ref_colorpicker.asp)

Try adding colors to various tags on the page!  You can make your `<h1>` the color `#005DFC`, your `<h3>` rgb(242,127,56), and your `<p>` `lightblue`.

## Wut
That's right, I haven't written the whole tutorial yet.  Be patient.  I have to get my ducks in order so I can astound your face.




























