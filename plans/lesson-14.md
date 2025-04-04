# Visual Unit Studio 2

<section class="prereqs">
    <details><summary><strong>Work to have achieved</strong></summary>
        <ul>
            <li>An optional short <a href="{{site.github.issues_url}}/9">blog post about possible consolidation-unit projects</a></li>
            <li>Work in pursuit of a final visual argument / rhetorical collage</li>
        </ul>
    </details>
</section>

**Plan for the day**:
1. Guiding thoughts for Studio (5-15 min)
2. Set intentions
3. Studio time!
4. Exit note


<div class="alert alert-success">
<strong>Today is all about working on your individual projects!</strong> Layer images, apply effects, watch relevant tutorials. I know your lives are busy; take advantage of this dedicated time free from other distractions and obligations to move your piece forward.
</div>

At the same time, it's worth noting that you're working **in a shared space**, in a studio. If you have questions, or you want feedback on something, you have your classmates and your instructor on-hand.



## Guiding thoughts for Studio (5-15 min)
Some seeds of revision possibilities I want to plant, based on seeing the latest drafts (as of last night):


<details><summary>Consider naming and/or grouping your layers.</summary>
    <p>It's always a good idea to know what you're looking at! By default, both GIMP and photoshop will label a layer with whatever the file was called – and most of those names aren't especially helpful, let alone concise. So if you haven't yet, I highly recommend that you double-click the name of each layer and update it so you can tell, at a glance, which is which.</p>

    <p>This is especially important if you have a lot of layers. At that point, you'll probably also benefit from organizing them into groups, so you can do things to them all at once: move them, toggle visibility, apply effects and tools, etc.</p>
    <p>This is a matter of convenience in Photoshop, but in GIMP (at least before GIMP 3 is fully released), it's also the <em>only</em> way to operate on multiple layers at once. See <a href="https://docs.gimp.org/en/gimp-layer-groups.html">docs.gimp.org/en/gimp-layer-groups.html</a>.</p>
</details>

<details><summary>Help your text pop.</summary>

  <p>If you have text on your image, it can be tricky to get it to stand out against the background, especially if the background is multicolored. Luckily, in a digital medium, we can collaborate with the machine to get some automated help. Play around with Filters > Drop-Shadow, or even the <strong>Xach effect</strong> (a quick-hit combination of highlight and drop-shadow) as explained in <a href="https://www.youtube.com/watch?v=oJiesAV32-8">this tutorial</a>, among others. NB: this works by adding two new layers (a shadow, and a highlight), one of which is masked; you can change the order of layers to affect only the ones you want.</p>

  <p>There are lots of websites with more advice on drop-shadowing, so I recommend searching around for examples. Some key points:
    <ul>
      <li>The goal is contrast, so don't pick a shadow color that's too close to your text color – you especially want to change the <em>luminance</em> of the shadow relative to the text. Try giving the brighter color a luminance at least 4.5 times that of the darker color, using HSL color selectors.</li>
      <li>Blur works better on image backgrounds than on solid backgrounds where it's more noticeable.</li>
      <li>Drop-shadow works best on headlines / top-level text, and less well on paragraphs.</li>
      <li>If you need more contrast everywhere, try going more minimalist. In other words: reconsider whether that text needs that background. <a href="https://web.archive.org/web/20150201032136/http://overthinkingdesign.com/2015/01/when-to-use-drop-shadows/" title="including Jason Horst of Piksl Design, whose blog this link points to">Some have argued</a> that drop shadow is a "bandage" for bad design: that the real solution is to rearrange the layout so there's more contrast to begin with. Not always doable, but still: food for thought! </li>
    </ul>
  </p>
</details>

<details><summary>To integrate objects more fully into a scene, try adding shadows.</summary>

  <p>Without shadows, objects and images brought in as layers can sometimes feel two-dimensional, floating over the scene (or stuck onto it) rather than inside of it. Sometimes that's exactly what you want! But if you're going for the illusion that people or objects are in the same space, slanting shadows that react as if to a shared light source can add a great deal of polish and realism.</p>

  <p>Both GIMP and Photoshop come with automated drop-shadow effects (see above for one use, with text), but depending on what you're trying to add, <strong>you'll often get the best customization if you create a copy of your object to manipulate</strong>: painting it black, free-transforming it to the desired angle, and adding both blur and a gradient fade. I've found some good video tutorials for <a href="https://daviesmediadesign.com/project/create-a-realistic-shadow-for-objects-in-gimp/">creating realistic shadows in GIMP</a> and <a href="https://www.youtube.com/watch?v=5TuhBcN9k8w">creating realistic shadows in Photoshop</a>.</p>

  <p>And if you're trying to add text to a <em>curved</em> surface, you might be interested in related tutorials <a href="https://www.youtube.com/watch?v=Eg10xTOcrCM" title="Adding a label to a cylinder or can from Eli Afram's GIMP channel">in GIMP</a> and in <a href="https://www.youtube.com/watch?v=B0oqxV_lvf4" title="How to wrap text around a cylinder from 2 Minute Photoshop channel">Photoshop</a>.</p>
