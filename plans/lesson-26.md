# Last day of class! Looking back and looking forward

<section class="prereqs">
    <details open><summary><strong>Work to have achieved</strong></summary>
        <ul>
            <li>Take the <a href="https://bit.ly/tech-comfort-redux">Tech Comfort Survey Redux</a></li>
            <li><em>(Optional)</em> Identify something said, read, or made in this course – by you or not – that you want to remember beyond this semester.</li>
            <li>Consider what earlier reflections,  feedback, commit messages, etc you'll want to include in the final portfolio to support your introductory letter</li>
            <li>Otherwise proceed on your plans toward consolidating and integrating what you've learned, saving/committing/pushing along the way</li>
        </ul>
    </details>
</section>

**Plan for the day**:

1. Gifts and Remembrances (optional)
2. OMETs, if you haven't yet (due Wed Apr 23 at 11:59pm)
3. Notes before studio
  - Final portfolio FAQ
  - Memory management: detaching from the fork tree
4. Studio
  - Set an intention
  - Exit note
5. The ends of a term


## Gifts and Remembrances (optional)
A handful of people had voted last class in favor of sharing something awesome they made and are proud of, or something awesome they appreciated from someone else in the class, for the purposes of celebrating our collective accomplishments. I heartily support this volunteerism!

Let's take 2-3 minutes for each share, up to a total of about 10 minutes (to preserve working time for everyone who voted to work).

## About OMETs (5 min intro + 10 min to fill out)

