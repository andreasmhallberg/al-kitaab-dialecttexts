---
title: README
lang: en
author: Andreas Hallberg
papersize: a4
fontsize: 12pt
mainfont: Linux Libertine O
date: \today
header-includes:
    - \newfontfamily\arabicfont[Script=Arabic]{Lateef}
    - \newfontfamily\arabicfontsf[Script=Arabic]{Lateef}
    - \newfontfamily\arabicfontit[Script=Arabic]{Lateef}
    - \frenchspacing
    - \def\UrlFont{\itshape}
---

<!--
- katīr and related with tā
- 3ms attached porn with wāw
-->


This repository contains transcripts of the Syrian Arabic video clips from the Arabic textbook *Al-Kitaab fii taʿallum al-ʿarabiyya*, Part&nbsp;1, Third edition (Brustad et al. 2013, Georgetown University Press). The texts are written in plain text in Pandoc flavored markdown and converted to pdf via [pandoc](http://pandoc.org). Both the markdown files and the pdfs are included in this repository. ~~The videos are available at <http://alkitaabtextbook.com>.~~

`index`-files in various formats provides lists of the files with links to the transcripts and the corresponding videos. This may be useful for lecture plans and the like.

# Background

*Al-Kitaab* includes videos with dialogues in Syrian and Egyptian Arabic. The authors have done a very good job in creating dialogues that feel authentic and are communicatively relevant, while at the same time being restricted by the grammar and vocabulary of the book. The pedagogical idea behind the inclusion of the videos in the book is for students to improve their listening comprehension of spoken material, and therefore no text is provided. I, however, find a written text to be useful for detailed discussion of the dialogues in the classroom, in that it makes it possible to point at things, look at several places in the text simultaneously, and go through the material slowly and methodically without having to pause and play. You can of course still use the videos to have students practice listening comprehension by having students first listen to and extract information from the dialogues, and only thereafter have them read the transcript.

# Orthography

The transcripts are written with Arabic script (i.e., not latinized). I have tried to follow the orthographic practices of *Al-Kitaab*, which often follows Standard Arabic orthography, even when this is at odds with orthographic practices of written Syrian Arabic (e.g. the 3ms enclitic pronoun is here <span lang="ar" dir="rtl">ـه</span> as in the book rather the conventional <span lang="ar" dir="rtl">ـو</span>), although there are inconsistencies. Dialectal phonology is reflected in the spelling some words (e.g. <span lang="ar" dir="rtl">تلاتة</span>) but not in others (e.g. <span lang="ar" dir="rtl">الحقيقة</span>). This is intended to reflect inconsistencies found in authentic written vernacular Arabic.

# Teaching procedure

At the Arabic department at the University of Gothenburg we teach Spoken (Syrian) Arabic in parallel with Standard Arabic. Both courses use *Al-Kitaab*. We typically cover one chapter each week, with the Standard Arabic material in the chapter covered Monday through Thursday, and the Syrian Arabic material covered on Friday. Students are then familiar with the basic vocabulary of the chapter when they are presented with the Syrian Arabic texts.

For the Spoken Arabic classes, students are provided with the transcript before class and are given the following instructions:

1. View the video several times without looking at the transcript. Pause and listen again to sections if you need to.

2. Try to answer the questions for the corresponding activity in the book, still without looking at the transcript.

3. Watch the video again, this time with the printed transcript at hand. Take notes of comments or questions and bring to class.

In class, we do the following:

1. We watch the video together to refresh our memory.

2. One student gives a short summary of the video in their own language (i.e., not in Arabic).

3. The transcript is projected on the whiteboard for ease of reference.

4. We discuss students' question, and I (the teacher) make further comments if needed. Much of this discussion is typically focused on pragmatics.

The procedure above usually take around 45 min. During the rest of the class (another 45 min) we do conversation exercises based on the vocabulary and phrases in the text.

# Generating pdfs

To generate pdfs from the markdown (`.md`) files you need to have [pandoc](http://pandoc.org), the [Scheherazade font](https://software.sil.org/scheherazade/), and a [standard LaTeX distribution](https://ctan.org/starter) installed on your system. All these are free (beer and freedom). To generate the pdfs, run the following command in the root directory of this repository:

```
pandoc 〈inputfile〉.md --pdf-engine=xelatex -o 〈outputfile〉.pdf
```