</details>

<details><summary>Consider using alignment tools and spacing to reinforce the design's cohesion.</summary>

  <p>As I hope you remember from the reading on <a href="https://www.smashingmagazine.com/2016/05/improve-your-designs-with-principles-similarity-proximity-part-1/#proximity">the gestalt principles of perception</a>, when objects' edges align, most viewers will treat them as related; if they're close-but-not-quite aligned, that feeling of not-quite-rightness may seep into viewers' first impressions of the design. (Note that this applies to symmetry, too: you can center or distribute things along a horizontal or vertical axis, and not just relative to the overall canvas.</p>

  <p>Both GIMP and Photoshop offer tools for aligning or distributing objects – which, in this context, usually means aligning <em>layers</em>. Here's the official <a href="https://docs.gimp.org/en/gimp-tool-align.html">GIMP documentation</a> and an <a title="which may share your frustrations" href="https://thegimptutorials.com/how-to-align-layers">outside tutorial</a>, plus the corresponding <a href="https://helpx.adobe.com/photoshop/using/aligning-layers.html">Photoshop documentation</a> and an <a href="https://jkost.com/blog/2021/10/align-and-distribute-layers-in-photoshop.html">outside tutorial there</a>, too, for good measure.</p>
</details>

<!-- <details><summary>Have a lot of content? Not sure where text could fit? Consider panels or frames.</summary>

  <p>This is related to the Gestalt <a href="https://www.smashingmagazine.com/2014/03/design-principles-visual-perception-and-the-principles-of-gestalt/#common-regions:~:text=%E2%80%9CElements%20are%20perceived%20as%20part%20of%20a%20group%20if%20they%20are%20located%20within%20the%20same%20closed%20region.%E2%80%9D">principle of common regions</a>. Much as a comic strip uses boxes to indicate a sequence of connected moments in time, you can divide your canvas into distinct areas, which can provide breath and space while preserving movement. There are several ways to define your areas: with distinct blocks of background image, color, or pattern; with a semi-opaque layer of white or black, acting like frosted glass over the layer below; or with positive-space images that cut between one chunk of the image and another.</p>

  <p>The same approach can also give you the effect of a museum poster, where the main image is framed as a single panel, with an off-image description delineated by a full-width rectangle (or full height, for a sidebar) of contrasting background. (Solid white or solid black often work well to signal "I'm not the image.") This technique can be useful for adding a clarifying slogan or title to an image, without messing up your existing design hierarchy.</p>

  <figure><img src="https://ctl.s6img.com/society6/img/UBgJ7V-HVB_yaJ_z3jEuYwf2Hlo/w_700/posters/top/~artwork,fw_2718,fh_3618,fy_-3,iw_2718,ih_3623/s6-original-art-uploads/society6/uploads/misc/a5494e8a55c24a1090059d40a7ba40c3/~~/vincent-van-gogh-art-exhibition3045631-posters.jpg?wait=0&attempt=0" alt="Van Gogh at Arles, 1984 Met Museum: poster with text outside the image on plain white background"><figcaption>My parents totally had this poster in the 1980s. Apparently they're being <a href="https://society6.com/product/vincent-van-gogh-art-exhibition3045631_poster">reprinted now</a> for some reason?</figcaption></figure>
</details> -->

<details><summary>Consider pointing viewers toward a follow-up.</summary>

    <p>Many of you are trying to get viewers to take an action; if you haven't yet, consider giving them a place to go to get involved, or to get more information. Make this link large enough to be easily readable, even though it probably won't fall at the top level of your visual hierarchy (because it makes more sense as the last thing, rather than the first thing, they see). Some of you are already doing this, which is awesome!</p>

    <p>Even if you don't have such a call to action in your visual argument, you might want to add an unobtrusive link to your credits file on GitHub – e.g. in a small font-size along the border. This would serve as a compromise between filling a sidebar or footer with all the required attributions for your Creative Commons images (though that may be fine, too, depending on your design) and not actually making those names available – which would be a violation of the CC-BY and related licenses.</p>

    <p>If you're wondering, "what border?" remember that you can always adjust the Image > Canvas Size to add a small extra strip along the bottom. If you give it a simple contrasting background, it should feel like it's outside of the image, rather than messing it up.</p>

    <p>NB: A link shortener like <a href="http://bit.ly">bit.ly</a> or <a href="http://ow.ly">ow.ly</a> may help to keep this kind of link subtle enough to not detract from your design. If you create a login, you can even customize the link.</p>
