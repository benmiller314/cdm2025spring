
# Writer/Designer's studio: web unit (content focus)

<section class="prereqs">
    <details><summary><strong>Texts to have read</strong></summary>
    <ul>
        <li>Kevin Powell's <a href="https://learn.kevinpowell.co/course/html-css-for-absolute-beginners">HTML & CSS for absolute beginners</a>, up through the end of the <a href="https://learn.kevinpowell.co/course/html-css-for-absolute-beginners/5-selectors-specificity-and-more-styling/1-time-for-version-2">module on Selectors, Specificity, and more</a><ul>
            <li>If you were unable to log in, you could also have done <a href="https://internetingishard.netlify.app/html-and-css/">Interneting is Hard (but it doesn't have to be)</a>, up through <a href="https://internetingishard.netlify.app/html-and-css/css-selectors/">"CSS Selectors"</a></li>
            </ul>
        </li>
        <li>Optional EXT readings on <a href="https://internetingishard.netlify.app/html-and-css/web-typography/">Web typography</a> and <a href="https://css-tricks.com/how-css-selectors-work/">a deeper dive on CSS selectors</a></li>
    </ul>
    </details>
    <details><summary><strong>Work to have achieved</strong></summary>
    <ul>
        <li>Push your tutorial code to GitHub</li>
        <li>Optional EXT playing with the selector game, [CSS Diner](https://flukeout.github.io/)</li>
    </ul>
    </details>
</section>


**Plan for the day**:
1. Threshold Concepts: what you all need to know
2. Ideas for studio <!-- Don't open all of these! Just read the headlines, and get into the inspector demo. -->
<!-- 2. Brief intro to the browser inspector (Firefox, Chrome) -->
3. Set goals and go forth!
4. Update your goals


## 1. Here's what you need to know today
<!--
### Beware of scope creep; plan for phased releases

Bear in mind that you only have a couple more weeks on this project. If you've just given yourself an ambitious agenda, think about "minimum deliverable product" and "stretch goals." You have version control; you can iterate. In other words: you can always come back and add *more*, but it's good to start with what's really at the *core* of your website idea. -->

### Start by thinking about structure (i.e. HTML before CSS)

Remember that though you probably have a vision for how your site should _look_, it makes sense to **begin by thinking about the _structure of your content_**. That will give you the material you need to support _multiple_ views, depending on screen size and/or what begins to feel most important.

So I recommend starting by listing and grouping:

1. What are the content sections your site will include?
2. How might you group those things hierarchically? That is, what's the most important for a viewer to encounter first? Which things are (or could be) parts of others, and which things have to be at the same level?
3. If you can make a nested list of your content areas, that could serve you as a navigation... and probably also a list of headers (`h1`, `h2`, etc).


### You don't have to reinvent the wheel

Like other kinds of media, web design has its genres... and certain _genre conventions_ that solve recurring design problems. You can find some of these by looking at the code of websites you like: you can right-click on any page and choose **"View Page Source"** (or something like it) to see the full rendered HTML page. From there, you can also click the link in the `head` to see the full stylesheet.

<div class="alert alert-warning">NB: This works a lot better on simple, static sites than, say, an e-commerce site that's tracking your clicks in complex ways. But even there, you should be starting to get a sense of how to skim for the recurring chunks of markup.</div>

For instance, a very common structure you should all know about is this one, for a basic navigation menu:
```html
<nav class="main-nav" id="main-nav">
  <ul>
    <li class="active"><a href="/index.html">Home</a></li>
    <li><a href="/about.html">About the Author</a></li>
    <li><a href="/articles.html">Past Publications</a></li>
    <!-- etc -->
  </ul>
</nav>
```

<div class="alert alert-success">
Let's look at this in a testing space: <a href="https://codepen.io/benmiller314/pen/xxpZrOY?editors=1100">https://codepen.io/benmiller314/pen/xxpZrOY?editors=1100</a>
</div>

Note that:

* The semantic element `<nav>` [automatically communicates](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/navigation_role) the navigation role to audio screen readers, helping blind users find their way around your site.
* We use list items so screen readers can easily enumerate the number of locations
* You can use a class like "active" to keep site visitors oriented within the space of your site. (There are other ways, too, but this is pretty simple.)

You can then style that menu to your heart's content:

```css

/***** Main menu styling *****/
  .main-nav {
    background-color: #eee; /* light gray */
  }

  .main-nav a {
    color: #4b8568;         /* dark green */
  }

  .main-nav ul {
    list-style-type: none;  /* Hide the bullets */
    display: flex;          /* Arrange horizontally, not vertically */
    flex-wrap: wrap;
  }

  .main-nav li a {
    display: block;
    padding: 1em 2em;           /* Add a little space around each link */
    text-decoration: none;
  }

  .main-nav .active, .main-nav a:hover, .main-nav a:focus   {
    background-color: #4b8568;  /* dark green, same as link color */
    color: #eee;            /* light gray, same as navbar */
  }

  .main-nav a:hover, .main-nav a:focus {
    text-decoration: underline;
  }

/* etc */
```

Note that:

* We don't need a specialized "button" element for navigation: we're not submitting anything, we're following hyperlinks.
* Instead, we can just style our `<a>` or `<li>` directly (or by adding classes directly to those elements), so it *looks and feels* like a button.
* This is a direct outcome of the Box Model you read about in the tutorial.

### When you're ready to work on appearances, test CSS rules directly in the browser

As I mentioned last time, there are real advantages to testing and revising CSS rules directly in the browser's inspector – especially Chrome (my preference for color) and Firefox (my preference for layout and accessibility checks).
Just **right-click on any element and choose "inspect element"** to see the local html, the _full cascade of CSS rules_ that apply to it, and a few other features beside.

I won't repeat the demo, but I've recorded a <a href="https://pitt.hosted.panopto.com/Panopto/Pages/Viewer.aspx?id=befd7ed1-81e0-4f73-a28e-afc7010eb105">brief screencast demonstration of these tools</a>, should you wish to see it at home.

<aside>Safari can do this, too, but you'll need to <a href="https://developer.apple.com/library/archive/documentation/NetworkingInternetWeb/Conceptual/Web_Inspector_Tutorial/EnableWebInspector/EnableWebInspector.html">activate it first</a>... and then "show the details sidebar."</aside>


## 2. Ideas for studio

In a moment, I'm going to invite you to set goals for studio time: if you've kept up to date with the tutorials, you should now know enough to really start marking up your own content!

**If you haven't yet sorted out your navigation, that's a great place to start.**

Here are some other things to consider as you move forward:

<details><summary>If you're working on the Interneting is Hard tutorial, skip ahead to the semantic html tutorial.</summary>
    <p>You already know that <code>&lt;div&gt;</code> can be used to group items together, e.g. to give them a shared background or border. (They're also kind of key for layout.) But they don't signal what <em>kind</em> of group you're looking at. HTML now has <strong>semantic elements</strong> like <code>&lt;header&lt;</code>, <code>&lt;main&gt;</code>, <code>&lt;footer&gt;</code>, <code>&lt;aside&gt;</code>, and more that signal the role each chunk of code plays in your site.</p>

    <p>This is especially important for assistive devices and their users. And no matter your interface, while coding you may well find them easier to work with than <code>&lt;div&gt;</code>, <code>&lt;div&gt;</code>, <code>&lt;div&gt;</code> all the time!</p>

    <aside>
        <p>HEADS UP for speedy workers: after Semantic HTML, read Web Typography. But beyond that and the other sections I've already assigned, use links from our class schedule for things like responsive layout. The rest of the Internetingishard tutorial is best saved as advanced or historical topics beyond what I'll assign across the rest of the unit.</p>
    </aside>
</details>

<details><summary>Your homepage should be called <em>index.html</em>.</summary>
    <p>I'm going to recommend that everyone use GitHub Pages to publish your sites unless you have a good reason not to. (And you might; but talk to me about it.) In that system, you store your files in a GitHub repository (often in a subdirectory called "docs"), so GH knows where to look to find your stuff. <em>By default, it'll show your README.md file as the home page, unless it finds a file called index.html or index.md</em>.</p>
    <p>Therefore, rather than call your landing page myproject.html, landing.html, or homepage.html, you're better off using the index.html name. You can always change the <code>&lt;title&gt;</code> to give it a more accurate name in the browser tab. : )</p>
</details>

<details><summary>Strive for semanticity.</summary>
    <p>
    Ask yourself:
    <ul>
      <li>Can you tell what's going on just by reading the HTML file?</li>
      <li>Do your header levels (<code>&lt;h1&gt;, &lt;h2&gt;</code>, etc) correspond to your intended hierarchy? Remember not to skip levels: that breaks the .</li>
      <li>Does the HTML hard-code any display (e.g. <code>&lt;center&gt;</code>, <code>&lt;b&gt;</code>) that should be in the CSS? (Older tutorials will suggest this, but it's not a great idea, so you won't find it in either of the tutorials I assigned.)</li>
    </ul>
    </p>
</details>  

<details><summary>Let appearances reflect the structure, not vice-versa</summary>  
    <p>This one's related to the previous item, but applies especially when you're starting to think about appearances. <em>Visuals are volatile; structure should be steady.</em> It can be very tempting to just accept your browser's default styles as a given, e.g. to jump from a large <code>&lt;h1&gt;</code> page title to an <code>&lt;h5&gt;</code> subtitle because the latter "looks about right." But this would mis-represent the actual structure of the document – and would seriously confuse screen-reader software trying to present the page to a blind visitor. Instead, use your browser's Inspector to take note of the CSS rules defining that <code>&lt;h5&gt;</code>, and apply them to <code>&lt;h2&gt;</code> in your stylesheet.</p><!-- This makes a good jump-point into the inspector... -->
</details>

<details><summary>Done with content, ready for CSS? Start with some basic spacing</summary>
    <p>As Kevin Powell will explain in the <a href="https://www.youtube.com/watch?v=VQraviuwbzU&list=PL4-IK0AVhVjM6kuUoUexfmnD8vHtZkXdd">video you'll all watch for homework</a>, "Before you write a single line of CSS, your website is responsive." If you keep your styles minimal, you'll have a fully-functional website, especially suited for smaller screens.</p>

    <p>In particular, I recommend making the following quick changes for pretty much any site (and you can always make it more complex later):</p>

    <pre>
    <code>
    /* include padding/margin in your width declarations */
    * {
        box-sizing: border-box;  
    }

    /* basic spacing */
    body {
        padding: 1em;     /* avoid crowding content against the edges */
    }

    /* make the appearance less "default".
       Note that this is a light theme; you could also make a dark theme by reversing the colors. */
    body {
        font-family: sans-serif; /* for body text on a screen, sans-serifs are often easier to read */
        color: #333;             /* pull back from hard black */
        background-color: #ddd;  /* pull back from hard white */
    }

    /* Use this class on section, article, or div elements
       to keep text lines from getting too long to comfortably read */
    .wrapper {
        max-width: 50em;  
    }

    /* keep images from overflowing the viewport */
    img {
        max-height: 100vh;
        max-width: 100vw;
    }

    </code>
    </pre>
</details>


## 3. Go forth!

In the [shared google doc](http://bit.ly/cdm{{site.course.slugterm}}-notes), **set a goal for today**: what do you need to do to level up on HTML, CSS, and resource gathering to move toward your specific project? Note that a Website Preview is due a week from today.

<!-- <div class="alert alert-info">
If you haven't yet, please do expand and read my notes above. Also remember that you have many <a href="{{site.github_url}}/resources#web-design">Resources</a> on our website; for today, might I especially point out the <strong>design advantages of <a href="https://loremipsum.io">placeholder text</a> and/or <a href="https://loremipsum.io/21-of-the-best-placeholder-image-generators/">images</a></strong>?
</div> -->

<div class="alert alert-info">
If you haven't yet, please do expand and read my notes above. Also remember that you have many <a href="{{site.github_url}}/resources#web-design">Resources</a> on our website; for today, might I especially point out the <strong><a href="https://benmiller314.github.io/cdm2025spring/resources#web-design:~:text=Some%20extensions%20I%20expect%20you%27ll%20find%20useful">helpful VS Code extensions</a></strong>, especially <a href="https://marketplace.visualstudio.com/items?itemName=Compulim.compulim-vscode-closetag">Close HTML/XML Tag</a>? Pulsar should have the equivalent function already installed when you download it; look for the keyboard shortcut under Packages > Bracket Matcher > Close Current Tag.
</div>

Save about five minutes at the end to write me a brief exit note about what you've been working on.

## 4. Exit note
<div class="alert alert-success">
Before you leave, just as a way for me to check in, I'd like to hear more about what happened today: Did you decide on your navigation? Block out the html? Make some progress on a stylesheet?

<strong>Reply to your note in the <a href="http://bit.ly/cdm{{site.course.slugterm}}-notes">google doc</a>.</strong>
</div>

# Homework for next time
* **View** Kevin Powell's video on [5 simple tips to making responsive layouts the easy way](https://www.youtube.com/watch?v=VQraviuwbzU&list=PL4-IK0AVhVjM6kuUoUexfmnD8vHtZkXdd&index=4) (runtime: 15:53 at 1x speed)
    - and catch up on any tutorial chapters you've missed so far. For Interneting is Hard users, that should include the chapter on Semantic HTML.
* **Compose and push** a _first draft_ of your website: a beginning, focused on html content and mobile (i.e. minimal) design.
    - If you've missed any of the expandable tips in today's lesson plan, please do check them out!
* _Recommended EXT:_ **Read** [Getting Started with the Google Fonts API](https://developers.google.com/fonts/docs/getting_started) and recall your knowledge of font choices from the visual unit to **choose** one main body font and one main header font (or consciously keep them the same, but at different weights / font sizes)
* _EXT for eager readers:_ Want still more advice?
    - Dive back into design principles: [Improve Your Designs With The Principles Of Continuation And Common Fate (Part Three)](https://www.smashingmagazine.com/2016/05/improve-your-designs-with-the-principles-of-continuation-and-common-fate-part-three/)
    - Get into the weeds with web fonts: [Choosing web fonts: A beginner's all-in-one guide](https://fonts.google.com/knowledge/choosing_type/choosing_web_fonts_beginners_guide)
