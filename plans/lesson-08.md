
# Sound studio

<section class="prereqs">
    <details><summary><strong>Work to have achieved</strong></summary>
        <ul>
            <li>Any remaining feedback from last class's workshop</li>
            <li>Work in pursuit of an audio narrative</li>
            <li>Optionally, a short <a href="{{site.github.issues_url}}">blog post about possible future audio projects or revisions</a></li>
        </ul>
    </details>
</section>

**Plan for the day**:

1. It's a studio day! You can choose what to do!
2. But I do have some revision-oriented notes for the whole class (5-10 min)
3. Studio time (50-60 min)
  - Make a plan
  - Execute it
  - Exit note
4. Reflection guidance / deadlines (10 min)

## 1. It's a studio day
<div class="alert alert-success">
<strong>Today is all about working on your individual projects!</strong> Mix sounds, apply effects, watch relevant tutorials. I know your lives are busy; take advantage of this dedicated time free from other distractions and obligations to move your piece forward.
</div>

At the same time, it's worth noting that you're working **in a shared space**, in a studio. If you have questions, or you want feedback on something, you have your classmates and your instructor on-hand. Try not to monopolize anyone's time, but do be open to the possibility of getting farther together than you could on your own.


## 2. Some revision-oriented notes for the whole class
A few seeds of ideas I want to plant, having listened through as much as I could:

<!-- 2025:
* overall limiter
* noise reduction and spectral editing
* put credits in the audio itself – even if it's just a pointer to the repo
* the limits of ShareAlike
* consider voiceover – or re-recording muffled voices currently in background tracks
-->


