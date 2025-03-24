
# Web Unit Studio / Accessbility and Layout

<section class="prereqs">
    <details><summary><strong>Texts to have read</strong></summary>
        <ul>
            <li>Kevin Powell's video on <a href="https://www.youtube.com/watch?v=VQraviuwbzU&list=PL4-IK0AVhVjM6kuUoUexfmnD8vHtZkXdd&index=4">5 simple tips to making responsive layouts the easy way</a></li>
            <li>Tutorials (<a href="https://learn.kevinpowell.co/course/html-css-for-absolute-beginners">Powell</a> or <a href="https://internetingishard.netlify.app/html-and-css">Interneting is Hard</a>) up through CSS selectors and Box model</li>
        </ul>
    </details>
    <details><summary><strong>Work to have achieved</strong></summary>
        <ul>
            <li>Compose and push a <em>first preview draft</em> of your <a href="https://github.com/benmiller314/webs2025spring#deadlines-and-products">website portfolio project</a>: mobile-first content, minimal styling, to get the gears turning. This should include:
                <ul><li>A multifile <strong>project folder</strong> – probably the pre-built folder named <code>docs</code>, for ease of use with GitHub Pages – containing a combination of HTML and CSS, even if it's not well-developed.</li> <li>A static <a href="https://www.take-a-screenshot.org/">screenshot (.png or .jpg)</a> of your <strong>website-in-progress</strong>, as rendered in a local web browser (for comparison later to subsequent drafts: this is your "flat" export).</li><li>A <a href="https://www.take-a-screenshot.org/">screenshot</a> of your <strong>text editor setup</strong>, too, with the navigation pane showing: this can sometimes help me give feedback more quickly.)</li><li> At least an initial update to your README.md file, introducing your site (as opposed to this assignment). Feel free also to ask questions or lay out next steps for yourself!</li> <li>An updated list of <strong>assets</strong>, now with any files or fonts you've actually obtained. As you go, add TASL documentation for any outside sources – title, author, source (e.g. url), and license (e.g. Creative Commons, fair use rationale).</li></ul>
            </li>
        </ul>
    </details>
</section>

**Plan for the day**:

1. Accessibility checks: check on your own, work with a neighbor to fix what needs fixing
    * document outline
    * alt text
    * contrast ratios
2. Thoughts for studio
3. Studio: toward a laid-out second preview
    * Set Goals
    * Go forth!
    * Exit note

## 1. Accessibility checks

The best way to make sure you're building a website that people can access is to work with accessibility in mind from the beginning, and checking periodically along the way. We already talked about alternative text representation of images: every image needs to declare alt text, or leave `alt=""` to signal that the image is purely decorative. We also talked about the importance of a sensible document outline, created by heading levels, with exactly one `h1` and levels governed by content, not appearance. Another is contrast: the Web Content Accessibility Guidelines (WCAG) recommends a minimum luminosity ratio of 4.5:1 between text and background, and ideally the ratio is even higher: 7:1.

Today I want to introduce a tool you can use to catch yourself making mistakes – or doing well! – with these and other accessibility concerns. It's called the Web Accessibility Evaluation Tool, or WAVE, and you can find it at **[wave.webaim.org/](https://wave.webaim.org/)**.