</details>

<details><summary>Don't forget your required README updates – and consider adding a title there.</summary>

    <p>Part of the draft requirements due on Monday was "an updated README.md file, introducing the Visual Rhetorical Argument to an audience beyond our class." When peers and future portfolio perusers land on your repository, they shouldn't see my assignment first thing (though you can always move it to a new file, like we did together in the audio unit). Instead, <strong>they should see an introduction to the repo's contents</strong>, which is to say, an introduction to your project.</p>

    <p>Some of you are doing great things with your Markdown: building tables of assets and their TASL information, adding hyperlinks to particular files in the repo, posting periodic updates on project progress, even keeping lists of the specific tools you're using and why (and, sometimes, with what settings).</p>

    <p>Another thing you might want to do in a README is give your project a name beyond "visual argument." <strong>A title can provide a context, a clue, a genre, a commentary</strong>; it can add an extra layer to viewer expectations. What will you call yours?</p>

    <!-- <p>Not sure where a title would go? Think of placards in museums: alongside the image is pretty common. You can put the title in your README. Sometimes the title is obvious from the image itself; sometimes it's not. Likewise, ad campaigns often have titles, even if they're not referred to in the ads themselves.</p> -->
</details>

<!-- <details><summary>Articulate permissions.</summary>

If you're using images you didn't make yourself, be sure to include enough information to recover where it came from: a direct link to the image and to the specific license (if there is one) is ideal. Where to do this? Ideally, somewhere small in the image file itself: along a border, say, in a 10-point font. If you have a lot of images, and can't fit the credits on your image even with a small font, you can instead link to a file in your repository. Link shorteners, like ow.ly and bit.ly, will help here.

<em>NB: If an image is under copyright, you can still use it if you can make a good case that it's a Fair Use.</em>  See _Writer/Designer_ page 156 to review the Four Factors you need to consider.
</details>


<details><summary>Remember that scaling down is easier than scaling up</summary>

<p>We talked about this a bit at the start of the unit, but it may bear repeating: both GIMP and Photoshop deal primarily in pixels, not vectors. (For vector graphics, try Inkscape and Adobe Illustrator.) So when you scale down an image or text, the software throws away the pixels it no longer needs; but if you then scale back up, it has to guess about what could fill in the gaps, and usually you'll get a blocky, pixellated appearance. Unless you're going for a Minecrafty look, that's probably not what you wanted.</p>

<p>If pixellation happens to you, take note of the final size you settled on, then re-import the image (or re-place the text) at higher resolution, and scale directly to the size you now know you need.</p>

</details>
-->
<!--
<details><summary>If your effects aren't showing up, try increasing the layer size.</summary>

Sometimes GIMP seems to promise the world, but when you apply the effect, it's like nothing happened. In these cases, it's often possible that you're just reaching past the edge of your workspace. See whether you get better results after Layer > Layer to Image Size (or give yourself more room overall with Image > Canvas Size).
</details> -->

<!-- <details><summary>Consider whether you have enough screenshots.</summary>

    <p>Think about what moments are worth remembering as you go: where did you level up, or realize something, or get stuck? Take a <a href="https://www.take-a-screenshot.org/">screenshot</a> in the moment, so you can refer back to it in your reflection.</p>

    <p>This is particularly important if you're not using GIMP: I'd like to know what about the workflow of the program you're using is especially compelling. Screenshots of work-in-progress (or even short gifs, which you can record using the strangely named <a href="https://www.cockos.com/licecap/">LICEcap</a>) will be really helpful to me in understanding how your project moves through the software at key junctures. It could also help your peers, and possibly your own future-self, too.</p>

</details> -->


## Okay, now go to!


<p>As usual for studio time, please <strong>set a daily goal</strong> in the <a href="http://bit.ly/cdm{{site.course.slugterm}}-notes#heading=h.ema3504c3kf3">shared notes doc</a>, both for accountability and so I can look for ways to help.</p>
<!--
Then **consult the clock and your partners**: leaving 5 minutes to return to the main room at the end of the class, do you want to set a couple 25-minute cycles and one 5-minute check-in? Three 15-minute cycles and two check-ins? One long work session with check-ins only for questions?

