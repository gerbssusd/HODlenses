---
theme: seriph
title: "Applying the Lenses: Heart of Darkness"
favicon: "Maxfav.png"
info: |
  Twenty critical lenses applied to Joseph Conrad's Heart of Darkness (1899), with MLA sources.
author: D. Gerber
layout: cover
class: text-left
background: '#191512'
transition: slide-left
mdc: true
drawings:
  persist: false
fonts:
  serif: Fraunces
  sans: Source Serif 4
  provider: google
  weights: '400,600,700'
  italic: true
aspectRatio: 16/9
canvasWidth: 980
exportFilename: heart-of-darkness-lenses
download: false
---

<div class="grid grid-cols-[1.5fr_1fr] gap-10 items-center h-full">
<div>
<p class="kicker">Twenty Critical Lenses · One Novella</p>

# Applying the Lenses: *Heart of Darkness*

Joseph Conrad, 1899

</div>
<figure class="m-0">
  <div class="portrait h-[330px]"><img src="https://commons.wikimedia.org/wiki/Special:FilePath/Joseph_Conrad%2C_Fotografie_von_George_Charles_Beresford%2C_1904.jpg?width=1600" alt="Photographic portrait of Joseph Conrad in 1904" style="object-position: 50% 20%" /></div>
  <p class="caption" style="color:#cbbfa8">Joseph Conrad, by George Charles Beresford, 1904 · Public domain</p>
</figure>
</div>

<!--
Welcome. In this presentation we apply twenty critical lenses to a single, endlessly contested text: Joseph Conrad's novella Heart of Darkness. Our goal is not to settle what the book means, but to see how each lens produces a different, arguable question about it.
-->

---

<p class="kicker">Context</p>

# From the Congo to the Page

<div class="grid grid-cols-3 gap-6 mt-8">
<div class="fact-card">
  <p class="year">1890</p>
  <p>Józef Teodor Konrad Korzeniowski travels up the Congo River for a Belgian trading company and briefly commands the steamer <em>Roi des Belges</em>.</p>
</div>
<div class="fact-card">
  <p class="year">1899</p>
  <p><em>Heart of Darkness</em> is serialized in <em>Blackwood's Magazine</em>.</p>
</div>
<div class="fact-card">
  <p class="year">Today</p>
  <p>The novella remains one of the most contested texts in the canon (Achebe).</p>
</div>
</div>

<SteamerLine class="mt-8" />

<style>
.fact-card { background: var(--c-card); border: 1px solid var(--c-rule); border-radius: 14px; padding: 1rem 1.1rem; box-shadow: 0 12px 26px -20px rgba(0,0,0,.7); }
.fact-card .year { font-family: var(--font-head); font-size: 2.4rem; font-weight: 700; color: var(--c-oxblood); margin: 0 0 .2rem !important; line-height: 1; }
.fact-card p { font-size: .9rem; margin: 0; }
</style>

<!--
First, some context. In 1890, Conrad, born Józef Teodor Konrad Korzeniowski, traveled up the Congo River in the service of a Belgian trading company and briefly took command of a river steamer, the Roi des Belges. He returned to Europe in poor health. Nine years later, in 1899, he published Heart of Darkness, serialized in Blackwood's Magazine. The novella's route, from the coast up to the Inner Station, follows the river he had traveled himself.
-->

---
clicks: 4
---

<p class="kicker">The Journey</p>

# Marlow's Route

<div class="grid grid-cols-[1fr_2.1fr] gap-8 items-center mt-2">
<div class="text-[0.95rem] leading-relaxed text-[var(--c-ink-2)]">
The novella's geography follows the river Conrad traveled, though the text never names Belgium, the Congo, or Brussels (Conrad).

<p class="mt-6 italic">"Going up that river was like travelling back to the earliest beginnings of the world" (Conrad).</p>
</div>
<RiverRoute :step="$clicks" />
</div>

<!--
Here is Marlow's journey as the novella stages it.

[click] He begins at the Company's offices in a European city that the text never names, where two women knit black wool at the door.

[click] He lands at the Outer Station on the coast, where he first witnesses the violence of the enterprise.

[click] He waits months at the Central Station, repairing a sunken steamer amid rumors about Kurtz.

[click] And finally he reaches the Inner Station, deep in the interior, where he finds Kurtz dying.
-->

