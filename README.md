**Todo:**

- Write SA-dialect cognates with SA orthography, so as not to complicate development of word identification skills.
- Add title in file name and in document
- ~\frenchspacing~ 2019-12-01
- ~uniform YAML headers~ 2019-12-01

<!--
- katīr and related with tā
- 3ms attached porn with wāw
-->


This repository contains transcripts of the Syrian dialectal video dialogues from the Arabic textbook *Al-Kitaab fii taʿallum al-ʿarabiyya*, Part&nbsp;1, Third edition. The texts are written in pandoc flavored markdown and converted to pdf via [pandoc](http://pandoc.org). Both the markdown files and the pdfs are included in this repository. The videos are available at <http://alkitaabtextbook.com>.

# Background

*Al-Kitaab* includes videos with dialogues in Syrian and Egyptian Arabic. The authors have done a very good job in creating dialogues that feel authentic and are communicatively relevant while being restricted by the grammar and vocabulary of the book. The pedagogical idea behind the inclusion of the videos in the book is for students to improve their listening comprehension of spoken material, and therefore no text is provided. I, however, find a written text to be useful for detailed discussion of the dialogue in the classroom, in that it makes it possible to point at things, look at several places in the text simultaneously, and go through the material slowly and methodically without having to pause and play. As a teacher, you can of course still use the videos to practice listening comprehension, by having students first listen to and extract information from the dialogues, and only thereafter give them the transcript.

# Orthography

The transcripts are written with Arabic script. I have tried to follow the orthographic practices of *Al-Kitaab*, which often follows Standard Arabic orthography, even when this is at odds with orthographic practices of written Syrian Arabic (e.g. the 3ms enclitic pronoun is here ـه as in the book rather the conventional ـو), although there are inconsistencies. Dialectal phonology is reflected in the spelling some words (e.g. تلاتة) but not in others (e.g. الحقيقة).

# Teaching procedure

At the Arabic department at the University of Gothenburg, where I teach, we teach Spoken (Syrian) Arabic in parallel with Standard Arabic. Both courses use *Al-Kitaab*. We typically cover one chapter each week, with the class in Syrian Arabic at the end  if the week, covering the same material that was covered during the week in the Standard Arabic classes.

For Spoken Arabic, students are provided with the manuscript before class and are given the following instructions:

1. View the corresponding video several times without looking at the manuscript. Pause and listen again to sections if you need to.

2. Try to answer the questions in the book, still without looking at the manuscript.

3. Watch the video again with the manuscript at hand. Take notes of comments or questions, and bring to class.

In class, we do the following:

1. We watch the video together to refresh our memory of it.

2. One student gives a short summary of the video in their own language (i.e., not in Arabic).

3. The transcript is projected on the whiteboard for ease of reference.

4. We discuss students' question, an I (the teacher) make further comments if needed.

5. Depending on time, students take turns to read sections of the text aloud.

The procedure above usually take 30-45 min. The rest of the class (another 45 min) we do conversation exercises based on the vocabulary and phrases in the text.

# Generating pdfs

If you want to generate pdfs from the markdown (`.md`) files yourself you need to have [pandoc](http://pandoc.org), the [Scheherazade font](https://software.sil.org/scheherazade/), and a [standard LaTeX distribution](https://ctan.org/starter) installed on your computer. All these are free. `cd` into the folder containing the markdown files and run the following command:

```
pandoc 〈inputfile〉.md --pdf-engine=xelatex -o 〈outputfile〉.pdf
```