<details open><summary>When giving credit, direct attention to your TASLs.</summary>
    <p>We talked a bit about this at the start of the unit: the idea that (a) if you're using Creative Commons assets, you're required to attribute them to a source, and (b) that such attribution ideally includes <strong>Title, Author, Source, and License</strong>, or <a href="https://wiki.creativecommons.org/wiki/Best_practices_for_attribution">TASL</a>. (If you know a date, I'd add that, too, for TASLD.) And most of you are doing a great job of listing those things in a file in your repo! Nice. Just remember that for "Source," a link to the search engine or database that you found it with (e.g. FreeSound) <em>isn't enough</em>: you'll want to point to the <em>specific page for the individual file</em> you're using.</p>
    <details><summary>A few finer points on CC licenses, especially if they say SA</summary>
        <p>Remember that in-class quiz: if you're using source material with a Creative Commons license, <strong>you do need to specify <em>which</em> license it uses</strong>: CC-BY, CC-BY-NC, etc. This is especially important for Share-Alike licenses (CC-BY-SA, etc), because they force you to use the same license and can therefore be in conflict with each other.</p>
        <p>And if you <em>are</em> using material with a Share-Alike license, make sure you license your project the same way! All you need to do is add a file called LICENSE.md to your repository, and add the HTML generated by <a href="https://chooser-beta.creativecommons.org/">https://chooser-beta.creativecommons.org/</a>.</p>
    </details>
    <p>But now imagine you send your mp3 to someone outside of the class. Does it contain all those references? Probably not. Does it contain a spoken tag letting people know where to find the file with all those references? Maybe not <em>yet</em>. But it probably should.</p>

    <p>A lot of the podcasts I listen to end with a sign-off: often, some kind of theme music, and a voice saying who played what role. Often they'll say who wrote the theme music, as well. You can use this same space to say, "For a full list of sources and attributions, please see github dot com slash [your username here] slash audio hyphen narrative hyphen 2025 spring."</p>
</details>

<!--
<details>
<summary>Realism doesn't have to mean real time.</summary>
<p>Silence, and sameness, sound a lot longer in playback than they do when you're recording them. Two seconds of nothing could be considered a Grand Pause. Think about how you would write a story with words: you wouldn't include every moment, every breath, every footstep; you'd just say, "The doorbell rang, and she opened the door." Similarly, in movies or TV, frequent cuts from one shot to another are the rule, and long takes are the exception. Feel free to elide some moments in time!</p>
<p>In retrospect, the examples I gave you included more examples of continuous time unfolding than of sharp jumps. But if you're trying to cover a larger period than four minutes, it may well help to have discrete / abrupt changes of background noise, music, etc, to signal scene changes. (You can sometimes also time these background changes to align with foreground sounds, like doors closing, a coat zipping, etc.)</p>
<p>And if you're worried about signaling how long something takes <em>within</em> a single scene, consider splitting a background track into two clips, sliding one underneath the other, and crossfading from an earlier to a later point in the same track. It works for dialogue as well as music!</p>
</details>
 -->
<!-- <details><summary>Differentiate using volume and left/right pan... but don't overdo it.</summary>
    <p>Many of you are doing smart work to differentiate foreground sounds from background, in part through "ducking" the background to a lower volume while keeping the sound going to provide depth. Similarly, many of you are doing smart work using left/right channels to differentiate speakers or to move things around the landscape.</p>
    <p>If you haven't yet tried either, go for it! The left/right channels are visible at the left of any track, as long as the track's tall enough. You can adjust the track's overall volume with the gain slider also located there. Alternately, you can use the Envelope Tool to reversibly change volume for just part of the track.</p>
    <p>Two caveats: First, if you're listening to someone way off to your left, you'll probably turn to face them, at least part of the way. So <em>you probably don't need to go all the way to 100% left or 100% right</em> when positioning human voices: try 50% and fine-tune from there.</p>
    <p>Second, one risk of layering sounds is "clipping," the kind of crackle or squeal you get if the sound level exceeds what the system can handle. This can especially happen as you layer these sounds together, or amplify them to bring them closer to the listener. If you notice any one waveform hitting the top of the track, or the overall volume going into the red during playback, you're "clipping" part of your sound. Try Effects > Clip Fix, which should give you a little more room.</p>
</details> -->

<details open><summary>Consider removing background noise</summary>
    <p>Sounds recorded in different places often have different levels of background hum, which can make their entrances and exits feel more intrusive. You can mask this with fade-ins/outs – or you can try to <strong>remove the background</strong>.</p>
    <p>Two options there: you can use Audacity's <strong>Noise Reduction</strong> effect (which is easiest if you recorded an extra second or two of "silence" before each take), or you can try to use the <strong>Spectral View</strong> to snip out particular pitches at particular times. Luckily, these are the first two tips in Mike Russell's <a href="https://www.youtube.com/watch?v=ox0NSwdOiyA">"10 Powerful Tips Every Audacity User Should Know"</a>. Well worth your time!</p>
</details>

<details><summary>Consider volume limiters as well as relative volume.</summary>
    <p>Many of you are doing smart work to differentiate foreground sounds from background, in part through "ducking" the background to a lower volume while keeping the sound going to provide depth. (If you're not, but you want to, look for it under <strong>Effects > Volume and Compression > Auto Duck</strong>.) But sometimes, there's just too much sound to hear clearly.</p>
    <p>On the foreground side, one risk of recording original sounds is overloading the microphone, such that you get a kind of crackle or squeal as the sound level exceeds what the system can handle. If you notice this happening in one or two specific spots – you can look for places where the waveform hits the top of the track, or where the volume goes into the red – try <strong>Effects > Clip Fix</strong>, which should give you a little more room.</p>
    <p>If each individual track is fine, and it's just the <em>sum total</em> mix that puts it over the top, <strong>you can apply a Limiter effect to the master track</strong> and it will auto-adjust the overall volume to a manageable level. Click the Effects button at the left of any track; you should see Master at the bottom.</p>
</details>

<details><summary>Consider a soundtrack.</summary>
    <p>Even if your narrative takes place somewhere you wouldn't expect music to actually be audible, a low-key background soundtrack offers a lot of benefits: it covers transitions that would otherwise be silent; it masks differences in background noise across assets and thus helps them seem more like they belong together; and, as we noted when we started this unit, music is great at signaling (or shifting) emotional tone. And it doesn't have to be obtrusive: in most movies, you notice it more when there <em>isn't</em> music playing than when there is.</p>
    <p>Be sure to check out the <a href="../resources#sounds-and-music">Sounds and Music section</a> of the Resources page for tips on where to find openly licensed tracks you can use, including some databases (such as the <a href="https://www.youtube.com/audiolibrary/">YouTube Audio Library</a>) where you can search by mood.</p>
</details>

<details><summary>Consider adding a voiceover layer.</summary>
    <p>Maybe I'm just getting old, but as I've puttered around various places by myself I've noticed that I don't stay silent: I mutter as I putter. Even if it's just short reactions to things I see ("nice!") or read ("really? <em>really</em>."), even if it's not actual words ("hmm."), I tend to narrate my day.</p>
    <p>All of which is to say, if your audio narrative takes your listeners along on a ride inside someone's head, but you haven't yet included any human voices, I'd at least give some thought to whether a word here or there might help. Or maybe the words are <a href="https://www.youtube.com/watch?v=eDEceUWSCIY>only thought, not spoken aloud</p>? You do you.
    <p>Note as well that the voice doesn't have to exist in the same timestream as the events of the narrative: think about some of the retrospective commentary in <a href="https://training.npr.org/2015/10/30/six-npr-stories-that-breathe-life-into-neighborhood-scenes/">the NPR reading I had you do</a>, especially the pieces featuring Steve Inskeep and Robert Siegel. Your narrative, that is, could also have a narrator.</p>
    <p>And if you like any of these ideas, but don't want to deal with hearing your own voice played back, consider swapping scripts with someone else in the class!</p>
</details>

<!-- <details><summary>Aim to blend at most clip entrances and exits</summary>
    <p>Sometimes, you really do want a sound to enter suddenly: a jump-scare, a bolt of lightning, a phone ringing. But more often, you want the new sound to feel like it's part of the same scene. If you want to use music or another kind of background sound to cover transitions, try overlapping the fade-in with the existing scene so as to <strong>minimize dead air</strong>: at a low volume, the effect will be a more seamless / integrated transition.
    </p>
</details> -->

<!-- <details><summary>Consider adding a transcript.</summary>

<p>If you're working off of a script, as a number of you seem to be, please do consider turning it into a readable transcript you can place alongside the sound file: it's not only more accessible for the temporarily or permanently hearing-impaired, but it also makes your piece easier to search for (and within).</p>

<p>I forgot to send an email with examples (I blame this illness), but I can fix that now! NPR's <em>This American Life</em> does a great job, and they're relatively straightforward in format, too. Why not check out some of their <a href="https://www.thisamericanlife.org/recommended">recommended episodes</a>, including a primer for listeners <a href="https://www.thisamericanlife.org/recommended/new-to-this-american-life">new to the show</a> that tipped me off to this <a href="https://www.thisamericanlife.org/109/notes-on-camp">one on camp</a>. (I was excited by this description: <em>"This one drops you in a place and immerses you there so quickly and happily. Just a deeply cheerful trip into childhood summertime."</em>) Or, for something closer to the length of what you'll be working on – a special episode with <a href="https://www.thisamericanlife.org/241/20-acts-in-60-minutes">20 acts in 60 minutes</a>?</p>

<p>You access the transcript from the top of each full episode page, but you can jump to specific sections, or "acts," when choosing what to listen to.</p>
</details> -->

<!--<details><summary>Consider how you'll signal it's over.</summary>
<p>Endings are tricky. In an essay, I'd say they usually depend on beginnings: completing some thought you'd left open, or answering a question. In stories, there's often an epiphany (new insight) or a denouement, a return to a previous situation but with the characters' perspectives on it now changed. You can try those things with audio, too, but there are added elements: if you have music, you can make sure to "resolve" back into the root chord, or to complete a rhythmic sequence; if you have an ongoing event, you can fade out; if you have a surprise or joke ending, you can signal intentionality by muting almost all the backgrounds to draw attention to the one track that remains.</p>
<p>There are lots of ways to do this. But if you're satisfied with the overall shape, endings are one place where you can put a little extra polish in!</p>
</details>-->

<!-- <details><summary>Consider adding a title.</summary>
<p>A title can provide a location, a clue, a genre, a commentary; it can make or unmake listener expectations. What will you call your audio narrative? Where will you let listeners know that name? (In the README? In a recorded introduction to the sound file itself, like on a podcast – either with or without a <a href="https://tvtropes.org/pmwiki/pmwiki.php/Main/TheTeaser?from=Main.ColdOpen">cold open</a>?)</p>
</details> -->




## Okay, now go to!

### Set a goal
What do you want to work on today? Add it to [bit.ly/cdm{{site.course.slugterm}}-notes](https://bit.ly/cdm{{site.course.slugterm}}-notes).

<div class="alert alert-success">
Don't forget to save and commit (and maybe screenshot) as you go!
</div>

<aside class="alert alert-white">
NB: If you're working asynchronously, e.g. making up class because you were out sick, set a timer for one hour.
</aside>

### Exit note
When your time is up, return to the google doc and say how far you got / set new goals for the weekend.


<div style="height:100px; height:10vh;">
<!-- This div left intentionally blank, for spacing -->
</div>

## Homework for next time

* Aiming for 10:00pm on Sunday, but definitely by Monday at noon, **complete – at least for now – your audio narrative.** Your repository (on GitHub, ideally, or in a Box/OneDrive folder shared to me as a fallback) should include:
    - Your most up-to-date layered Audacity project file (.aup3)
    - A flattened, playable export (.mp3)
    - A series, now, of screenshots showing your Audacity project in progress. (Think about what moments are worth remembering as you go: where did you level up, or realize something, or get stuck?)
        * If you need to go back, you can browse the repository at different points in the history and download the project files to reopen them – just be careful not to overwrite your current ones!
    - An updated set of credits (in their own file or just the README) reflecting what you actually used, including documentation of any outside sources and your permission to use them (e.g. explicit licenses like CC – say which one – or fair use).
        * If you use material with a ShareAlike license (CC-BY-SA or CC-BY-NC-SA), add a LICENSE.md file with [the matching license](https://chooser-beta.creativecommons.org/). If you don't have any SA material, this is optional.
    - An updated README.md file introducing your audio narrative to a new audience. Give your piece a title! Make it something to live beyond this assignment, if you can. :¬)


<div class="alert alert-warning">
   If completion to baseline feels impossible from where you are, please talk to me about an extension as soon as you can. That said, we're going to have a similarly rapid pace for the visual argument unit, so the best extension option here may just mean pausing work wherever you are by the weekend, writing a reflection to document your current thinking, and coming back to the project during the Integration​/​Consolidation unit at the end of the term.
</div>

* By Monday at noon, **write a prose reflection** that incorporates images from your feedback and screenshots of your Audacity project. As explained in the [prompt](https://github.com/benmiller314/audio-narrative-{{site.course.slugterm}}#deadlines-and-products), this should include:
   - At least 500 words describing the work you did
   - Your own assessment of how you met the baseline criteria and goals for the unit, as well as  aspirational criteria as appropriate
   - At least one screenshot of feedback you used (and please say how)
   - At least two screenshots of your work in progress (ideally, related to the discussion in the previous two bullets)
* **Post your reflection** to the course site's [Issue queue]({{site.github.issues_url}}), to make it easier to embed images.
   - If you want to then copy the source code into a file in your repo called reflections.md, I won't stop you!
   - If you feel strongly that you'd rather keep your reflection private, you can email it to me instead. But my default assumption is that we learn from each other as much as from ourselves, so I hope you can find a way to write publicly about your experience with this project.
* Relatedly: Want to see a sample reflection? You could do worse than to look at the reflections by the creators of the samples you've already heard, e.g. [Fatema Quaid's](https://github.com/benmiller314/cdm2019fall/issues/3#issuecomment-534351121) retelling of her process on "A Haunted Halt", [Jackie Joo's](https://github.com/benmiller314/cdm2021spring/issues/5#issuecomment-780070186) detailed breakdown of techniques on "Come Over for Dinner", or [Ben Adams's](https://github.com/benmiller314/cdm2023spring/issues/6#issuecomment-1421109922) structured assessment of "Spent on a Rainy Day." I would point out, though, that these are all significantly longer the minimum length. That's not necessary, or expected! But you might treat them as a maximal vision of what you *could* include.