---
clicks: 3
layout: two-cols
layoutClass: gap-8
---

<p class="kicker">How the Story Is Told</p>

# A Tale Within a Tale

<div class="portrait h-[200px] mt-4">
  <img src="https://commons.wikimedia.org/wiki/Special:FilePath/The_Thames_below_Westminster.jpg?width=1600" alt="Monet's misty painting of the Thames with boats and Westminster" />
</div>
<p class="caption">Claude Monet, <em>The Thames below Westminster</em>, c. 1871 · Public domain</p>

<p class="text-[0.95rem] mt-4">Every lens must look through three layers of narration.</p>

::right::

<FrameNarrative :step="$clicks" />

<!--
Before we choose a lens, notice how the story is told.

[click] On the outside, an unnamed narrator sits aboard a yawl, the Nellie, anchored on the Thames.

[click] Inside that frame, Marlow tells the story of his voyage.

[click] And at the center is Kurtz, whom we meet only through Marlow's memory, and whose voice reaches us at two removes. Every lens we use must look through these three layers.
-->

---
layout: statement
---

<p class="kicker text-center">Method</p>

# One Lens · One Question · One Essay

<p class="text-lg italic text-[var(--c-ink-2)] mt-4">Read with the lens's focus in mind, then pose a single arguable question the lens makes visible.</p>

<!--
Our method is simple. Choose one lens. Read the novella with that lens's focus in mind. Then pose a single, arguable question that the lens makes visible. On the following slides, each group of lenses appears with its focus and a question about Heart of Darkness that you could develop into an essay.
-->

---

<p class="kicker">Group 1 of 6</p>

# Empire, Race, and Culture

<div class="grid grid-cols-[2.2fr_1fr] gap-6 mt-3 items-start">
<div class="grid grid-cols-2 gap-3">
  <LensCard v-click name="Postcolonialism" color="var(--c-oxblood)" focus="Imperial domination, &quot;othering,&quot; and fractured identity (Said)." question="Does the novella indict colonial greed, or reduce Africans to a &quot;primitive&quot; backdrop for Marlow's journey? (Siegel; &quot;Critical Lenses&quot;; ben)" />
  <LensCard v-click name="Critical Race Theory" color="var(--c-oxblood)" focus="How texts reinforce or challenge systemic racism." question="Test Achebe's charge that Conrad was &quot;a thoroughgoing racist&quot; against the novella's imagery of light and dark (Achebe; &quot;Critical Lenses for Heart&quot;)." />
</div>
<figure class="m-0"><div class="portrait h-[300px]"><img src="https://commons.wikimedia.org/wiki/Special:FilePath/Punch_congo_rubber_cartoon.jpg?width=1600" alt="Cartoon of a snake with King Leopold's head coiling around a Congolese man" /></div><p class="caption">Edward Linley Sambourne, “In the Rubber Coils,” <em>Punch</em>, 1906 · Public domain</p></figure>
</div>

<!--
We begin with empire, race, and culture.

[click] Postcolonial criticism, following Edward Said, asks how imperial powers represent the colonized. Does Conrad's novella indict European greed, or does it reduce Africans to a primitive backdrop for a European's psychological drama?

[click] Critical race theory sharpens that question. In a famous lecture, the Nigerian novelist Chinua Achebe called Conrad a thoroughgoing racist. Students can test that charge against the novella's racial hierarchies and its imagery of light and darkness.
-->

---

<p class="kicker">Group 2 of 6</p>

# Power, Gender, and Economics

<div class="grid grid-cols-3 gap-4 mt-3">
  <LensCard v-click name="Marxism" color="var(--c-teal)" focus="Class, accumulation, and economic power (Eagleton)." question="How does the Company's pursuit of ivory exploit African laborers and lower-ranking agents alike? (&quot;Literary Theory and Schools&quot;; ben)" />
  <LensCard v-click name="Feminism" color="var(--c-teal)" focus="Patriarchy and the marginalization of women (Gilbert and Gubar)." question="Marlow says women &quot;should be out of it&quot; (Conrad). Compare the Intended with Kurtz's African mistress (Siegel; &quot;Critical Lenses&quot;)." />
  <LensCard v-click name="Gender and Queer Theory" color="var(--c-teal)" focus="Homosocial bonds in male-dominated spaces (Sedgwick)." question="Why does Marlow crave the approval of a dying tyrant? (Coon)" />
