
# Lesson 10: Generative Studio

<section class="prereqs">
    <details><summary><strong>Texts to have read / listened to / watched</strong></summary>
        <ul>
            <li><a href="https://www.aiweirdness.com/an-exercise-in-frustration">An Exercise in Frustration</a>, by Janelle Shane</li>
            <li>the anonymous <a href="https://www.facebook.com/groups/1404116417142065/posts/1459674184919621">Facebook post</a> Shane links to in the opening line</li>
            <li><a href="https://www.youtube.com/watch?v=w0quo4S8Oqw">Learn GIMP in 20 Minutes</a>, from Chris' Tutorials</li>
        </ul>
    </details>
    <details><summary><strong>Work to have achieved</strong></summary>
        <ul>
            <li>Download and install <a href="https://www.gimp.org/downloads">GIMP</a></li>
            <li>Post a reading-response to the <a href="{{site.github.issues_url}}/7">the Issue Queue</a></li>
        </ul>
    </details>
</section>


**Plan for the day**:

1. On AI and Editing
2. In-class exercises
    - extracting a figure from its background
    - from flat to layered
4. Open studio
    <!-- Option: try it again with a generated image. Option: start homework reading. -->
5. Homework for next time: design principles; proposal


## 1. On AI and Editing: takeaways and open questions from the forum

Josh noted that I didn't give you an AI-advocate voice, and that was an oversight. Mea culpa! But he also helpfully complicated the issue by reminding us that it's not an all-or-nothing proposition: genAI can produce _materials for human designers to work with and edit_.

Likewise, Grace gestured toward another tension, between achieving an artist's singular vision and making concessions to whatever the tool produces. Again, it's easy to imagine that one or the other will dominate, but I encourage you to live within the dialectic: whether working with AI tools or not, creative endeavors are often a push-and-pull between the initial idea and the ideas that emerge as you're writing, drawing, playing. It's that mid-ground tension that produces the best vibrations, I find.

This puts me in mind of something Weini wrote:
> AI is simply a tool that can improve efficiency and assist with tasks, but it cannot do the entire job for you. It still requires human creativity, judgment, and effort to achieve the best results.

<details><summary>Does anyone remember what I set as the genAI policy for this class?</summary>
    <p>In brief:
    <ul>
        <li>Acknowledge it</li>
        <li>Generate multiple responses to the prompt, so you have to make active choices</li>
        <li>Exercise your own judgment, and take your own responsibility</li>
    </ul>
    </p>
    <p>See <a href="../policies#on-artificial-intelligence">the Policies page</a> for more details and my reasoning.</p>
    <p>In the context of this assignment, you may want to generate some images if you're not finding what you were looking for in Flickr or Unsplash or wherever; but <strong>don't generate the <em>whole</em> visual argument – generate <em>assets</em>, and edit from  there.</strong> Become the capable editors the FB writer was looking for, rather than the hapless prompters who can't revise.</p>
</details>

There were lots of other insightful posts. Any other questions or takeaways that you wanted to discuss?



## 2. In-class exercise: into GIMP

Now that you've had a tour of the software, it's time to play around with GIMP for yourselves and see what it and you are already capable of.

I've got two main ideas for what you might do:

1. Practice extracting images from their backgrounds, and
2. Open one of the finished visual arguments from last class, to see how it was done.

But once you've done those, the rest of the time is Open Studio: find and watch tutorials, start the homework reading, experiment with image generators, have some fun! Feel free to post your own work to your in-class-exercise folder, but please _don't_ post anything that you don't have license to distribute... including especially past students' work.


### 2a. Extract foreground from background

The idea of this exercise is to practice extracting an image from its context, so you can repurpose it in another context. To save time finding images to work with, I've bundled a few for you in your visual-argument-2025spring repos: look for the "in-class-exercise" folder, which includes instructions as well.

<aside class="alert alert-white">Note that when a repo's subfolder has a README, the GitHub website will also display that when you open the folder.</aside>

Since you'll be working locally, though, not through the website, for convenience, I'll reproduce the heart of those instructions here.

 **To begin, expand the zipped archive (images.zip) to find a set of five images to work with.**

Starting with the image of a hot-air balloon (beverly-and-pack--fly-me-to-the-moon.jpg), **experiment with GIMP's tools to select just the balloon** – or just the moon, etc. Once it's selected, you can copy it and paste it into a new layer – or into an entirely different file – where it can be resized, repositioned, recolored, and so on.

<details open><summary>A few options to consider for selecting</summary>
    <ul>
        <li><strong>Scissors select</strong> (edge detection). Using a series of single clicks, trace your way around the border between the foreground and the background. If the contrast is high enough, GIMP should automatically curve the selection lasso along the boundary line.</li>
        <li><strong>Fuzzy select</strong> ("magic wand") to detects contiguous pixels or <strong>Color select</strong> for non-contiguous pixels, but both based on color similarities. You can adjust the sensitivity (ie. how similar is "similar"?) in the tool options pane. It's often particularly useful to select a relatively monochrome <em>background</em>, allowing you to then Invert Selection to extract a foreground object.</li>
        <li><strong>Additive/subtractive selection</strong>. With all the select tools, you can hold down combinations of control, shift, and alt/command to change whether you're <em>replacing</em> an existing selection (the default), <em>adding</em> to it, <em>subtracting</em> from it, or finding the <em>intersection</em> between old and new. Try it with the <strong>shape select</strong> (i.e. rectangle or ellipse) and <strong>free select</strong> (lasso) tools – or with either AI-assisted tool above – to iteratively get closer to the selection you want.</li>
    </ul>
