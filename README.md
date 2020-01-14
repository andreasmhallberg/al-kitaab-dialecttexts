**Todo:**

- Write SA-dalect cognates with SA orthographic, so as not to complicate development of word identification skills.
- Add title in filename and in document
- ~\frenchspacing~ 2019-12-01
- ~uniform YAML headers~ 2019-12-01


This repository contains transcripts of video dialogues from the Arabic textbook *Al-Kitaab fii taʿallum al-ʿarabiyya*, Part&nbsp;1, Third edition. Currently, only the longer dialogues in Damascene (*shaamiyy*) Arabic from chapters 1–8 are included. Transcripts for dialogues in chapter 9–15 will be added this spring. Transcripts for قصة بالعامية texts may be added in the future. The texts are written in pandoc flavored markdown and converted to pdf via [pandoc](http://pandoc.org). Both the markdown files and the pdfs are included in this repository. The videos are available at <http://alkitaabtextbook.com>.

# Background

*Al-Kitaab* includes videos with dialogues in Syrian and Egyptian Arabic. The authors have done a very good job in creating dialogues that feel authentic and are communicatively relevant while being restricted by the grammar and vocabulary of the book. The pedagogical idea behind the inclusion of the videos in the book is for students to improve their listening comprehension of spoken material, and therefore no text is provided. I, however, find a written text to be useful for detailed discussion of the dialogue in the classroom, in that it makes it possible to point at things, look at several places in the text simultaneously, and go through the material slowly and methodically without having to pause and play. You can of course still use the videos to train listening comprehension by having students first listen and extract information from the dialogues, and only thereafter give them the transcript.

# Orthography

The transcripts are written with Arabic script. I have tried to follow the orthographic practices of *Al-Kitaab*, which often follows Standard Arabic orthography, even when I think it is at odds with orthographic practices of written Syrian Arabic (e.g. the 3ms enclitic pronoun is here ـه as in the book rather the conventional ـو). Dialectal phonology is reflected in the spelling some words (e.g. تلاتة) but not in others (e.g. الحقيقة).

# Teaching procedure

*To be added after more experimentation.*

# Generating pdfs

If you want to generate pdfs from the markdown (`.md`) files yourself you need to have [pandoc](http://pandoc.org), the [Scheherazade font](https://software.sil.org/scheherazade/), and a [standard LaTeX distribution](https://ctan.org/starter) installed on your computer. All these are free (beer and freedom). `cd` into the folder containing the markdown files and run the following command:

```
pandoc 〈inputfile〉.md --pdf-engine=xelatex -o 〈outputfile〉.pdf
```

The following is useful to batch convert all markdown files.