I know some of you have already turned in your surveys for the Office of Measurement and Evaluation of Teaching (yep, that's what OMET stands for). If so, you can feel free to work on your own projects, though I hope what I'm about to say is still useful information.

Actually, I hope you all know this stuff already, but my experience has been otherwise, so I try to say it in every class:

<details><summary>OMETs are a pretty important way of getting your voices heard; they can also have some pretty outsized effects on your teachers' lives.</summary>
    <!-- <div class="alert alert-info"> -->
    <strong>These evaluations of teaching serve multiple purposes, and go to multiple audiences:</strong>
    <ul>
    <li>They'll go to my program director, to help determine if I should keep teaching this course;</li>
    <li>they'll become part of my portfolio application for promotion, read by other faculty inside and outside my department; <!-- again: renewal. also: promotion --></li>
    <li>and, after grades are turned in, they'll go to me, so I can use them to revise and update the course. For that purpose, I especially value the free responses. (I also added a few Likert questions that are particular to this section of the course.)</li>
    </ul>
    <!-- </div> -->

    <p>The same is true for all your instructors.</p>

    <p>Filling out OMETs for all your classes is important because they're a great way that you the student can participate in the work of the university, make your voice heard, and help identify and celebrate excellent teaching.</p>

    <p>But on the other hand, they can also powerfully affect hiring, especially for women, immigrants, and people of color, i.e. people who are already more vulnerable to bias and exclusion. This is particularly important to keep in mind if you are taking classes in fields that are majority white and/or majority male.</p>

    <p>So in this class, and in every other class that you take, keep that bigger systemic bias that OMETs can have in mind. I think it’s important to bring up this potential bias since it’s been shown that <a href="https://pubmed.ncbi.nlm.nih.gov/31329505/">being made aware of biases on standardized evaluation forms can help to combat bias</a>.</p>

    <p>Of course, I want you to be truthful and accurate in your experience. It’s important to be critical of ineffective teaching practices if you see them. But knowing the upsides and downsides of OMETs can help you do this in an even-handed way across your classes.</p>

</details>

In brief: please do fill these out, but <strong>please do your best to be fair, to be thoughtful, and to be considerate of how things like race, gender, and linguistic difference might color your responses.</strong>

<div class="alert alert-success">
If you haven't yet filled out your survey, please do so now. You should have a link to the survey on Canvas, or in your Pitt email.</div>

EXT 1: I know some of you may already have filled out the end-of-semester version of the <a href="https://bit.ly/tech-comfort-redux">Tech Comfort Survey</a>, but if you haven't, I hope you'll consider doing so now.

EXT 2: If you've done the Survey and the OMET to your satisfaction and you're waiting for your classmates to finish, you can use this time for solo work on your portfolio / revisions or your final reflection. Start by reading my notes below.

<!-- <div class="alert alert-white">
I'll turn off the Zoom recording and absent myself for a bit in a breakout room, just in case you want to talk amongst yourselves. Figure it'll take around 10 minutes? I'll monitor the completion rate to know when it's safe for me to come back. Or come find me if everyone's done.
</div> -->

## Notes before Studio

We'll spend just about the rest of class working on your individual and group projects / final reflections.

### Memory management: detaching from the fork tree

The way GitHub sets up forks assumes that everyone's contributing to one shared project. If the root repository being forked uses large file storage (Git-LFS), they therefore assume that all the files should belong to the root repository also.

For professional software development, that's probably a safe assumption; for classroom assignments, like ours, it's very much not. And one result of that assumption is that I am currently paying for all the large files you created this semester.

<details><summary>To fix that problem <em>and</em> keep all your files, here's what to do.</summary>

    <ol>
        <li>Locate your CDM repositories on github.com.</li>
        <li>For each repository, run a few commands in Terminal (Mac) or Git Bash (Windows) to <a href="https://docs.github.com/en/repositories/creating-and-managing-repositories/duplicating-a-repository#mirroring-a-repository-that-contains-git-large-file-storage-objects">mirror that repository</a>, creating a local copy. Be sure to follow instructions for <strong>"mirroring a repository that contains Git Large File Storage objects."</strong><ul>
        <li>If you don't have it yet, you may need to first <a href="https://git-scm.com/book/en/v2/Getting-Started-Installing-Git">install command-line git</a> for your operating system.</li></ul></li>
        <li><a href="https://docs.github.com/en/repositories/creating-and-managing-repositories/deleting-a-repository">Delete the original online repository</a>, now that you have a distinct local copy saved.</li>
        <li><strong>Republish your mirrored repository</strong> on its own (i.e. no longer as a fork of my assignment repo).<ul>
            <li><a href="https://docs.github.com/en/desktop/adding-and-cloning-repositories/adding-an-existing-project-to-github-using-github-desktop">You can do this in GitHub Desktop</a> by adding the new repo location, then clicking "Publish repository" in the menu bar.</li>
            <li>Make sure it's public if you want me to still be able to see it!</li></ul>
        </li>
    </ol>
</details>

<div class="alert alert-warning">
NB: One step involves (temporarily) deleting your public repository. If you're nervous about doing this before the final portfolio is due and graded, you can for sure wait until afterwards! I'm also happy to help you, even if it's over the summer: we can meet by Zoom.
</div>



### Final portfolio FAQ

Some people have historically asked questions that maybe you have floating around in your head, too.

<details><summary>What do you mean by “linked thumbnail”?</summary>

<p>All I mean by <em>thumbnail</em> is a small picture; all I mean by <em>linked</em> is that it should be clickable, a hyperlink.</p>

<p>As you know from previous reflections, you can upload an image into your post on the Issue Queue just by dragging and dropping the file, which will generate some markup like this:</p>

<div class="language-markdown highlighter-rouge"><div class="highlight"><pre class="highlight"><code><span class="p">![</span><span class="nv">name-of-file.png</span><span class="p">](</span><span class="sx">https://somecrazylongURLthatGitHubauto-generates</span><span class="p">)</span>
</code></pre></div></div>

<p>If you want the image to link directly to your repository for that project, you would add another layer of markup, using the structure <code class="language-plaintext highlighter-rouge">[anchor](URL)</code>. So in this case, because the anchor is that whole long thing GitHub generated after the drag-and-drop, you’d link like this:</p>

<div class="language-markdown highlighter-rouge"><div class="highlight"><pre class="highlight"><code><span class="p">[</span><span class="nv">![name-of-file.png</span><span class="p">](</span><span class="sx">https://somecrazylongURLthatGitHubauto-generates</span><span class="p">)</span>](https://github.com/username/repo)
</code></pre></div></div>

<p>Note the double closing in the middle: close-parenthesis, close-bracket. You can also use real HTML (i.e. <code>&lt;a&gt;</code>) inside Markdown, but you can't use Markdown inside HTML, so you'd need to convert the Markdown image syntax to your usual <code>&lt;img&gt;</code> syntax.</p>

<p>If all that’s too annoying, or it keeps breaking and you're not sure why, you can also just paste the regular link underneath the image, like this:</p>

<pre><code class="language-Markdown">**Audio narrative thumbnail:**

![name-of-file.png](https://somecrazylongURLthatGitHubauto-generates]

[Link to soundscape file](https://github.com/username/repo/blob/master/name-of-playable-file.mp3)
[Link to soundscape repository](https://github.com/username/repo)
</code></pre>

</details>
<details><summary>Why do I need to link to the project <strong>and</strong> link to the repository? Aren't those the same?</summary>
<p>The project link should take us to the final, rendered version: the "flat" export, or the home page of the website. This is to avoid any potential confusion in your file structure, where it might be unclear which version is really the final one. So click through to the actual file in your repo, and then grab <em>that</em> URL.</p>
<p>That said, I also want to have easy access to the repository as a whole, so I can look at things like the README, credits, commit history, etc.</p>
</details>
<details><summary>When you say, "link to a specific point in the revision history..."</summary>
<p>Remember how, during workshop, you would click on a particular commit message to leave comments? And it would open a page showing the files that were changing in that commit? It's <em>that</em> kind of page I'm talking about. You can once again use the structure <code class="language-plaintext highlighter-rouge">[anchor](URL)</code>, but instead of getting the URL of the repo as a whole, <em>click through to the commit history, like you did for workshop, and grab the URL of the commit</em> that represents that past moment you want to compare to the present.</p>

<p>Hope that clarifies things!</p>

</details>

Anything else you're wondering?


### Set an intention

As usual, please...

1. Write your goals [in the google doc](http://bit.ly/cdm{{site.course.slugterm}}-notes#heading=h.1tqhsvrbsrr2)
2. Expect to leave an exit note to report on progress and re-set goals for moving forward.
3. Save an extra couple of minutes at the end of class, to bring us back together, for closure.

<!-- For Zoomers, I'll once again set breakout rooms for maximum flexibility, and otherwise hang out in the main room unless people need one-on-one time (when we can go to an extra room set aside for that purpose). -->

Just for fun: Final stats for the shared google doc, as of last night (and probably longer now!)
* 15,689 words
* ~56 pages
* 40,576 revisions


### Exit note

When we're getting toward those last few minutes, please head back to the google doc to write an update: What have you achieved today? What are your goals for the weekend? For the final portfolio?

## The ends of a term

* The final portfolio will be due during our final exam slot, which is **Monday, April 28th at noon**.
* The reflection is the main thing, so **if you do make revisions to earlier projects, please be sure to talk about them in the reflection.** Or even if you don’t have time to make revisions, but want to talk about what you _would_ revise, if you had more time, you can talk about that in the reflection, too. I'm most interested in what you've learned this semester, and what will help you keep learning after it ends.

* Office hour update: I have office hours today and on Wednesday at <a href="../office">the usual times</a>, but Wednesday will be on Zoom only. Let me know if you're coming at the link above, or just drop by. And you can also always email me with questions.

<div class="alert alert-white">I like to <a href="https://www.poetryfoundation.org/poems/47785/at-the-san-francisco-airport">end with poetry</a>.</div>
