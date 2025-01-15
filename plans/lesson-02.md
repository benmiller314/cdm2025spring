
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

Welcome back! I really enjoyed reading all the introductory posts and letters; thank you for those. If you haven't had a chance to get to know your classmates' opening posts, I encourage you to [check them out]({{site.github.issues_url}}/1)!

And if you haven't posted one, please do! As noted in the contract, you get one free missed homework per unit, but you don't want to spend it before you really need it.


## Plan for the Day

<!-- <div class="alert alert-warning">
We've had a request to record today's session. Is everyone okay with that?
</div> -->

1. Introduction to GitHub (~30 min)
    <ol class="lalpha">
        <li>What's version control for?</li>
        <li>Considering the interface</li>
        <li>Clone, edit, save, commit</li>
        <li>Push and pull</li>
    </ol>
2. Taking your turn at the fork (~20-30 min)
    <ol class="lalpha">
        <li>Get your own copy</li>
        <li>Make some changes</li>
        <li>Push to your own repo</li>
        <li>EXT: Request a pull from upstream</li>
    </ol>
3. Report back and discuss (~10-15 min)
4. HW Preview (2-3 min)




## 1a. Introduction to GitHub: what's version control for?

In those intro posts, we saw that GitHub can host a discussion forum, so in that sense it's a community website: it makes media social.

But its core functionality is meant to solve a different (though related) media problem: how to _track changes to files over time_... especially if you're working on those files with someone else.

<figure role="figure">
  <a href="http://phdcomics.com/comics/archive.php?comicid=1531"><img src="../assets/img/cham-phd101212s.gif" style="max-height: 600px; max-height: 70vh; width: auto;" alt="webcomic shows a series of panels renaming final.doc to final_rev2, final_rev_6.comments, and so on to absurdity" title="I'm not the first to use this comic in a discussion of version control. See, for example, https://caltechlibrary.github.io/git-desktop/aio/."></a>
  <figcaption>from <a href="http://phdcomics.com/comics/archive.php?comicid=1531">PhD Comics</a> by Jorge Cham (2012).</figcaption>
</figure>

Retaining and renaming ever more files isn't just messy to keep track of: it also eats up your storage space, especially if you're working with multimedia. What git allows you to do instead is to **track the differences** between versions of files **while keeping the same filename.**

The rest of today's class will involve an interactive demo and an exercise you can do on your own and/or in groups. By the time we're done, you should be able to...

* Consider how an interface design (e.g. visual layout; menu options) communicates the priority of actions the designers expect you to perform
* Create and edit files with a plain text editor on your own computer
* Label important edits meaningfully
* Use GitHub to share files with others, along with a history of how they've changed
* Define the following terms:
    <ul class="flexit">
      <li>repo / repository</li>
      <li>README</li>
      <li>Markdown / .md</li>
      <li>clone</li>
      <li>commit</li>
      <li>commit message</li>
      <li>diff</li>
      <li>push</li>
      <li>pull</li>
      <li>fork</li>
      <li>EXT: pull request</li>
      <li>EXT: branch</li>
    </ul>

<div class="alert alert-info">
    <p>I've set up a shared note-taking space: <a href="https://bit.ly/cdm{{site.course.slugterm}}-notes">bit.ly/cdm{{site.course.slugterm}}-notes</a>. Any volunteers to be in charge of notes for today? Usually 2-3 people works best...</p>
    <p>PS. Advice from my years of experience doing simultaneous note-taking: it always helps to leave a blank line at the bottom for another note-taker to jump in. (Which also means, please add another blank line at the bottom when you do jump in!)</p>
</div>


## 1b. Considering the interface

In a new window, which you can also open up on your own devices, let's have a look at <strong><a href="https://github.com/benmiller314/cdm-gh-practice">github.com/benmiller314/cdm-gh-practice</a></strong>.

With any new interface – which a website is, but so is a desktop application, and so is a book – you can think about its design:

* Where is your attention drawn? e.g. What takes up the most area? What's given high contrast, in color or size?
* What's grouped together? Can you tell why, or by what principle?
* What functions/tools do you have quick access to? e.g. What can you interact with directly? What buttons or menus do you have, if any (whether in a toolbar or on a right-click)?

The answers may suggest (hopefully suggest) how the designers expect you to use it. Certainly they help set the parameters for how you'll explore it.

<!--
* Define repository, using text from the README.
* Point out the table of files, each with its most recent commit (linked) and when it happened
* Click on a file: this-is-just-to-say.txt. It displays; we could edit it! But let's not just yet...
-->

## 1c. Clone, edit, save, commit

### Clone: GitHub Desktop

Let's try engaging one of those highlighted tools! I'm going to **clone** the repository, opening it with GitHub Desktop. This creates a local copy on my computer that knows about the one online: it links files between the **clo**ud and the **ne**ar.

Let's take a first impression of GitHub Desktop:

* Where is your attention drawn? e.g. What takes up the most area? What's given high contrast, in color or size?
* What's grouped together? Can you tell why, or by what principle?
* What functions/tools do you have quick access to? e.g. What can you interact with directly? What buttons or menus do you have, if any (whether in a toolbar or on a right-click)?


### Edit: Pulsar (or VS Code)

Once again, let's follow the lead the software gives us and *open the repository in your external editor*.

* Where is your attention drawn? e.g. What takes up the most area? What's given high contrast, in color or size?
* What's grouped together? Can you tell why, or by what principle?
* What functions/tools do you have quick access to? e.g. What can you interact with directly? What buttons or menus do you have, if any (whether in a toolbar or on a right-click)?

