# Transcripts of Syrian Arabic dialogue videos from *Al-Kitaab fii taʿallum al-ʿarabiyya,* Part 1 (3d ed.)

This repository contains transcripts of video dialogues from the Arabic textbook *Al-Kitaab fii taʿallum al-ʿarabiyya*, Part&nbsp;1, Third edition. Currently, only the longer dialogue in Damascene (*shaamiyy*) Arabic from chapter 1--8 are included. Texts for chapter 9--15 will be added this spring. The قصة بالعامية texts may be added in the future. Transcripts were written in markdown and then converted to pdf via [pandoc](http://pandoc.org). Both markdownfiles and pdfs are included in this repository.

## Background

*Al-Kitaab* includes videos with dialogues in Syrian and Egyptian Arabic. The authors have done a very good job in creating dialogues that feel authentic and are communicatively relevant while being restricted by the grammar and vocabulary of the book. It the University of Gothenburg our Arabic program includes a course in Spoken Arabic (currently Syrian) that runs parallel to our course in Standard Arabic. These videos form main part of this course. I have also used these videos, with the procedure described below, in Standard Arabic courses before we had any dedicated course for Spoken Arabic, focusing then on features that contrast with Standard Arabic.

## Orthography

The transcripts are written with Arabic script. I have tried to follow orthographic practices of *Al-Kitaab*, which follows Standard Arabic orthography, even when I think it is at odds with orthographic practices of written Syrian Arabic (e.g. the 3ms enclitic pronoun is here ـه as in the book rather the conventional ـو). Dialectal phonology is reflected in some words (e.g. تلاتة) but not in others (e.g. الحقيقة).

## Teaching procedure

The pedagogical idea behind the inclusion of the videos in the book is for students to improve their listening comprehension of spoken material, and therefore no text is provided. I however feel that a written text is necessary for detailed discussion. This makes it possible to point at things, look at several places in the text simultaneously, etc. I therefore transcribed the texts I use in class.

The procedure is usually the following:

1. Students watch the video at home in preparation for the class.

2. In class, we watch the video once and then discuss what is happening in the scene to make sure that everyone has a rough idea of the contents.

3. I then distribute the transcripts that students read in pairs, instructed to pay attention to certain elements, such as politeness phrases, names of dishes, terms of address, or whatever may be of interest in that particular text. They are also asked to mark things they want to comment or ask about.

4. We discuss the text together with the transcript projected at the whiteboard, focusing on the things they were asked to pay attention to and to things they had noted whilst reading.

I have found that we need at least 45 min. of class time to go through the steps above. If there is more time after the discussion I have students read small sections of the text aloud. The other half of class time (we usually have 2x45 min. classes) is spent on conversation exercises, typically where phrases from the video can be used.

## Generating pdfs

To generate the pdfs from the markdown (`.md`) files you need to have [pandoc](http://pandoc.org), the [Lateef](https://software.sil.org/lateef/) font, and a [standard LaTeX distribution](https://ctan.org/starter) installed on your system. All these are free (beer and freedom). `cd` into this repository and run the following command:

```
pandoc <inputfile>.md --pdf-engine=xelatex -o <outputfile>.pdf
```
