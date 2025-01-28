
# Lesson 5: Sources, Citation, Studio

<section class="prereqs">
    <details><summary><strong>Texts to have read / listened to / watched</strong></summary>
        <ul>
            <li><a href="https://ebookcentral.proquest.com/lib/pitt-ebooks/reader.action?docID=6745793&ppg=229">"Working with Multimodal Assets and Sources," by Ball, Sheppard, and Arola</a></li>
            <li><a href="https://training.npr.org/audio/six-npr-stories-that-breathe-life-into-neighborhood-scenes/">"Breathe Life into Neighborhood Scenes"</a> by Alison MacAdam, from NPR Training</li>
            <li><a href="https://libguides.udayton.edu/oral-history-recording/phone-tips">Tips for Recording Audio on a Phone</a>, a LibGuide from the University of Dayton</li>
        </ul>
    </details>
    <details><summary><strong>Work to have achieved</strong></summary>
        <ul>
            <li>An audio narrative proposal, posted to the <a href="{{site.github.issues_url}}/4">issue queue</a> (and optionally to your own repository)</li>
        </ul>
    </details>
</section>


## Plan for the day

1. Sourcing ethics and GitHub: ignoring files and folders (5-10 min)
2. Sourcing ethics: key concepts and practical takeaways (~10-20 min)
3. In-class studio (~45 min)
    - Read composing advice
    - Set explicit goals
    - Work on your own (ask for help/advice as needed)
    - Exit note
4. Sharing fun clips (from last time? from today?)
5. Homework: audio narrative preview


## 1. Sourcing ethics and GitHub: ignoring files and folders

As you know from _Writer/Designer_, there are some source files that we have implicit license to reuse and distribute (e.g. public domain), some that we have explicit license to reuse and distribute, albeit potentially with some restrictions (e.g. Creative Commons), and some that we can make limited fair uses of, but can't distribute in their entirety (copyright).

**But if we're working with a public repository on GitHub, what are we to do with source files we aren't allowed to distribute?**

GitHub offers a solution: the `.gitignore` file. Any file path that matches the patterns in that file won't be tracked or version controlled. In the assignment repository you cloned from me, I had already pre-populated that file with the line `sources/**`: in other words, any file in the "sources" folder should be ignored.

<div class="alert alert-success">
Try it out! Temporarily move a small file from the in-class-exercises folder into the sources folder, and head over to GitHub Desktop.
</div>

You should see that the file was deleted from its original location... but not added to its new location, because _GitHub can't see inside the sources folder: it's been ignored_.

<div class="alert alert-success">
Go ahead and move the file back.
</div>

Should you ever want to change what git/GitHub is ignoring, you can! In GitHub Desktop, go to the Repository menu, then select Repository Settings > Ignored Files... or just edit the .gitignore file in your text editor of choice.

<details><summary>Show me</summary>
    <figure>
        <img src="../assets/img/github-desktop--repository-settings.png" alt="GitHub Desktop's Repository menu">
        <figcaption>Start with the Repository menu and choose "Repository Settings"</figcaption>
    </figure>
    <figure>
        <img src="../assets/img/github-desktop--repository-settings-2--gitignore.png" alt="Repository Settings for Ignored Files">
        <figcaption>The 'Ignored Files' tab lets you edit the .gitignore file directly from the GH Desktop app.</figcaption>
    </figure>
</details>


## 2. Sourcing ethics: key concepts and practical takeaways (10-20 min)

I'm going to ask you to <a title="The quiz is set up individually, so you can either keep the groups from last time or mix it up.">group up</a> again and work through some [questions about the reading/listening from the last week](https://canvas.pitt.edu/courses/296641/quizzes/395355/), which I've set up as a quiz in Canvas. Don't worry, it's not factored into your grade! But I do still want to make sure you understand these things.

<div class="alert alert-success">
<p>Discuss before putting in your group's answer, and then please pay attention to the notes that I've added to my answers. We can talk through any questions or discrepancies; call me over! </p>

<p>When you're done discussing these questions (and answers), head back here for some more open-ended prompts to discuss within your group.</p>
</div>

Some questions you should be able to zip through quickly; others may require more discussion. Heads up: even several of the True/False questions are more complicated than that binary implies! ;)