</div>

<!--
Next, power, gender, and economics.

[click] A Marxist reading treats the Company as a capitalist machine, and asks how the pursuit of ivory exploits African laborers and lower-ranking European agents alike.

[click] A feminist reading begins with Marlow's claim that women should be out of it, kept in a beautiful world of their own. Compare Kurtz's Intended in Europe with his African mistress, and ask how gender allocates power and knowledge.

[click] And gender and queer theory examine the bond between Marlow and Kurtz. Why does Marlow seek the approval of a dying tyrant?
-->

---

<p class="kicker">Group 3 of 6</p>

# Mind and Myth

<div class="grid grid-cols-[2.2fr_1fr] gap-6 mt-3 items-start">
<div class="grid grid-cols-2 gap-3">
  <LensCard v-click name="Psychoanalytic" color="var(--c-ochre)" focus="Repression and the unconscious (Freud)." question="Is the journey upriver a descent into the unconscious, and Kurtz the unchecked id? (&quot;Critical Lenses for Heart&quot;)" />
  <LensCard v-click name="Archetypal / Jungian" color="var(--c-ochre)" focus="Recurring myths and character types (Frye)." question="Marlow descends to the underworld; the two women knitting black wool become the Fates (&quot;Critical Lenses for Heart&quot;)." />
</div>
<figure class="m-0"><div class="portrait h-[300px]"><img src="https://commons.wikimedia.org/wiki/Special:FilePath/Gustave_Dor%C3%A9_-_Dante_Alighieri_-_Inferno_-_Plate_9_%28Canto_III_-_Charon%29.jpg?width=1600" alt="Engraving of Charon the ferryman on a dark river with souls crowding the shore" /></div><p class="caption">Gustave Doré, <em>Charon</em>, illustration for Dante's <em>Inferno</em>, 1861 · Public domain</p></figure>
</div>

<!--
Now, the lenses of mind and myth.

[click] A psychoanalytic reading follows the river inward. Is the journey upriver a descent into the unconscious, and is Kurtz a figure wholly consumed by the unchecked id?

[click] An archetypal reading sees Marlow's voyage as a descent into the underworld. Kurtz becomes a fallen god, and the two women knitting black wool at the Company's door become the Fates.
-->

---

<p class="kicker">Group 4 of 6</p>

# Language, Form, and Philosophy

<div class="grid grid-cols-3 gap-4 mt-3">
  <LensCard v-click name="New Criticism / Formalism" color="var(--c-indigo)" focus="Close reading of diction, motif, and syntax (Brooks)." question="How does the fog on the river produce paralyzing ambiguity? (&quot;New Criticism&quot;; Siegel)" />
  <LensCard v-click name="Deconstruction" color="var(--c-indigo)" focus="Collapsing binary oppositions (Derrida)." question="How does &quot;civilized&quot; Europe come to look dark and savage? (ben; Coon)" />
  <LensCard v-click name="Existentialism" color="var(--c-indigo)" focus="Meaning in an indifferent universe." question="Read &quot;The horror! The horror!&quot; (Conrad) as a recognition of the void (Siegel)." />
</div>

<!--
Next, language, form, and philosophy.

[click] A formalist reading isolates a single passage, such as the fog that blinds the steamer, and shows how diction, motif, and syntax create a sense of paralyzing ambiguity.

[click] A deconstructive reading presses on the novella's binaries, savage and civilized, light and dark, until civilized Europe itself appears dark and savage.

[click] And an existentialist reading hears in Kurtz's last words, The horror! The horror!, a recognition of the void beneath human ambition.
-->

---

<p class="kicker">Group 5 of 6</p>

# Context and the Reader