</details>

<div class="alert alert-info">
    NB: Because you can edit selection anchors until you're satisfied, you'll want to <strong>press Enter</strong>, double-click inside the selection, or switch to another tool <strong>to confirm the selection.</strong>
</div>

<aside class="alert alert-white">
If you're a more visual learner and want to see some options in video form, check out <a href="https://www.youtube.com/watch?v=lOzSiOIipSM">5 Ways to Remove a Background with GIMP</a> from Logos By Nick (runtime 6:42).
</aside>
Once you have your selection, you can...

* Copy and paste to create a new "floating" layer
* Click the green page button to secure more permanent status for that new layer
* Play around with sizes and colors
    - NB: This is a *raster* editing program, so once something gets smaller, you can't guarantee you'll be able to make it bigger again: pixels get thrown away.
    - It's often a good idea to **resize a copy** until you find the right position and size, and then move the original directly into that desired destination.
* Paste into a new file
* Paste as a repeating pattern

There's quite a bit more, of course, and I encourage you to find tutorials for any task your imagination suggests to you! I've linked to some on the [../resources] page, but there are a great many more only a search-engine away.


### 2b. From flat to layered

Each of the projects I linked to in our last class was in a repository, where you can also find a .xcf GIMP project file (or, in one case, a .psd Photoshop file). <strong>Choose one</strong>, download the file like we did for the [audio workshop](lesson-07), and open it up in the appropriate software.

Consider:

* How did they organize the layers?
* Try turning the visibility of layers on and off to appreciate how they created the attentional effects you noticed last time.

Options:
<ol>
    <li><a href="https://github.com/ktdemay/visual-argument-2020spring/blob/master/future.xcf">The Future of Sports</a>, by Kevin DeMaioribus</li>
    <li><a href="https://github.com/csk32/visual-argument-2020fall/blob/master/Human_Trafficking_updated.xcf">Human Trafficking</a>, by Christianna Kelley</li>
    <li><a href="https://github.com/fathimashabnam/visual-argument-2019fall/blob/master/VisualArgument.xcf">The Extinction Crisis</a>, by Fathima Shabnam</li>
    <li><a href="https://github.com/emmaknaub/visual-argument/blob/master/visual_argument.xcf">Radiate</a>, by Emma Knaub</li>
    <li><a href="https://github.com/anayoungblut/visual-argument-2023spring/blob/main/FINAL/visual%20argument%20FINAL.psd">Don't Do It</a>, by Ana Youngblut</li>
    <li><a href="https://github.com/suchiattota/visual-argument-2023spring/blob/main/TheCoverUp.xcf">The Cover-Up</a>, by Suchi Attota</li>
</ol>

## Open Studio

This is your time: find and watch tutorials, start the homework reading (or writing), experiment with image generators. Have some fun!

<div class="alert alert-success">As always, please set yourself a <a href="http://bit.ly/cdm{{site.course.slugterm}}-notes">studio goal in the doc</a>; at the end of class, I'll ask you to write a brief exit note on what you were able to achieve / what your next steps are.</div>



# Homework for next time:

The main thing will be to write a proposal for your unit project, but first, some design theory and examples!

* **Read** the following articles, each from a series on design principles in _Smashing Magazine_:
    - [Improve Your Designs With The Principles Of Similarity And Proximity (Part 1)](https://www.smashingmagazine.com/2016/05/improve-your-designs-with-principles-similarity-proximity-part-1/), by Jon Hensley
    - [Improve Your Designs With The Principles Of Closure And Figure-Ground (Part 2)](https://www.smashingmagazine.com/2016/05/improve-your-designs-with-the-principles-of-closure-and-figure-ground-part-2/), by Jon Hensley
    - [Design Principles: Compositional, Symmetrical And Asymmetrical Balance](https://www.smashingmagazine.com/2015/06/design-principles-compositional-balance-symmetry-asymmetry/), by Steven Bradley
    - [Design Principles: Dominance, Focal Points And Hierarchy](https://www.smashingmagazine.com/2015/02/design-principles-dominance-focal-points-hierarchy/), by Steven Bradley
* **Review** the unit-assignment [goals and options](https://github.com/benmiller314/visual-argument-{{site.course.slugterm}}#project-2-visual-argument--rhetorical-collage) for the rhetorical collage / visual argument, including the current baseline requirements and the Parachute Prompts if you're not sure what to propose.
* **Write** a project proposal, thinking in words about what you'd like to make:
    - What idea or argument will you try to present to or illustrate for readers? Or, at least, what is the triggering idea (starting point) of that argument or idea? What intervention will you try to make?
    - Include or link to a **prospective assets list**, i.e. a table of the images you think you'll need and where you might be able to source them. You can choose to include that assets list in the proposal or place it as a file in your repository, to more easily track changes.
    - **Link to your project repository,** so it's easier to find when we get to group work.
* **Post** your proposal to the appropriate forum on the [Issue Queue]({{site.repo_url}}/issues).
