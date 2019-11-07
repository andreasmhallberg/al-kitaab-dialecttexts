# Transcripts of Syrian Arabic dialogue videos from *Al-Kitaab fii taʿallum al-ʿarabiyya,* Part 1 (3d ed.)

This repository contains transcripts of video dialogues from the Arabic textbook *Al-Kitaab fii taʿallum al-ʿarabiyya*, Part&nbsp;1, Third edition. Currently, only the longer dialogues in Damascene (*shaamiyy*) Arabic from chapters 1–8 are included. Transcripts for dialogues in chapter 9–15 will be added this spring. Transcripts for قصة بالعامية texts may be added in the future. Transcripts were written in markdown and then converted to pdf via [pandoc](http://pandoc.org). Both the markdown files and the pdfs are included in this repository. The videos are available at <http://alkitabtextbook.com>.

## Background

*Al-Kitaab* includes videos with dialogues in Syrian and Egyptian Arabic. The authors have done a very good job in creating dialogues that feel authentic and are communicatively relevant while being restricted by the grammar and vocabulary of the book. The pedagogical idea behind the inclusion of the videos in the book is for students to improve their listening comprehension of spoken material, and therefore no text is provided. I, however, find a written text to be useful for detailed discussion of the dialogue in the classroom in that it makes it possible to point at things, look at several places in the text simultaneously, and go through the material slowly and methodically without having to pause and play. You can still use them to practice listening comprehension, by using the procedure explained below.

## Orthography

The transcripts are written with Arabic script. I have tried to follow the orthographic practices of *Al-Kitaab*, which follows Standard Arabic orthography, even when I think it is at odds with orthographic practices of written Syrian Arabic (e.g. the 3ms enclitic pronoun is here ـه as in the book rather the conventional ـو). Dialectal phonology is reflected in the spelling some words (e.g. تلاتة) but not in others (e.g. الحقيقة).

## Teaching procedure

The follow is done at the end of the week when we have covered the contents of chapter and students are familiar with the vocabulary. When using these videos in classes I usually follow the following procedure:

1. Students watch the video at home in preparation for the class, guided by the accompanying questions in the book.

2. In class, we watch the video once and then discuss what is happening in the scene to make sure that everyone has a rough idea of the contents.

3. I then distribute the transcripts and have students read them through pairs or groups of three. They are instructed to pay attention to certain elements, such as politeness phrases, names of dishes, terms of address, or whatever may be of interest in that particular text. They are also asked to take notes of any comments or questions they might have, and not to get stuck if they find a certain passage difficult but to try to get through the text in the allotted time.

4. We discuss the text together with the transcript projected on the whiteboard, focusing on the things they were asked to pay attention to and to things they had noted whilst reading.

I have found that you need at least 45 min. of class time to go through the steps above, preferably a bit more. If there is more time after the discussion I have students read small sections of the text aloud.

## Generating pdfs

To generate the pdfs from the markdown (`.md`) files you need to have [pandoc](http://pandoc.org), the [Lateef](https://software.sil.org/lateef/) font, and a [standard LaTeX distribution](https://ctan.org/starter) installed on your system. All these are free (beer and freedom). `cd` into this repository and run the following command:

```
pandoc <inputfile>.md --pdf-engine=xelatex -o <outputfile>.pdf
```