<details><summary>Quiz questions, for future reference</summary>
    <ol>
        <li>True or false: if you can find it on the internet, you can use it in your project.</li>
        <li>True or false: the only sources you can use in this project are those you record yourself.</li>
        <li>True or false: if you record your own sources, you don't have to cite them.</li>
        <li>True or false: if you use a source with a Creative Commons license, you don't have to cite it.</li>
        <li>True or false: to cite a source with a Creative Commons license, you should be sure to write "licensed under the Creative Commons."</li>
        <li>True or false: you're <strong>not</strong> allowed to mix assets from CC-BY and CC-BY-SA licensed sources.</li>
        <li>What's the difference between fair use and Creative Commons?</li>
    </ol>
</details>

### Discussion questions

When you're done with the quiz, and you've gone over the notes, talk through these. Take notes in our shared google doc: [bit.ly/cdm{{site.course.slugterm}}-notes](https://bit.ly/cdm{{site.course.slugterm}}-notes).

8. How would you define a "credible citation" in relation to the audio narratives you've proposed?
9. Why do you think Ball, Sheppard, and Arola are so insistent about folder structure and file naming conventions?
10. Would you (each of you, specifically, for this project) want to work from a written script? Why or why not?
11. Would you (again, each of you in <!--the breakout room--> your group, today) want to incorporate human voices in your audio narratives? How or how much, and why (or why not)?

### EXT: Bonus questions for the swift

12. Does my use of the "Piled Higher and Deeper" comic in [lesson 2](lesson-02) fulfill the criteria of fair use? Consider all four major factors.
13. What's one way to make sure you're recording the sound you want to (and not, say, the loud bus passing by your conversation)? <!-- headphones -->
14. What does MacAdam consider tempting cliches of soundwriting, and how does she suggest getting past them?  <!-- birds chirping, cars rolling by (which also sounds like water), kids at a playground. Get past with strong voiceover writing; contextualizing structure; specific instances of a theme. -->


* EXT on the EXT: Read through the link at the top of Fowkes' piece: [Top 10 Simple Field Recording Tips](https://citiesandmemory.com/2014/03/ten-top-simple-field-recording-tips/). Any surprises that others in the class should know about? Let us know in the notes doc!



<!-- <div class="alert alert-success">
As time allows, Let's talk through any <strong>questions or tensions</strong> that came up. I especially want to make sure we're all on the same page about those fuzzier "True/False" questions.</div> -->


<h2 id="hw-preview">Homework preview (5 min)</h2>
<a href="#hw">Jump down</a>


## 3. In-class studio

Most of the rest of the day will be time to work on your own: scripting, finding sources (and recording TASL information: Title, Author, Source, License), importing sources into Audacity to extract assets, arranging assets into a story, etc.

But first, read through my notes below, and then **write a short note about your goals for the day in the <a href="https://bit.ly/cdm{{site.course.slugterm}}-notes">shared notes doc</a>:** what are you working on today?

When it's time to stop (around 2:00 or 2:05), I'll ask you to return to this note and reply to yourself: how'd it go? What's your new goal for the next time you work on this project?

### 3a. Composing advice, mostly based on proposals

Lots of great ideas in those proposals. My small bits of broadly applicable advice as you get underway:

<details><summary>Record some "silence" every time you record</summary>
    As we discussed last time, every location has its own characteristic background noise. If you're recording in more than one place (or sometimes, the same place at different times), you might be able to hear the difference, especially if you're not recording under ideal conditions, e.g. with sound absorption on your microphone etc. BUT if you record a few seconds of that background before or after what you're hoping to use in your project, you'll give Audacity what it needs to try to <a href="https://support.audacityteam.org/repairing-audio/noise-reduction-removal">Noise Reduction</a>.
</details>

<details><summary>This is my life (not someone else's)</summary>
  If you're doing a day-in-the-life, a commute, a night out, the challenge is to make at least some of your narrative different from everyone else's: parts of a particular soundscape, not a generic one. Voiceover, even the little mutterings of a solitary person to themselves, may help; your choice of a soundtrack overlay might, as well. Or, like Will or Weini, you might decide that this particular day is less typical than it seems at first...
</details>

<details><summary>Consider getting it in writing</summary>
  One benefit to drafting a project in prose is that your script doubles as a transcript – which improves both accessibility and discoverability. It also means you get clean version history as you revise your script. (One downside is that it's sometimes easier to <em>do</em> or <em>say</em> than it is to <em>write</em>.) Still: something to keep in the back of your mind, especially if you're working on something fictional or working with voice actors.
</details>

<details><summary>Roll tape!</summary>
  On the flip side, if you're proposing something where you're not sure what you'll find, consider a journalistic approach: record more than you think you'll need; narrate what you're doing as you're doing it; then add a post-hoc voiceover that makes sense of (tells the story of) what you ultimately found.
</details>

<details><summary>Need to show time passing? Try a cut – or a crossfade</summary>
  If your proposal covers a long time – a full day, a full game, etc – you won't be able to represent it minute by minute. Instead, you might want to jump from moment to moment with a sharp cut from one background track to another. (Compare this to panels in comics, or cuts between camera shots in film.) But if you want to give a sense of time passing without changing where you are, one option is to fade out from the first moment <em>while you fade in</em> the later one. You can even do this with parts of the same musical track. You should get a sense of change within sameness – a kind of auditory montage.
</details>

### 3b. Set a goal
<div class="alert alert-success">
To help with goal-setting and reflection (and so I can figure out where I can be most helpful), please <strong>write a brief note in the <a href="http://bit.ly/cdm{{site.course.slugterm}}-notes">shared doc</a> about what you're planning to work on today.</strong> At the end of class (around 2:00 or 2:05), reply to your own note to say what you achieved and/or to set yourself a new goal for homework.
</div>

### 3c. Go for it! (40-45 min)

<strong>Do whatever work you need to get <em>something</em> toward your project posted to your GitHub repository by the night before our next class:</strong> find audio sources you have permission to use, extract assets from them, record test voiceover with your phone or computer, start moving things around in Audacity, practice some more with GitHub Desktop (or command line git).

**Save as you go, and commit when you have something to say about what you've achieved.** Remember: thanks to version control, you won't need to rename this file, so call it something that will last.

<div class="alert alert-warning">
Warning: <strong>don't use the GitHub <em>website</em> for Audacity files!</strong> They quickly get too large for the site to handle. Instead, commit locally, then push, from GH Desktop (or the command line). Using <abbr title="Large File Storage">Git-LFS</abbr> should bypass that concern... but the website interface doesn't know how to do that!
</div>

The goal for now is to get a feel for how you work with audio, not to have a finished product. In our next class, we'll use your experience to refine our shared baseline criteria and brainstorm some aspirational goals.

**Call me over if you need help** with Audacity, Git/GitHub, or determining the license on an audio source!

<section id="faq"> <!-- commented out in 2025spring -->
    <!-- ## 2b. FAQ / Q & A -->

    <!-- <details> <summary>I'm assuming that because repurposed assets are borrowed from other authors with their permission, they are not considered copyright?</summary>
        <p>Not exactly. Something being copyrighted does not automatically mean no one else can use it: it just means that <em>the author gets to decide</em> what permissions to grant. And in the US, as Ball et al note, "the moment an author 'fixes' an original idea into a text, he or she immediately has copyright over that text" – though they are permitted to transfer that right to others, e.g. to a publisher (154). </p>
        <p>In the case of a work that's Creative Commons licensed, for example, the work is also still protected under the copyright of its creator(s), who can decide to change the license later; and all CC licenses (except for CC0) require derived works to cite the original creator. (This is the BY clause.) On the other hand, even copyrighted works are subject to fair-use doctrine, so reuse can't be restricted entirely.</p>
    </details> -->

    <!-- <details><summary>Recently with the invention of neat AI systems like ChatGPT and Dall-E copyright has become a topic I'm more interested in. While ChatGPT and Dall-E generate text and image respectively, what happens when an AI generates music. Can someone copyright that as their own?</summary>
        <p>It's an open question, for now, and a tricky one! Part of the complication is how these AIs are trained: usually, by scraping and processing many thousands of previous creative works, including many that are under copyright. The question then becomes whether the resulting work is sufficiently transformative of the original art. If you do a targeted scrape of the collected works of Lin-Manuel Miranda and specifically ask the AI to produce music in the style of Lin-Manuel Miranda, that's probably too directly derivative. If you instead ask it to produce music in the style of Mozart, you might get something more new and strange &ndash; and therefore more defensible under fair use precedents. (Likewise, the more diverse the training set.)</p>
        <p>Another part of the complication is the question of who counts as the "creator" of algorithmically generated works: the AI itself? the people who fed it training data? the people who wrote the algorithm? the people who passed the algorithm a prompt to generate from?</p>
        <p>This is so new that it's only just starting to go through the courts, and it wouldn't be surprising for the courts to reach different conclusions that then have to be resolved higher up in the system. For those interested in reading more, think pieces abound. Here are a few I found just now:
          <ul>
            <li>Brittain, Blake. 2023. “Computer Scientist Says AI ‘artist’ Deserves Its Own Copyrights.” Reuters, January 11, 2023, sec. Litigation. <a href="https://www.reuters.com/legal/litigation/computer-scientist-says-ai-artist-deserves-its-own-copyrights-2023-01-11">https://www.reuters.com/legal/litigation/computer-scientist-says-ai-artist-deserves-its-own-copyrights-2023-01-11</a>.</li>
            <li>Mathur, Atreya. 2022. “Art-Istic or Art-Ificial? Ownership and Copyright Concerns in AI-Generated Artwork.” <em>Center for Art Law</em>. November 21, 2022. <a href="https://itsartlaw.org/2022/11/21/artistic-or-artificial-ai/">https://itsartlaw.org/2022/11/21/artistic-or-artificial-ai/</a>.</li>
            <li>Vincent, James. 2022. “The Scary Truth about AI Copyright Is Nobody Knows What Will Happen Next.” <em>The Verge</em>. November 15, 2022. <a href="https://www.theverge.com/23444685/generative-ai-copyright-infringement-legal-fair-use-training-data">https://www.theverge.com/23444685/generative-ai-copyright-infringement-legal-fair-use-training-data.</a>
            </li>
          </ul>
        </p>
    </details> -->

    <!-- <details><summary>What does "credibility" mean in the context of our audio narrative projects, which are narrative rather than scholarly?</summary>
      <p>It's less a matter of accuracy, in this case, than of appropriateness and ethos more broadly: Does your use of the asset take genre expectations into account? Have you cited where it came from and your license for using it (which could be that it's a fair use, or that you created it), so listeners know you're being ethical in your sourcing?</p>
      <p> Relatedly, if you're using CC-licensed material that includes an attribution (BY) clause, have you named your source <em>in the derived project itself</em>, i.e. in the audio? (Even if it's a "for full credits, go to this URL.") If you're using something with a sharealike (SA) clause, have you applied <em>the same license</em> to your own work? Do you have any <em>incompatible</em> SA licenses? Have any identifiable voices given their consent to being recorded, and have you documented that consent somewhere?</p>
      <p>All of those actions help determine whether you seem trustworthy in your use of source material. </p>
    </details> -->


    <!-- <details><summary>Do we need to request permission from a copyright owner for sounds, such as crowd noises, we may find on the internet for our project?</summary>
        <p>It depends on how you're using it, and what permissions the creator may already have granted. There's a lot of multimodal source material that's released either into the public domain (in which case you don't even <em>need</em> to cite it... though I suggest you do, for ethos reasons) or released with explicit permission to copy (e.g. with a Creative Commons license). In those cases, you don't need to ask for permission because you already have it.</p>

        <p>You may also be able to make the case that your use of the source material counts as a Fair Use. Consider the Four Factors (Ball et al 156): the <em>purpose</em> of your use, the <em>nature</em> of the copyrighted work, the <em>amount</em> of the work used, and the <em>market effect</em>. If the preponderance of those factors point to your use being fair, you can probably get away without consulting the original writer/designers.</p>

        <p>Where copyright and explicit requests for permission come into play is when your use does *not* qualify as Fair Use: for instance, if you're releasing something widely that just reuses the full chorus of a famous song and could ostensibly substitute for paid downloads of an original song, you're on the wrong end of nature (creative work), amount (heart of the work), and market effect.</p>

        <p>It's legitimately complicated! Feel free to talk it out with me if you're not sure about the Fair Use analysis.</p>
    </details> -->


    <!-- <details><summary>Do we have to obtain a CC license? </summary>

        <p>Not necessarily! You get to decide, based on whether you want others to be able to reuse and remix your work without asking you, or if you'd rather they got in touch so you could decide to offer or withhold permission. Remember that if you do nothing, your work is automatically under your own copyright!</p>

        <p>And even if you do want to be permissive by default, you'd usually still have the freedom to decide what level of permission to give: e.g. whether it could be used for commercial purposes or not, if your work had to be left intact to be used or if it could be modified, etc. There's a free tool at <a href="https://creativecommons.org/choose/">creativecommons.org/choose/</a> to help you weigh those licenses... and there are other open licenses, besides CC.</p>

        <p>The one exception, when you don't get a say in what license to use (or whether to provide any license), is if you're using material that has a ShareAlike clause: that is, if one of your assets is <a href="https://creativecommons.org/licenses/by-sa/4.0/">CC-BY-SA</a> or <a href="https://creativecommons.org/licenses/by-nc-sa/4.0/">CC-BY-NC-SA</a>. In that case, you <strong>must</strong> use the same license as your source. <em>Note that this means you cannot simultaneously use sources with incompatible ShareAlike licenses.</em></p>
    </details> -->

    <!--
    <details><summary>Who exactly are asset lists for?</summary>
    This came in late enough that I don't have a full write-up. What do you all think?
    </details>
    -->

    <!-- <details> <summary>How does GitHub stack up to actual cloud storage services? Should we be mindful of how many commits of larger (non-text) files we make?</summary>
        This came in late enough that I don't have a full write-up, but two short answers: (1) this is why we need <a href="https://git-lfs.github.com/">git-lfs</a>, which I've already set up on the audio narrative repository; (2) this is one reason to keep your full sources in a folder that you <a href="https://docs.github.com/en/get-started/getting-started-with-git/ignoring-files">.gitignore</a>
    </details> -->
