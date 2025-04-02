
# Web Unit Post-Workshop Studio

**Work to have done**: asynchronous peer-review; optional [forum post about possible consolidation-unit projects]({{site.github.issues_url}}/13)

**Plan for the day**:

* Planting seeds
* Gathering questions
* Studio time!
  - Check for new feedback
  - Set an intention
  - Work time
  - Exit note



## Planting seeds

As a reminder of past advice, please:
* **Call your homepage index.html**. (Other html files can be called whatever you want... but will probably work best in lowercase and without spaces.) Note that you don't need to add a new subfolder: placing the html files directly inside **docs** is easiest for publishing, as any subdirectories will become part of your site's URL.
* Be sure to **include some [basic spacing](../plans/lesson-18#:~:text=Done%20with%20content%2C%20ready%20for%20CSS%3F%20Start%20with%20some%20basic%20spacing)**, even if you're keeping your CSS minimalist, to limit the length of lines and let your content breathe.

In addition, after reading through the drafts and comments, I've come up with the suggestions below. While not all these ideas will apply to every project, they all apply to more than one, and some projects could benefit from several. Please start by reading through these notes and considering where each might help you!


<details><summary>Have text running into a background image? Try a container with <code>backdrop-filter</code> to improve contrast.</summary>
    <p>To quote <a href="https://developer.mozilla.org/en-US/docs/Web/CSS/backdrop-filter">the MDN documentation</a>, <blockquote>The <strong><code>backdrop-filter</code></strong> CSS property lets you apply graphical effects such as blurring or color shifting to the area behind an element. Because it applies to everything <em>behind</em> the element, to see the effect the element or its background needs to be transparent or partially transparent.</blockquote></p>

    <p>With just two lines of CSS (again, I'm quoting MDN here), you can add a kind of "frosted glass" effect that will help your foreground pop:</p>

    <pre><code class="css">
.box {
    background-color: rgb(255 255 255 / 30%);
        /* note that 30% opacity; some transparency  */
        /* is required for this effect.              */
    backdrop-filter: blur(10px);
}
    </code></pre>

    <p>Be sure to check out their example at the bottom of the page linked above.</p>
</details>

<details><summary>If alignments or aspect ratios get weird when you resize the window, level up with Grid and Flexbox.</summary>
<!-- TO DO: add gifs of these changes -->
    <p>While the basic starting point for a CSS grid has you declaring an explicit number of columns (and sometimes rows), the implicit grid can be very powerful. Check out <a href="https://gridbyexample.com/examples/example28/">Rachel Andrew's use of auto-fill repeating tracks</a>: with a single line of CSS...</p>
<pre><code>grid-template-columns: repeat(auto-fill, minmax(200px, 1fr) ) ;</code></pre>
    <p>... she sets up a flexible number of columns. Instead of warping to get smaller than their preferred size (here, 200px), the items just wrap into the next row, and grow to fill the available space. When the window is wide enough for another 200px item, it automatically rearranges the grid.</p>
    <p>In that example, each item is just a box, but there's no reason it can't be a <em>flex</em>box or grid itself, and in fact this is a super-common pattern, often called a <a href="https://developer.mozilla.org/en-US/docs/Web/CSS/Layout_cookbook/Card">card layout</a>. A group of divs (the cards) is arranged in a grid, and each inner div (card) will contain an image and some text. With a few quick lines, you can line up the card's content neatly:</p>
    <pre><code class="css">
.card {
    display: flex;
    justify-content: space-between;
    align-items: stretch;          /* or center */
}
</code></pre>
    <p>The MDN card layout linked above uses grid for the card, too, so you've got options.</p>
    <p>P.S. Have different sized images, rather than cards all alike? Try the <a href="https://developer.mozilla.org/en-US/docs/Web/CSS/grid-auto-flow"<code>grid-auto-flow: dense</code></a> property.</p>
</details>

<details><summary>Reuse your stylesheet on multiple pages if the rules haven't changed.</summary>
  <p>As I noted in response to questions about the baseline call for a "sitewide" stylesheet, it's an important threshold concept of CSS that you can have a single set of rules that are invoked in multiple places. In other words: instead of copying out your rules into a new file for each HTML page, just copy the <code>&lt;link rel="stylesheet" href="styles.css" /&gt;</code> from your first page into the <code>&lt;head&gt;</code> of your second page (and third, and fourth, etc).</p>
  <p>If you do have a style that you want to change – say, a heading size that's bigger on the homepage than on other pages – you can "scope" those rules with descendent selectors. For example: <pre><code class="css">
        body {
          font-size: 18px;    /* sets the baseline font size */
        }

        /* heading styles for most pages */

        h1 {
          font-size: 2em;     
        }

        h2 {
          font-size: 1.75em;
        }

        /* bigger heading sizes for home page */

        body.home h1 {
          font-size: 4em;
        }
      </code></pre>
  </p>
  <p>That last rule selects <code>h1</code> elements only if they're inside a <code>&lt;body class="home"&gt;</code>. You add the class to the opening <code>&lt;body&gt;</code> tag at the top of the file, and voila! A per-page style within a single sitewide stylesheet.</p>
</details>

<details><summary>Use alt text to convey significance as well as the basic facts.</summary>
    <p>Text-alternatives, which you add to images using <code>&lt;img alt="text description here" src="path/to/source.jpg"&gt;</code>, are a required element in validated html. They're also really helpful, and not only to blind users: they make the html file more readable on its own, and thus more semantic, and they help you troubleshoot layout when image paths are broken by showing you where each image is trying to appear.</p>
    <p>But alt text can also be <em>fun</em>: its purpose is to provide a way for more users to experience your site. If the image is there to help us get a sense of <em>you</em>, the words should do the same. If the image is there to add beauty, let your words add beauty; if the image is there to make us smile, relax, laugh, cry, imagine ways you might get us there – at least part of the way – with words.</p>
    <p>For some inspiring examples of poets having a go at alt text, see the <a href="https://docs.google.com/document/d/15oSMuDX5OnYaJ6ZTe5QVTC2fB7kE-EDY5wPQMmD-3BA/edit?tab=t.0#heading=h.xuogj64mgi96">Alt Text as Poetry Workbook</a> by Bojana Coklyat and Shannon Finnegan. For bad AI-generated alt text accompanied by some inspired textual descriptions of color, see <a href="https://cripritual.com/haagaard/">Alex Haagaard's "Shitty Alt Text" project</a>. For general guidance on how to write useful alt text, including many further links and examples, see <a href="https://www.perkins.org/resource/how-write-alt-text-and-image-descriptions-visually-impaired/">Veronica Lewis's guide for the Perkins School for the Blind</a>. </p>
</details>

<details><summary>Remember to credit your sources somewhere on the site.</summary>
  <p>If you're using resources you didn't make yourself, be sure to <em>include enough information to recover where it came from</em>: a direct link to the image and to the specific license (if there is one) is ideal. Creative Commons sources often provide that html for you!</p>
  <p>Where to put this information? Ideally, somewhere small near the image itself. (There's a semantic html way of doing this with <code>&lt;figure&gt;</code> and <code>&lt;figcaption&gt;</code>, which you may remember from <a href="https://www.internetingishard.netlify.app/html-and-css/semantic-html/#figures-and-captions">the Semantic HTML</a> section of the tutorial. See also <a href="https://www.scottohara.me/blog/2019/01/21/how-do-you-figure.html">this extended discussion of figures, figcaptions, and alt text</a>.)</p>
  <p>Alternately, you can have a rights page somewhere, or use the site footer – or have a live hyperlink from your site to an external credits.md file in your repo.</p>
  <div class="alert alert-info"><em>NB: If an image is under copyright, you can still use it if you can make a good case that it's a Fair Use.</em>  See the homework reading after <a href="lesson-04">Lesson 4</a> to review the Four Factors you need to consider.</div>
</details>

<!-- <details open><summary>Level up your HTML.</summary>
<p>There are a few patterns that I notice often as people learn HTML and search for models online:</p>
  <details><summary>Use <code>div</code> for grouping, semantic HTML for basic structure</summary>
    <p>When you have divs inside divs inside divs, they all start to flow and meld and it's hard to see what role each thing is actually playing. Sometimes we call this "div soup." To help with that, <em>see whether you can replace some with a more semantic tag</em>: <ul><li>Is that div with one line of text acting like an <code>&lt;h2&gt;</code> (or vice versa)?</li><li> Are those divs wrapping up each of several items, each with a recurring structure like photo / name / description? Maybe they're actually <code>&lt;article&gt;</code>s.</li><li>Is the whole display of articles really a <code>&lt;section&gt;</code>?</li><li>etc</li></ul></p>
  </details> -->
  <!-- <details><summary>Avoid hard-coded spacing</summary>
    <!-- AFTER 2023 SPRING: add note warning against using padding or margin for layout. Padding should be used to adjust the size of individual elements, so that flex or grid can assign the remaining whitespace responsively. Margins should be used to keep adjacent elements (or groups of elements) from crashing into each other. Note that you can also use gap for this purpose, if you're within a grid or flexbox. -->
    <!--    <p>When I say "hard-coded spacing," I mean especially spacing that uses <code>&lt;br/&gt;</code>. That tag is not really for spacing, but rather for creating <em>manual but meaningful line breaks</em>. Think poetry, or maybe a two-part heading where you want to enforce a particular phrasing (e.g. a line break after a colon). A real <code>&lt;br/&gt;</code> should itself be part of your content, a piece of punctuation as much as a comma or period.</p> <p>Instead of hard-coding space after your paragraphs or headers, a better practice is to give them some <code>margin-bottom</code>, which you can also adjust using <code>@media</code> queries if need be. A margin of 1em or slightly more (depending on your <code>line-height</code>) should do the trick.</p>
  </details> -->
  <!-- <details><summary>When I say don't skip heading levels...</summary>
    <p>Headings like <code>h1</code>, <code>h2</code>, and <code>h3</code> are essentially the outline of your site's content. You should be able to read them to get a stripped-down sense of what the page is about. For screen-readers that read sites out loud to blind or vision-impaired visitors, this outline of headings can be literally the first way the page is presented.</p>
    <p>For that reason, your headings should follow a nested sequence that respects their numbers: the top-level heading on any given page should be an <code>h1</code>, and you shouldn't have any <code>h3</code>'s unless you first proceed through <code>h2</code>. If you like the look of a smaller header, but that would "require" you to skip a level, instead use your browser's inspector to find the current CSS – font size, color, spacing, etc – and copy/paste that into a new rule for the heading level you're actually up to.</p>
    <p>(See the <a href="https://flukeout.github.io/">CSS Diner</a> for tips on limiting the scope of these changes through classes and descendent selectors.)</p>
  </details> -->

  <!-- <details><summary>Remember to proofread for tag nesting.</summary>
    <p>The <code>&lt;body&gt;</code> should be at the top of the page, but I also know it's often confusing for newcomers to html: many of you are naturally inclined to put your navigation up above the body tag, sometimes in the head and sometimes even above the html tag. I get it: in many contexts, the "body of the page" doesn't include things like headings and menus. And many browsers will be flexible enough to figure out what you mean.</p>
    <p>But properly speaking, the <em>entire</em> rendered content of the page should fall between <code>&lt;body&gt;</code> and <code>&lt;/body&gt;</code>, and <code>&lt;/html&gt;</code> should be the last line in the file with any content. (A blank line after that is fine.)</p>
    <p>An html element that you can use instead of <code>&lt;body&gt;</code> to designate the main area of the page is, appropriately enough, <code>&lt;main&gt;</code>.</p>
  </details> -->


<!-- <details><summary>Level up your ordered lists.</summary>

Did you know you can choose the number an <code>&lt;ol&gt;</code> list starts with?

You can also <a href="https://css-tricks.com/almanac/properties/l/list-style">choose different list-item-types</a> for alphabetical or roman counting systems. Same goes for bullets in your <code>&lt;ul&gt;</code>'s.
<figure role="figure">
<p class="codepen" data-height="265" data-theme-id="light" data-default-tab="html,result" data-user="matt-west" data-slug-hash="DCEzd" style="height: 265px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;" data-pen-title="HTML List Demos">
  <span>See the Pen <a href="https://codepen.io/matt-west/pen/DCEzd">
  HTML List Demos</a> by Matt West (<a href="https://codepen.io/matt-west">@matt-west</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://cpwebassets.codepen.io/assets/embed/ei.js"></script>
</figure>

</details> -->


<!-- <details>
<summary>Call your homepage <strong>index.html</strong></summary>
<p>When you make your site live through GitHub Pages, the default URL you'll get is https://{username}.github.io/{reponame}. If you open that address, it will display one of two things: index.html or README.md.</p>
<p>If your index.html file is directly inside your docs folder, you're good to go! But if it's inside a subdirectory, you're going to see the README at that address – which will consist, if you haven't seen this yet, of instructions for how to host your site on GitHub Pages. You can add a subdirectory or alternate filename to the end of the URL, like https://{username}/github.io/{reponame}/website/home.html, but it's a little less convenient.</p>
<p>So if you haven't yet done so, you probably want to move your files into the docs folder (not a subdirectory), and make sure your home page is called index.html, not home or mysite or welcome.</p>
</details> -->

<!-- Consider titles
<details>
<summary>Consider titles.</summary>

A title can provide a context, a clue, a genre, a commentary; it can add an extra layer to viewer expectations. In previous units, you were titling your entire project; for a website, every page has its own <code>&lt;title&gt;</code> element in the <code>&lt;head&gt;</code>, which will show up in the browser's tab. These titles <em>could</em> be the same for all your pages, but they could also vary. What text do you want on top of the window, to show users where they are?
</details> -->


<!-- Lowest linecount challenge
<details>
<summary>When you're ready for polish, take the lowest line-count challenge.</summary>

<p>This is primarily a polishing step after all your content and style is pretty much set – but it may also help you clarify what your HTML is really doing, which can in turn make it easier to style.</p>

<p>Do your CSS rules repeat each other? Maybe they can be combined. <ul>
  <li>Look for elements that all behave the same way, and give them a shared class.</li>
  <li>Remember that you can apply more than one class to the same html element, so you can make rules for shared attributes in one class and special cases in another.</li>
</ul></p>

<p>Does your HTML have lots of containers with only one element in them?
<ul>
  <li>Some containers are important for positioning, e.g. centering with a flexbox.</li>
  <li>Others, though, are unnecessary clutter: if you can "unwrap" the element and apply CSS rules directly to it, with no loss in function, go ahead and unwrap it. You can usually move classes from an outer element straight onto the inner one. See my <a href="https://pitt.hosted.panopto.com/Panopto/Pages/Viewer.aspx?id=9171fa85-be27-437d-99b9-acfa00f44a4f">demo video from last week</a> for an example.</li>
</ul></p>
</details> -->


<!-- Update your README
<details>
<summary>Remember to update your README.</summary>
Each folder in a repository can have one, but the <em>main</em> README.md file is the one at the repository root: that's what visitors will find when they first open your repo. So that's where you should have a brief description of your project... and may I also suggest an active link to your live website, if you have one?
</details> -->

## Gathering questions

As you finish taking in the advice of your peers (and going over my suggestions above), I'd like to know **what questions you have that I might be able to help with** – especially if it's about something you've seen in assigned readings or revision suggestions, but you're not sure how to implement.

<div class="alert alert-success">
Head into <a href="http://bit.ly/cdm{{site.course.slugterm}}-notes">the google doc</a> and write down what you're thinking about. It can be anonymous!</div>

I'll float and respond to in-person questions, as usual, but when I have some down time I'll also come back to these questions in the gdoc and write up responses.


## Studio Time!
### Check for new feedback

Please **open up your website repo, head into the history, and see if you have any unread comments there.**

Hopefully everyone has by now received at least 2 (ideally 3) comments from members of your workshop groups! **If you have not, please let me know**, so I can make sure you've got a diverse set of perspectives on your work in progress.


### Set an intention
As usual, before you start, <a href="http://bit.ly/cdm{{site.course.slugterm}}-notes">go to the next section of the google doc</a> and write a quick line about what you hope to accomplish with your remaining time. e.g. Will you...
  <ul>
    <li>Work on responsive layout?</li>
    <li>Work on replacing placeholder content with real content?</li>
    <li>Work on one of the suggestions above? (Which?)</li>
    <li>Work on one of your stretch goals? (Which?)</li>
    <li>etc etc</li>
  </ul>
Just a sentence or two as a guidepost will give you something to come back to, to reorient, if you find yourself walking in circles or caught in a thicket.

<div class="alert alert-success">
Don't forget to save periodically as you go:
 <ul>
   <li>as an html / css / js file</li>
   <li>as a screenshot</li>
   <li>as a git commit, saying what you've just achieved</li>
 </ul>
</div>

### Work Time
Please ask questions as they come up. Otherwise, I'll try to work through the questions from the doc.


### Exit Note
Before you leave, as a way for me to check in, I'd like to hear more about what happened today: did you find images? Level up on a particular CSS skill? Decide something about your project? Raise a question in a new way that you'd like some help with?


# Homework for next time

* Continue revising forward on your website, aiming to **push a finished-for-now version by 10pm on Sunday, April 6** so you can submit a reflection to the <a href="{{site.github_url}}/issues">issue queue</a> by **noon on Monday, April 7.** This should include, as usual...
    - at least 500 words describing the work you did and the design decisions you made
    - at least two screenshots showing your work in progress
    - at least one screenshot of feedback that you responded to in revising, and what you did in response
    - your own assessment of how you met the baseline criteria, as well as aspirational criteria as appropriate
* The main goal of this deadline is to free you up to begin reflecting on the semester as a whole in our Consolidation/&#8203;Integration unit. That said, one of your possible projects for that unit is to continue working on a previous project.
    - If you anticipate that you'll want to just carry on with the website, that's fine! Please still turn in a reflection for Monday, noting that you're continuing to revise.

* Don't forget to **save, commit, and push as you go!**