Make sure you agree, then start your timers (if you're using them). Each time you pause, ask yourself (or each other):

* What do you feel good about?
* What challenges came up?
* What questions do you have?

**You can find me in the main room, or call me in to your breakout room if you have a question in common**: just use the "Ask for Help" button ![ask for help button, which shows a question mark in a circle](https://assets.zoom.us/images/en-us/desktop/generic/in-meeting/ask-for-help-icon.png) in your meeting menu.
 -->


<div class="alert alert-success">
Don't forget to save periodically as you go:
 <ul>
   <li>as a project file</li>
   <li>as a screenshot, showing your process</li>
   <li>as a git commit, saying what you've just achieved</li>
 </ul>
</div>


### EXT: Feel like your project is finished, and not sure what to do?
1. Make sure everything's pushed properly to GitHub
2. Make some lists: things I have learned about GIMP/Photoshop/fonts; questions I have about GIMP/Photoshop/fonts; things I have learned about gestalt principles of perception; questions I have about gestalt principles of perception.
3. Work with the Internet, or peers, or me to answer the questions from step 2.
4. Write a draft of your reflection; remember that you still have time to revise, though.
5. Have a look at what your classmates have posted to the [issue queue]({{site.github.issues_url}}), looking forward to the integration/consolidation unit. Anything you're excited by? Anything you want to add?


<!--
<div class="alert alert-warning"><p>To get credit for asynchronous participation, <strong>add your working goals to the <a href="http://bit.ly/cdm2022spring-notes">google doc</a> when you start your session</strong>, set your timer, and when the bell rings, <em>add a brief reply</em> to your initial note with a status update. (This can be very brief.) Run through this cycle at least twice.</p>

<p>NB: To make it easier for me to find your additions to the doc, please use either Comments or Suggestion Mode.</p>
</div> -->


## Quick report back (with 5 min left)

Just as a way for me to check in, I'd like to hear more about what happened today: did you find images? Level up on a particular GIMP skill? Which ones? Decide something about your project (what was it)? Raise a question in a new way that you'd like some help with?

Take five minutes to reply to your own notes in <a href="http://bit.ly/cdm{{site.course.slugterm}}-notes#heading=h.ema3504c3kf3">shared notes doc</a>. If everyone finishes early, we can hear from a few volunteers out loud.



# Homework for next time

<div class="alert alert-danger">
No class next week: it's spring break!
</div>

* Aiming for 11:59pm on Sunday, **complete – at least for now – your visual argument / rhetorical collage.** Your repository (on GitHub or in a shared Box folder) should include:
    - Your most up-to-date layered _project file_ (.xcf for GIMP, .psd for Photoshop)
    - A series, now, of screenshots showing your _project workspace_ in progress
    - An _exported flat image_ (.png or .jpeg), for speedy previewing or as a backup should something go wrong with the project file
    - An updated list of assets reflecting what you actually used, including Title, Author, Source (a direct link if appropriate) and License (e.g. explicit licenses like CC or unsplash, or rationales for claiming fair use)
    - An _updated README.md file introducing your project to a new audience._ Go ahead and give your piece a title! Make it something to live beyond this assignment, if you can. :¬)
* By Monday at noon, **write a prose reflection** that incorporates images from your feedback and screenshots of your GIMP project. As explained in the [prompt for the assignment](https://github.com/benmiller314/visual-argument-{{site.course.slugterm}}#deadlines-and-products), this should include:
    - At least 500 words
    - Your own assessment of how you met the [baseline criteria](http://bit.ly/cdm{{site.course.slugterm}}-notes) and goals for the unit, as well as any aspirational goals as appropriate
    - At least one screenshot or blockquote of feedback you used (and please say how)
    - At least one or two screenshots of your work in progress (ideally, related to the discussion in the previous two bullets)
* **Post your reflection** to the course site's [Issue queue]({{site.github.issues_url}}), to make it easier to embed images.
    - If you want to then copy the source code into a file in your repo called reflections.md, or paste it down at the bottom of your README, it should have all your images embedded, too!
    - If you feel strongly that you'd rather keep your reflection private, you can email it to me instead. But my default assumption is that we learn from each other as much as from ourselves, so I hope you can find a way to write publicly about your experience with this project.

<div class="alert alert-info">
    <p>I know it's a little awkward to have this fast turnaround ending during break. As I mentioned last time, this timing will (a) let me get a jump on responding to your projects, and (b) let you have most of your week to unwind between projects.</p>
    <p>That said, if you need extra time – especially if you're traveling at the start of the weekend and won't have that pre-deadline time available – just let me know you need an extension and we can work it out.</p>
</div>

Looking ahead: when we get back, it's our web design unit!

* You should already have done this, but just in case: if you don't already have a syntax-highlighting text editor you prefer, please download, install, and get comfortable with either [Visual Studio Code text editor](https://code.visualstudio.com/) or [Pulsar](https://pulsar-edit.dev). We'll be using text editors extensively for our upcoming web design unit.
    - If you're using VSCode, you may want to check out some [intro tutorials](https://www.youtube.com/playlist?list=PLj6YeMhvp2S5UgiQnBfvD7XgOMKs3O_G6). I also recommend this list of [HTML-specific features and optional settings](https://code.visualstudio.com/docs/languages/html).