Compare what you're seeing here to what we saw on GitHub's web interface... and in GitHub Desktop.

<!-- Same files as online. But now when we click on a file we can edit right away. -->

<div class="alert alert-success">
Let's make some changes, and see what happens!
</div>

### Save

And then let's head back to GitHub Desktop. Where's your attention drawn now?

### Commit

Git history isn't automatic: it doesn't track things every few seconds, like Google Docs. (Speaking of: how are those notes going?) Instead, it waits for you to be sure you have something worth keeping. It waits for you to **commit**.

A commit is, essentially, a _named_ save: a point in time you might want to come back to, or at least set as a basis for comparison. And while you can in theory name it [anything](https://xkcd.com/1296/) you want, it's a good idea to _make it meaningful_.

For example, "update files" doesn't tell you anything about what the update contains. A message like "draft 3" is better, but still quite vague (and it possibly masks a wide range of unrelated changes). Instead, aim for something like "replace plums with thumbs, and run with that" or "move title to the bottom," etc. Something that will let you actually find this point in history if you're looking for it later.

Note that the commit message interface has two parts: a short label, and a bigger box beneath. These are kind of like the subject line of an email and the email body. The first is what you'll see automatically when browsing the history; the second will usually require an additional click. And while GitHub will let you leave the "body" blank, you're required to have a "subject line."

## 1d. Push and pull

We've got the changes saved locally, and they're committed to git's history. But remember what I said way at the beginning, about GitHub being a _social_ site?

To get the changes out into the world, we can **push** them out into the ether.

If someone (including us) makes changes elsewhere, we can **pull** just those changes from out there back to our existing clone.

<div class="alert alert-info">
Each commit is actually just recording the <em>difference</em> from the previous state, so we don't need to re-copy the whole repository – only those bits that have changed. You only have to clone once.
</div>

## 2. Taking your turn at the fork

So far, we've been working in my copy of the repository. But one of the coolest things about GitHub is that you can very quickly make any public repo your own, and take it in a new direction.

This is called making a **fork**. To fork a repo is to _make a copy_ of it: all the files, and – importantly – the complete \*history\* of those files. This lets you safely play with and edit the files, without worrying that you'll overwrite someone else's work.

Importantly, once you've forked a copy of a repo, you now have a version of it _that you control_. The web address of that repo, for example, will change to show your username, rather than the original owner's. The two repos remain linked, though, so you can pull changes back and forth if you want to.
<!--
NB: For this exercise you can work alone or in groups. If you're working in groups, you'll want one partner to fork my repository, and the others to fork that fork. This will make it easier to combine your forks later on without worrying about overlapping with other groups in the original benmiller314 repo. -->

<div class="alert alert-success">
For this exercise, you're going to compose a very short story about what changes when <em>digital</em> comes into the mix. And you're going to write it in a forked repository, so we can merge them together later.</div>

You can work solo or in groups, but either way I'll ask you to sit with some new people: I've used your Tech Comfort Survey responses from Lesson 1 to build teams where at least one person has prior GitHub experience, so you can help each other where needed! (Also, if you indicated that you're used to being the only one doing the work in a group? Congratulations, now you're matched with others who said the same!)

<div class="alert alert-success">
When you've found your people, open up <a href="https://github.com/benmiller314/cdm-gh-practice/blob/main/your-turn">the your-turn folder</a> of the demo repository and follow the instructions there!
</div>

<!-- groups go here: -->
* Weini, Billy D, Maddie, Morgan
* Mia, Alyssa, David, Raegan B
* Reagan H, Erin, Grace, Hannah
* Yang, Carla, Dana, Will L
* Josh, Ellie, Shreya, Avery

(Moving into position also functions as a stretch break and a name refresher. :)

Read through the details, then follow the steps to add one piece of the story at a time, committing as you go. **We'll work in groups for about 10-15 minutes, then report back.**



Call me if you need me! Otherwise, I'll be floating from group to group. And note the EXT activity in the repository itself if you finish early.


## 3. Report back and discuss

What was exciting? What was challenging?

Any volunteers to share what you wrote?

Any terms from that <a href="https://bit.ly/cdm{{site.course.slugterm}}-notes">notes doc</a> that are still unclear?

(Did anyone get to the EXT with Janet Murray?)



## HW for next time:

* **Read** and **watch** two versions of "Five Principles of New Media: Or, Playing Lev Manovich," by Madeleine Sorapure:
    - a roughly 6-page _[text-only version](https://kairos.technorhetoric.net/8.2/coverweb/sorapure/five.pdf)_ that was always served alongside the [original Flash site](https://kairos.technorhetoric.net/8.2/binder2.html?coverweb/sorapure/index.htm) (now defunct)
    - a [_video recording_ of the original Flash site](https://sorapure.net/five.mp4), demonstrating the interactive features that no longer work. (Run time is 22:24 at 1x speed.)
    <!-- FOR NEXT TIME: Experiment time! If your name starts with A-L, read the text before the video. If your name starts with M-Z, watch the video before the text. -->

* **Write** a short blog post (~200–500 words) to the appropriate thread [on the issue queue]({{site.github.issues_url}}):
    - What do you notice, i.e. what stands out while reading or watching? Locate us somewhere in the "text."
    - What does that suggest, or what does it make you wonder?
    - In particular, _what can and can't text do_ (clarify, convey, etc) in this context?

* EXT for eager readers: interested in more on affordances? Try [this short chapter](https://wac.colostate.edu/docs/books/design/chapter7.pdf) from *Keywords in Design Thinking*.
