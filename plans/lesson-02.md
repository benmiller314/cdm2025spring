
# Interfaces and Repositories

<!--  BEN: Set up (Zoom breakout) groups ahead of time! -->

<section class="prereqs">
    <details open><summary><strong>Texts to have read</strong></summary>
        <ul>
            <li><a href="/{{site.course.base_url}}uploads">the syllabus</a> and <a href="{{site.canvas_url}}/modules">related Canvas modules</a></li>
        </ul>
    </details>
    <details open><summary><strong>Work to have achieved</strong></summary>
        <ul>
            <li>Respond to the <a href="https://bit.ly/cdm2021survey">Tech Comfort Survey</a></li>
            <li>Post to the main course <a href="{{site.github.issues_url}}/1">issue queue</a>, introducing yourself to classmates (and whoever stumbles upon it)</li>
            <li>Download and install <a href="https://desktop.github.com">GitHub Desktop</a> and <a href="https://code.visualstudio.com">VSCode</a> (or <a href="https://pulsar-edit.dev">Pulsar</a> or another syntax-ready text editor)</li>
        </ul>
    </details>
</section> <!-- /.prereqs -->


## Plan for the Day

<!-- <div class="alert alert-warning">
We've had a request to record today's session. Is everyone okay with that?
</div> -->

1. GitHub, part 2 (~20-30 min)
  * Why version control?
  * Introduction to GitHub
  * a demo of diffs<!-- repo, commit, history, diff -->
  * Multiple views of the same files: web, Finder/Explorer, GH Desktop, text editor
2. Your turn! Practice forking an assignment repository and editing its files (~20-30 min)
3. Shareback and discuss (~10-15 min)
4. HW Preview (2-3 min)

Welcome back! I really enjoyed reading all the introductory posts and letters; thank you for those. If you haven't had a chance to get to know your classmates' opening posts, I encourage you to [check them out]({{site.github.issues_url}}/1)!

And if you haven't posted one, please do! As noted in the contract, you get one free missed homework per unit, but you don't want to spend them before you really need them.


## 1. GitHub, part 2
In those intro posts, we saw that GitHub can host a discussion forum, so in that sense it's a community website: it makes media social.

But its core functionality is meant to solve a different media problem: tracking changes to files over time.

<figure role="figure">
  <a href="http://phdcomics.com/comics/archive.php?comicid=1531"><img src="../assets/img/cham-phd101212s.gif" style="max-height: 600px; max-height: 70vh; width: auto;" alt="webcomic shows a series of panels renaming final.doc to final_rev2, final_rev_6.comments, and so on to absurdity" title="I'm not the first to use this comic in a discussion of version control. See, for example, https://caltechlibrary.github.io/git-desktop/aio/."></a>
  <figcaption>from <a href="http://phdcomics.com/comics/archive.php?comicid=1531">PhD Comics</a> by Jorge Cham (2012).</figcaption>
</figure>

Retaining and renaming ever more files isn't just messy to keep track of: it also eats up your storage space, especially if you're working with multimedia. What *git* allows you to do instead is to **track the differences** between versions of files **while keeping the same filename.**


<div class="alert alert-success">
Let's check out the GitHub.com web interface, and see how it works:
<strong><a href="https://github.com/benmiller314/text-demo">https://github.com/benmiller314/text-demo</a></strong>
</div>

### Initial questions to ask of any app:

- How is the space laid out?
- What's given the most prominent visual focus? Secondary focus?
- What features/tools do you have quick access to?

<!--
1. Create a new .txt file based on https://www.poetryfoundation.org/poems/56159/this-is-just-to-say
2. <del>Demo the importance of the extension by previewing what happens if it's .md?</del> NAH
3. Commit the new file directly to the main branch.
    - Note that the commit message has two parts: a short label, and a bigger box. These are kind of like the subject line of an email and the email body. The first is what you'll see automatically when browsing the history; the second will require an additional click. And GitHub will let you leave the "body" blank, but you're required to have a "subject line."
4. Use the CODE button to *Open in GitHub Desktop*. Ask the questions above again: how is the space laid out? What's given the most prominent visual focus? Secondary focus? What features/tools do you have quick access to?
5. Open the file and change the text. *Ask for suggestions (in the Zoom chat, if on Zoom).*
6. Create a new branch, then merge it. Why, you ask?
   It matters when you're working with others: you want to make sure you're comparing against the most up-to-date version, so you don't accidentally erase something new.
   This will become important in a minute.
-->

## 2. Your turn

Time to take these abstractions and put them into practice.

We'll be working in groups. I've used your Tech Comfort Survey responses from Lesson 1 to build teams where at least one person has prior GitHub experience, so I hope you'll be able to help each other where needed!

<!-- groups go here: -->
* Weini, Billy D, Maddie, Morgan
* Mia, Alyssa, David, Raegan B
* Reagan H, Erin, Grace, Noah
* Yang, Carla, Dana, Will L
* Josh, Ellie, Shreya

<div class="alert alert-success">
Head to
<p><strong><a href="https://github.com/benmiller314/cdm-gh-practice#readme">https://github.com/benmiller314/cdm-gh-practice</a></strong>, where you'll find more instructions for what to do next – starting with forking the repo. (Thanks, group GitHub anchors!)</p>

<p>Please start by skimming through the instructions in the README file, so you know where this is headed. (It'll spare you confusion later, based on past semesters!)</p>

<p>I'll give you the overview while we're still together:</p>

<ol><li>Make a copy of the repository for your group</li>
<li>Write a short story, one line per person, committing every time you add a line</li>
<li>File a <em>pull request</em> to merge it back to my repo</li></ol>
</div>

Read through the details, then follow the steps. **We'll work in groups for about 10-15 minutes, then report back.** <!-- Don't forget that you can use Zoom chat and screenshare to show your groupmates what you're doing. --> NB: For this task, you can use either the GitHub web interface or use GitHub Desktop to "pull" files to edit on your own computer and then "push" them back.

Call me if you need me! Otherwise, I'll be floating from group to group. And note the EXT activity in the repository itself if you finish early.

## 3. Report back and discuss

What was exciting? What was challenging? Anyone get to the EXT?

## HW for next time:

* **Read** and **watch** two versions of "Five Principles of New Media: Or, Playing Lev Manovich," by Madeleine Sorapure:
    - a _text-only version_ that was always served alongside the [original Flash site](https://kairos.technorhetoric.net/8.2/binder2.html?coverweb/sorapure/index.htm) (now defunct)
    - a [_video recording_ of the original Flash site](https://sorapure.net/five.mp4), demonstrating the interactive features that no longer work. (Run time is 22:24 at 1x speed.)

* **Write** a short blog post (~200–500 words) to the appropriate thread [on the issue queue]({{site.github.issues_url}}):
    - What do you notice, i.e. what stands out while reading or watching? Locate us somewhere in the "text."
    - What does that suggest, or what does it make you wonder?
    - In particular, _what can and can't text do_ (clarify, convey, etc) in this context?



## EXT: VS Code interface

Using those same questions from above:

- How is the space laid out?
- What's given the most prominent visual focus? Secondary focus?
- What features/tools do you have quick access to?