There, you can [download an extension or add-on](https://wave.webaim.org/extension/) for either Chrome or Firefox (or Edge) that will run a quick inspection of the current page your browser has open – including local pages.

<div class="alert alert-success">
Please take a minute to install the plugin on your browser of choice, if you don't already have it.
</div>

UPDATE: To make this work with local files, you'll need to change the permissions of the extension. After installing, right-click on the icon and choose "manage extension" (or the equivalent for your browser). A new page will open with options; look for "Allow access to file URLs" and toggle that to _on_.

### Quick demo

I'll give you a brief tour, using my own site.

* Errors, alerts, and features
* Page structure
* Reading order
* Contrast errors

### Your turn!

Start by analyzing the preview draft you brought in for today. What's working? What do you need to fix?

Then share your findings with a partner. Work together to celebrate your wins and correct any outright errors.


## 2. Thoughts for studio

Keeping it brief this time:

* After your accessibility check, layout is probably next: start with tonight's HW reading / tutorials.
* NB: You may need to add HTML to achieve your layout, because you may need containers or groups. Divs can act as a first pass for both those things! But sometimes a semantic element like `main`, `section`, `article`, etc is a good improvement on a generic div.
* Some layouts take several rules to get working. **Don't panic; work iteratively.** Stuff may look weird for a sec (as when you first turn on flexbox) – or nothing may change at first (as when you first turn on grid).
* Use your commits to give yourself safe-spots in history, where you know it's not broken; then press forward.



## 3. Studio: toward a laid-out second preview

### Set Goals

As usual, please write down some goals in the [shared google doc](https://bit.ly/cdm{{site.course.slugterm}}-notes), **setting a concrete plan for today**: what do you need to do to level up on HTML, CSS, and resource gathering to move toward your specific project?

<div class="alert alert-info">
For my sake and yours, <strong>please be as specific as possible:</strong> e.g. rather than “working on my site,” you might say, “choosing images for photo gallery” or “building grid for layout with top menu and featured image” etc.
</div>

EXT: *Already feeling done?* Ask yourself:

- Are you repeating the same CSS rule in multiple places? Instead, see if you can reuse CSS classes in multiple places, extending them where you need to.
- Does that div need to be there? If it's not for layout or semantic grouping, it might not be necessary: remember that you can apply classes directly to elements.
- Do you have style or presentation directly in the HTML? See if you can extract it out to the stylesheet for consistency, flexibility, and ease of maintenance.
- Would it help to define colors relative to starting values? See [css-tricks.com/a-complete-guide-to-custom-properties/](https://css-tricks.com/a-complete-guide-to-custom-properties/).

### Go forth! And Don't forget to document your process

<div class="alert alert-success">
Don't forget to save periodically as you go:
 <ul>
   <li>as a project file</li>
   <li>as a screenshot, showing your process</li>
   <li>as a git commit, saying what you've just achieved</li>
 </ul>
</div>

### Exit note

Before you leave, just as a way for me to check in, I'd like to hear more about what happened today: Did you decide on your navigation? Block out the html? Make some progress on a stylesheet? Work through a tutorial or two (and which)?

<strong>Reply to your note in the <a href="http://bit.ly/cdm{{site.course.slugterm}}-notes">google doc</a>.</strong>

## Homework for next time

1. **Work through** a tutorial on layout:
    - Kevin Powellists, do [Module 6: Layouts](https://learn.kevinpowell.co/course/html-css-for-absolute-beginners/6-layouts/1-creating-layouts-with-css).
        - NB: when you get to the section on [Flexible layouts with Flexbox](https://learn.kevinpowell.co/course/html-css-for-absolute-beginners/6-layouts/5-flexible-layouts-with-flexbox), there's a typo in the first interactive code block: he says there are two layouts, one using grid and one using flex, but the HTML only has one. You can fix it with a little copy-paste! Just edit the class on the outer `div` so you have one `<div class="flex">` and one `<div class="grid">`.
    - If you've been doing Interneting is Hard, skip the layout chapters and instead **read** two pieces by Josh Comeau:
        - [Interactive Guide to Flexbox](https://www.joshwcomeau.com/css/interactive-guide-to-flexbox/) and
        - [Interactive Guide to CSS Grid](https://www.joshwcomeau.com/css/interactive-guide-to-grid/).
        - NB: if Comeau's page on Flexbox feels too abstract, try [MDN's flexbox intro](https://developer.mozilla.org/en-US/docs/Learn_web_development/Core/CSS_layout/Flexbox) instead. But please do use Comeau's intro for Grid; it's one of the best I've seen.
2. Everyone will also probably benefit if you **watch** Powell's [Useful & Responsive Layouts, no Media Queries required](https://www.youtube.com/watch?v=p3_xN2Zp1TY) (11:02 runtime at full speed).
    - It's got a bunch of ready-to-roll layout solutions that will apply broadly. Do the reading above first, though: it will make much more sense if you're already familiar with Flex and Grid layouts.
3. Armed with all that info, **compose and push a _second preview draft_**, now adding or updating layout for larger screens (i.e. desktop).
    - On Wednesday we'll talk about criteria and aspirations, getting ready to spend next Monday workshopping your full website drafts.


* EXT for enthusiasts:
    - If you're doing Powell's tutorial, check out the two Josh Comeau resources above, which get into more depth than Powell's Layouts chapter does.
    - If you haven't yet done so, try the MDN Test Your Skills pages for [Flexbox](https://developer.mozilla.org/en-US/docs/Learn_web_development/Core/CSS_layout/Flexbox_skills) and for [Grid](https://developer.mozilla.org/en-US/docs/Learn_web_development/Core/CSS_layout/Grids).
    - Want even *more* layout templates and examples? Try Rachel Andrew's [Grid By Example](https://gridbyexample.com/patterns/), which also has video tutorials.