<div class="grid grid-cols-3 gap-4 mt-3">
  <LensCard v-click compact name="New Historicism" color="var(--c-olive)" focus="Texts among texts; erased voices (Greenblatt)." question="Read the novella beside records of Leopold II's Congo Free State (ben; Coon)." />
  <LensCard v-click compact name="Ecocriticism" color="var(--c-olive)" focus="The environment as active force (Glotfelty and Fromm)." question="Is the jungle scenery, or a living antagonist? (Coon)" />
  <LensCard v-click compact name="Reader-Response" color="var(--c-olive)" focus="Meaning as transaction with readers (Fish)." question="Does Kurtz mean differently to a reader in 1899 and a reader today?" />
  <LensCard v-click compact name="Biographical" color="var(--c-olive)" focus="The author's life as evidence (Abrams and Harpham)." question="Where does Korzeniowski end and Marlow begin?" />
  <LensCard v-click compact name="Cultural Studies" color="var(--c-olive)" focus="Literature beside popular media (Barry)." question="Does the novella answer or echo the &quot;civilizing mission&quot; propaganda?" />
</div>

<!--
Our fifth group places the novella in context and in the hands of readers.

[click] New Historicism reads the novella beside records of King Leopold the Second's Congo Free State. Does the fiction subvert the colonial propaganda of the eighteen nineties, or uphold it?

[click] Ecocriticism treats the jungle not as scenery but as a living antagonist that resists European machinery.

[click] Reader-response criticism asks how Kurtz means differently to a reader in 1899 and a reader today.

[click] Biographical criticism uses Conrad's Congo diary to ask where Korzeniowski ends and Marlow begins.

[click] And cultural studies asks whether the novella answers, or echoes, the speeches and advertisements that sold empire as a civilizing mission.
-->

---

<p class="kicker">Group 6 of 6</p>

# Ethics, Narrative, and Intertext

<div class="grid grid-cols-[3.4fr_1fr] gap-6 mt-3 items-start">
<div class="grid grid-cols-3 gap-3">
  <LensCard v-click compact name="Moral / Philosophical" color="var(--c-plum)" focus="Ethical inquiry (Abrams and Harpham)." question="Is depravity what remains when restraint is removed, or is civilization the lie?" />
  <LensCard v-click compact name="Semiotics" color="var(--c-plum)" focus="Signs and difference (Saussure)." question="How does &quot;ivory&quot; come to signify greed, status, and death?" />
  <LensCard v-click compact name="Narratology" color="var(--c-plum)" focus="Layers of narration and reliability." question="Why filter the truth through three narrative layers?" />
  <LensCard v-click compact name="Disability Studies" color="var(--c-plum)" focus="Illness, madness, and the body (Garland-Thomson)." question="Is Kurtz's wasting body only a metaphor for his soul?" />
  <LensCard v-click compact name="Intertextuality" color="var(--c-plum)" focus="Texts woven from earlier texts." question="How does Marlow's journey echo Dante's Inferno and Virgil's Aeneid?" />
</div>
<figure class="m-0"><div class="portrait h-[250px]"><img src="https://commons.wikimedia.org/wiki/Special:FilePath/Gustave_Dor%C3%A9_-_Dante_Alighieri_-_Inferno_-_Plate_8_%28Canto_III_-_Abandon_all_hope_ye_who_enter_here%29.jpg?width=1600" alt="Engraving of Dante and Virgil before the gate of Hell" /></div><p class="caption">Gustave Doré, <em>Abandon All Hope</em>, illustration for Dante's <em>Inferno</em>, 1861 · Public domain</p></figure>
</div>

<!--
Finally, ethics, narrative, and intertext.

[click] A moral reading asks whether depravity is what remains when society's restraints are removed, or whether civilization itself is the lie.

[click] A semiotic reading maps how the word ivory comes to signify greed, status, blindness, and death.

[click] A narratological reading asks why Conrad filters the truth through three layers of narration.

[click] Disability studies asks whether Kurtz's wasting body is only a metaphor for a decaying soul, or a body in its own right.

[click] And an intertextual reading traces Marlow's journey back to Dante's Inferno and Virgil's Aeneid.
-->


---

<p class="kicker">One Word, Many Lenses</p>

# Following "Ivory"

<div class="ivory mt-6">
  <div class="hub">ivory</div>
  <div class="spoke" style="--c: var(--c-ochre)"><h3>The Company</h3><p>profit; the reason for the voyage</p></div>
  <div class="spoke" style="--c: var(--c-oxblood)"><h3>Marxist lens</h3><p>the commodity that organizes all labor</p></div>
  <div class="spoke" style="--c: var(--c-teal)"><h3>Semiotic lens</h3><p>a drifting sign: wealth, idol, and Kurtz's bald head, "an ivory ball" (Conrad)</p></div>