</section>

<!--
<div class="alert alert-success">
Has anyone tried out any of the sites linked to from our plentiful <a href="{{site.github_url}}/resources">Resources</a> page? Any recommendations, warnings, or other advice for your classmates?

Note that there are sections for both free/licensed sounds and music, and also (separately) for audio-unit-specific advice and examples.
</div> -->



## Homework for next time:

<ul>
    <li>Look over the audio resources on the site, and dig into anything that seems like it would help you.<ul>
      <li><a href="../resources#sounds-and-music">Free and licensed sounds and music</a></li>
      <li><a href="../resources#audio-editing--soundwriting">Advice and examples</a></li></ul>
    </li>
    <li><strong>Work</strong> on your audio narratives, getting at least two sound assets in Audacity in conversation with each other. If you have time, do more!</li>
    <li><strong>Push a preview</strong> of your project to your GitHub repository. As per the <a href="{{site.github.owner_url}}/audio-narrative-{{site.course.slugterm}}#deadlines-and-products">assignment prompt</a>, this should include:
      <ul>
      <li> A layered <strong>Audacity project file (.aup3)</strong>, showing the arrangement of your sounds so far, however rough. (It need not be a complete soundscape or narrative yet.) <span class="alert-warning">Remember: thanks to version control, you won't need to rename this file, so call it something that will last.</span></li>
      <li> At least one static <strong><a href="https://www.take-a-screenshot.org/">screenshot</a></strong> (.png or .jpg) of your Audacity file in progress. (You'll use this in your final reflection, for comparison later to subsequent drafts). Note that link: you shouldn't use your camera for this!</li>
      <li> A plain text (.txt) or markdown (.md) file, explaining in at least 300 words <strong>what you're showing us</strong> in this preview. Feel free also to ask questions or lay out next steps for yourself!</li>
      <li> An <strong>updated list of assets</strong> (either directly in README.md or in a separate assets.md / credits.md file), indicating which the files you've actually recorded or otherwise obtained. Add source documentation for any outside sources – along with your permission to use them (e.g. licenses, fair use; see <em>Writer/Designer</em> p. 160-165).</li>
      <li>Finally, <strong>export a playable mp3 file</strong>, both as a snapshot and just in case something goes awry with your Audacity project file.</li>
      </ul>
    </li>
</ul>


<details>
    <summary>Screencast of submission process</summary>

    <figure>
        <figcaption>Submitting a project preview: Save, Export, Commit, Push</figcaption>
        <iframe src="https://pitt.hosted.panopto.com/Panopto/Pages/Embed.aspx?id=eb1ab95d-5f91-4081-8602-ae2a0115f1db&autoplay=false&offerviewer=true&showtitle=true&showbrand=false&captions=false&interactivity=all" height="405" width="720" style="border: 1px solid #464646;" allowfullscreen allow="autoplay"></iframe>
    </figure>

</details>

<a href="#hw-preview">Jump back to studio instructions</a>
