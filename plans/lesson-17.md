
# Core Concepts of HTML & CSS + Studio

<section class="prereqs">
    <details><summary><strong>Texts to have read</strong></summary>
    <ul>
        <li>Kevin Powell's <a href="https://learn.kevinpowell.co/course/html-css-for-absolute-beginners">HTML & CSS for absolute beginners</a>, up through the end of the <a href="https://learn.kevinpowell.co/course/html-css-for-absolute-beginners/3-css/1-what-is-css">CSS module</a><ul>
            <li>If you were unable to log in, you could also have done <a href="https://internetingishard.netlify.app/html-and-css/">Interneting is Hard (but it doesn't have to be)</a>, up through <a href="https://internetingishard.netlify.app/html-and-css/hello-css/">"Hello, CSS"</a></li>
            </ul>
        </li>
    </ul>
    </details>
    <details><summary><strong>Work to have achieved</strong></summary>
    <ul>
        <li>Push your tutorial code to GitHub</li>
    </ul>
    </details>
</section>


**Plan for the day**:

1. Tutorial check-in (~10 min)
    - Who used which tutorial?
    - Compare your results so far, discuss design choices & challenges
2. Alt text activity (~20-30 min)
3. Designing with dev tools (~10 min)
4. Studio / practice (~30 min)


## 1. Tutorial check-in

First question: was everyone able to log into the Kevin Powell site eventually? If not, who used Interneting is Hard?

What I mostly want to do here is give you a chance to compare notes, and especially to **compare the tutorial-led websites you've been building so far**. Working in pairs or groups of 3, show each other what you've built:

* What choices have you made in implementing the design spec in the Powell tutorial? Or what modifications have you made (if any) from the basic instructions in Interneting is Hard?
* Is there anything you were _not_ able to achieve? See if you can figure it out together, and call me over if you need help. <!-- in particular: was everyone able to link to a separate stylesheet? did you successfully use a *relative path* to your stylesheet? discuss what could go wrong if you use an absolute path. -->

Let's take about 5-10 minutes here; any remaining questions you have, you're probably not alone, so let's talk about them together!

## 2. Alt text activity

As you should know by now, **every `<img>` on the web requires `alt=""`**. As this [guide from NCSU libraries](https://www.lib.ncsu.edu/accessibility-guide/alt-text) explains,

> Good alt text describes **what is in the image**, focusing on what is most relevant to **the reason for including the image** and has the following properties:
>
> * it is as concise as reasonably possible
> * it relates to the surrounding content of the page without being repetitive
> * it avoids relying only on “sensory characteristics” to convey meaning
> * its writing style is consistent with the writing style of the page
>

Notice that this emphasis on reasons and reasonability mean that context is really important – so it's hard to rely on an AI alt-text generator, even as they're getting better. Your human sense of purpose is part of what you're doing here.

A few relevant metaphors: writing a text description of an image is kind of [like leading a Dungeons & Dragons campaign](https://ericwbailey.website/published/dungeons-and-dragons-taught-me-how-to-write-alt-text/ "thanks to Powell for this recommended reading!"), trying to bring readers/listeners along on a shared adventure; it's also a bit [like poetry](https://alt-text-as-poetry.net), trying to convey a wealth of subjective meaning using condensed, expressive language. <!-- look for an example or two of color descriptions based on associations -->

The authors of the latter site also point out that alt text is a kind of _translation_: it always involves creative decisions, with no single correct answer, and you have to recognize that something will always be lost – but ideally something will be gained as well.

### Practicing together

I'm going to pull a random image or two from [unsplash](https://unsplash.com), but let's recognize that we'll need to imagine an artificial context. Some shout out if you see an image that starts to tell a story for you, and we can get it into our notes doc and write a few  descriptions for it.
<!-- NOTES AFTER 2025 SPRING: Don't do rando unsplash, use the images from the Bouldering website. Start by having everyone list their descriptions in the gdoc, and look for what changes. Use those to talk about what different shades they fill in or leave out. Ask: why does it matter that ___? Does it matter? What does it add? -->

### Practicing in pairs – and on your own
<!-- NOTES AFTER 2025 SPRING: this will work better as a callback exercise when students have their own images. Or ask them to choose some as part of the homework. -->

1. Working in groups of two, repeat the process: find a picture that suggests a context for you, that you could imagine writing alt text for.

2. **Working solo first,** write a text description of the image, keeping your context in mind.

3. Compare descriptions. What differences did you notice? What similarities?

EXT: waiting for the others? Repeat the process, using pictures from your own camera roll. What do you emphasize when describing your own picture that your neighbor did not?

### Full-group discussion

* What surprised you, or what do you most want to remember from this experience?
* How did/does subjectivity enter into text descriptions? In what contexts does that feel most or least helpful?

Let's get some notes in the shared doc.


## 3. Designing with dev tools

Toward the end of the CSS module, Powell shows you how to use your browser to look for broken CSS rules. Did you know you can also use those tools to make changes on the fly?

**Let's have a look at the CSS Zen Garden, stripped of its CSS.** (You can also [download this HTML file](https://www.csszengarden.com/examples/index) from https://www.csszengarden.com/.) <!-- NOTES AFTER 2025SPRING: That would have worked well for the first intro to HTML, but now it just felt weird and rushed and not related to what they'd done in the tutorial. Instead, again, inspect and modify *the tutorial site*: demo some of the quick changes you'd make to any site. Change font-color to #333 so it's not harsh black and change background-color to #ccc so it's not harsh white... then revert that for h3. Change font-family to sans-serif.  -->

* You can see how the HTML relates to what's displayed
* You can add rules for the currently selected element
    - NB: it will use the most specific selector available, which may not be what you want. We can come back to that.
* You can edit existing rules to see what changes.
* You can see the full list of rules we've applied: it's actually a new stylesheet!
* If you don't save (rules from) the inspector stylesheet, those rules will be lost when you refresh the page.

### Your turn (~5 min)

You probably already have this lesson plan open; if not, go ahead and open it now.

* Fire up the Chrome or Firefox inspector and explore the rules I already have in place.
* Make some changes and see what happens. :)
* If you have some new CSS you'd like to propose I adopt, please do send them my way!

<aside class="ext">
    <p>EXT: Open up the example sites from last year (from HW reading, and pasted again below for convenience), looking at the HTML with either View Source or your browser's inspector. How are the pages structured? Any surprises? Any changes you'd want to make? Anything you'd want to borrow for your own site?</p>

    <details><summary>Convenient links</summary>
        <ul>
            <li> <a href="https://fatemaquaid987.github.io/website/index.html">Fatema Quaid</a>, by Fatema Quaid</li>
            <li><a href="https://cmgo412.github.io/website-portfolio-2021spring/">Hi, I'm Caela</a>, by Caela Go</li>
            <li><a href="https://cap-alt-delete.github.io/website-portfolio-2021spring/">Loose Leaf</a>, by Lynn Priestley</li>
            <li><a href="https://shreyababu.github.io/website-portfolio-2020fall">The Rwandan Genocide: 100 Days of Silence</a>, by Shreya Babu</li>
        </ul>
    </details>
</aside>

## 4. Studio / Practice (45-60 min)

<div class="alert alert-success">
See below for options, then please go to <a href="https://bit.ly/cdm{{site.course.slugterm}}-notes>our notes doc</a> and let me know what you're working on; this helps me figure out where I can be most helpful.
</div>

1. **If your tutorial pages aren't looking like the examples, tell me now, so I can help you get there!** You'll get a lot more out of the later tutorials if you've got these first ones solidly under your belt.

2. The assignment for next class includes another two chapters in the tutorial and some optional texts on more advanced CSS selectors. If you haven't yet gotten that far, why not start those homework assignments?

3. How would you describe your own visual unit project if presenting it as alt text? Work up a couple options.

4. If you're feeling good about all that, start translating your website sketches – especially your website *content* – into HTML and then CSS.
    - Begin by adapting the tutorials, once you know you've got them working, to include your own materials: first build out the HTML tags you think you'll need, so you're sure they open/close appropriately, then write your content into the tags.
    - Use the _docs_ folder for files you'll eventually want to publish on the web.
    - Call the file for your landing/home page **index.html**. You can always change the `<title>`.

4. Above all, call me over for help as needed.

EXT: If you've already done the above, and you're good on what a CSS class is, and how to add it to an HTML element, read up on [CSS frameworks]({{site.github_url}}/resources#frameworks) on our course Resources page. They're basically a bunch of pre-created CSS classes you can use to design your own layout from scratch: a little like Lego for web design. (I use the Bootstrap framework on this site.)


## Homework for Next Time

* **Work through** more of the [HTML & CSS tutorial](https://learn.kevinpowell.co/course/html-css-for-absolute-beginners):
    - [Module 4: The box model](https://learn.kevinpowell.co/course/html-css-for-absolute-beginners/4-the-box-model/1-everything-is-a-box)
    - [Module 5: Selectors, Specificity, and more styling](https://learn.kevinpowell.co/course/html-css-for-absolute-beginners/5-selectors-specificity-and-more-styling/1-time-for-version-2)
* NB: If you still can't get in to that tutorial, the equivalent sections from Interneting is Hard are [The Box Model](https://internetingishard.netlify.app/html-and-css/css-box-model/) and [CSS Selectors](https://internetingishard.netlify.app/html-and-css/css-selectors/)
* _Optional EXT:_ Want to get deeper?
    - See if the old tutorial's page on [Web Typography](https://internetingishard.netlify.app/html-and-css/web-typography/) is up and running
        - Remember your resources on fonts from the previous unit? They can help you here, too!
    - Read more about [how CSS selectors work](https://css-tricks.com/how-css-selectors-work/)
    - Try loading and clearing plates at the [CSS Diner](https://flukeout.github.io/).
* Save and commit as you go!