</div>

<style>
.ivory { display: grid; grid-template-columns: 1fr 1fr 1fr; gap: 1.2rem; position: relative; }
.ivory .hub { grid-column: 1 / -1; justify-self: center; font-family: var(--font-head); font-size: 2.6rem; font-style: italic; color: #fbf7ef;
  background: radial-gradient(circle at 30% 30%, #4a3f33, #191512); padding: .6rem 2.4rem; border-radius: 999px; box-shadow: 0 18px 30px -18px rgba(0,0,0,.8); }
.ivory .spoke { background: var(--c-card); border-radius: 14px; padding: 1rem; border: 1px solid var(--c-rule); position: relative; }
.ivory .spoke::before { content: ''; position: absolute; top: -1.2rem; left: 50%; width: 2px; height: 1.2rem; background: var(--c); }
.ivory .spoke h3 { color: var(--c) !important; font-size: 1.15rem !important; margin: 0 0 .3rem !important; }
.ivory .spoke p { margin: 0; font-size: .9rem; }
</style>

<!--
To see how much a single lens can do, follow one word: ivory. To the Company, ivory is profit. To a Marxist critic, it is the commodity that organizes all labor in the novella. To a semiotician, it is a sign whose meaning drifts, from wealth, to idol, to the color of Kurtz's own bald head, which Marlow compares to an ivory ball. One word, three lenses, three essays.
-->

---
layout: center
---

<p class="kicker text-center">From Lens to Thesis</p>

# A Sample Thesis

<div class="claim mt-6 max-w-[800px]">
Read through <span class="slot" style="background:var(--c-teal)">a narratological lens</span>,
the novella's <span class="slot" style="background:var(--c-ochre)">three layers of narration</span>
do not clarify Kurtz but <span class="slot" style="background:var(--c-oxblood)">deliberately obscure him</span>, implicating every listener, including us, in Marlow's lie to the Intended.
</div>

<!--
Here is how a lens becomes a thesis. Name the lens, name the textual feature, and state the claim that lens makes visible. For example: read through a narratological lens, the novella's three layers of narration do not clarify Kurtz but deliberately obscure him, implicating every listener, including us, in Marlow's lie to the Intended. That claim is arguable, specific, and grounded in the text.
-->

---
class: wc
---

<h1 class="wc-title">Works Cited</h1>

<div class="works-cited">

Abrams, M. H., and Geoffrey Galt Harpham. *A Glossary of Literary Terms*. 11th ed., Cengage Learning, 2015.

Achebe, Chinua. “An Image of Africa: Racism in Conrad’s *Heart of Darkness*.” *Hopes and Impediments: Selected Essays*, Anchor Books, 1989, pp. 1–20.

Barry, Peter. *Beginning Theory: An Introduction to Literary and Cultural Theory*. 4th ed., Manchester UP, 2017.

ben \[@fangedbobo\]. “Joseph Conrad’s *Heart of Darkness*: A Critical Review.” *Medium*, 11 Dec. 2022, medium.com/@fangedbobo/joseph-conrads-heart-of-darkness-a-critical-review-a70486dce176. Accessed 16 Oct. 2026.

Beresford, George Charles. *Joseph Conrad*. 1904. Photograph. *Wikimedia Commons*, commons.wikimedia.org/wiki/File:Joseph\_Conrad,\_Fotografie\_von\_George\_Charles\_Beresford,\_1904.jpg. Accessed 16 Oct. 2026.

Brooks, Cleanth. *The Well Wrought Urn: Studies in the Structure of Poetry*. Reynal and Hitchcock, 1947.

Conrad, Joseph. *Heart of Darkness*. Edited by Paul B. Armstrong, 5th ed., W. W. Norton, 2017. Norton Critical Edition.

Coon, Brandon. “Critical Lenses.” *CoonWriting*, www.coonwriting.com/critical-lenses.html. Accessed 16 Oct. 2026.

“Critical Lenses for *Heart of Darkness*.” *English with Mrs. Lamp*, 11 June 2024, englishwithmrslamp.com/2024/06/11/critical-lenses-for-heart-of-darkness/. Accessed 16 Oct. 2026.

“Critical Lenses.” *Classroom of Mrs. Baltsas*, Google Sites, sites.google.com/cps.edu/theclassroomofmrsbaltsas/critical-lenses. Accessed 16 Oct. 2026.

Derrida, Jacques. *Of Grammatology*. Translated by Gayatri Chakravorty Spivak, Johns Hopkins UP, 1976.

</div>

<!--
The following slides list the works cited in this presentation, formatted in MLA style.
-->

---
class: wc
---

<h1 class="wc-title">Works Cited (continued)</h1>

<div class="works-cited">

Doré, Gustave. *Abandon All Hope Ye Who Enter Here*. Illustration for Dante Alighieri’s *Inferno*, canto 3, 1861. *Wikimedia Commons*, commons.wikimedia.org/wiki/File:Gustave\_Doré\_-\_Dante\_Alighieri\_-\_Inferno\_-\_Plate\_8\_(Canto\_III\_-\_Abandon\_all\_hope\_ye\_who\_enter\_here).jpg. Accessed 16 Oct. 2026.

Doré, Gustave. *Charon*. Illustration for Dante Alighieri’s *Inferno*, canto 3, 1861. *Wikimedia Commons*, commons.wikimedia.org/wiki/File:Gustave\_Doré\_-\_Dante\_Alighieri\_-\_Inferno\_-\_Plate\_9\_(Canto\_III\_-\_Charon).jpg. Accessed 16 Oct. 2026.

Eagleton, Terry. *Marxism and Literary Criticism*. U of California P, 1976.

Fish, Stanley. *Is There a Text in This Class? The Authority of Interpretive Communities*. Harvard UP, 1980.

Freud, Sigmund. *The Interpretation of Dreams*. Translated by James Strachey, Basic Books, 2010.

Frye, Northrop. *Anatomy of Criticism: Four Essays*. Princeton UP, 1957.

Garland-Thomson, Rosemarie. *Extraordinary Bodies: Figuring Physical Disability in American Culture and Literature*. Columbia UP, 1997.

Gilbert, Sandra M., and Susan Gubar. *The Madwoman in the Attic: The Woman Writer and the Nineteenth-Century Literary Imagination*. Yale UP, 1979.

Glotfelty, Cheryll, and Harold Fromm, editors. *The Ecocriticism Reader: Landmarks in Literary Ecology*. U of Georgia P, 1996.

Greenblatt, Stephen. *Renaissance Self-Fashioning: From More to Shakespeare*. U of Chicago P, 1980.

“Literary Theory and Schools of Criticism.” *Benton English*, bentonenglish.com/wp-content/uploads/2014/02/literary-criticism.pdf. Accessed 16 Oct. 2026.

</div>

<!--
The list of works cited continues on this slide.
-->

---
class: wc
---

<h1 class="wc-title">Works Cited (continued)</h1>

<div class="works-cited">

Monet, Claude. *The Thames below Westminster*. c. 1871. National Gallery, London. *Wikimedia Commons*, commons.wikimedia.org/wiki/File:The\_Thames\_below\_Westminster.jpg. Accessed 16 Oct. 2026.

“New Criticism.” *Mural*, Universitat de València, mural.uv.es/jadiazso/newcriticism. Accessed 16 Oct. 2026.

Said, Edward W. *Orientalism*. Pantheon Books, 1978.

Sambourne, Edward Linley. “In the Rubber Coils.” *Punch*, 28 Nov. 1906. *Wikimedia Commons*, commons.wikimedia.org/wiki/File:Punch\_congo\_rubber\_cartoon.jpg. Accessed 16 Oct. 2026.

Saussure, Ferdinand de. *Course in General Linguistics*. Translated by Wade Baskin, edited by Perry Meisel and Haun Saussy, Columbia UP, 2011.

Sedgwick, Eve Kosofsky. *Epistemology of the Closet*. U of California P, 1990.

Siegel, Kristi. “Introduction to Modern Literary Theory.” *Kristi Siegel*, www.kristisiegel.com/theory2.htm. Accessed 16 Oct. 2026.

</div>

<!--
The list of works cited concludes on this slide.
-->


---
layout: end
---

<p class="kicker">Choose · Ask · Return to the Text</p>

# Thank You

<!--
One novella, twenty lenses, and countless arguments. Choose your lens, ask its question, and return to the text. Thank you.
-->
