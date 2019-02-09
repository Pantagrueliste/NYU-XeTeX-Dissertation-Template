## NYU-XeTeX-Dissertation-Template

This XeTeX template is designed for New York University doctoral candidates whose dissertation needs to comply with the strict [formatting guidelines](http://gsas.nyu.edu/content/dam/nyu-as/gsas/documents/dissertationsubmissionrelated/Doctoral%20Dissertation%20Formatting%20Requirements%2010-09-15.pdf "formatting guidelines") of the Graduate School of Arts and Sciences. 

### Why would I use a template?

1. You're a busy Ph.D. candidate? Chances are you don't want to waste time with Byzantine format requirements.

2. You work in the humanities? Scholars in the humanities have specific needs, such as unicode compatibility, multilingual support, and advanced typographic features. This template is intended to address all of these needs.

3. NYU GSAS expects a separate list of appendices. This template complies with this requirement, adapting the table of contents to prevent any redundancy.    

### Things you need to verify before using this template

1. Your adviser is ready and willing to work in a format that is fundamentally incompatible with Microsoft Word.
  * You can use pandoc to convert a LaTeX file into a .docx, but you'll not be able to track changes.
  * You can try using diff to compare two .pdf files, but chances are that your adviser neither has the remotest idea of how this might work, nor the time and/or will to learn.

2. You are not thinking of using this template two months before your defense, are you? Make sure you have plenty of time ahead of you to fine tune this template and iron out any potential issue.

3. NYU GSAS has not amended its formatting rules since the creation of this template.
  * If they do, please send me a message.

4. You keep track of changes using Git and you:
  * Write one sentence per line.
  * Divide your dissertation in multiple files.
  * Send commits without moderation.
  * Create [a proper .gitignore file](https://gist.github.com/kogakure/149016 "a proper .gitignore file") to exclude autogenerated files.
  
  ### How to use this template
Dissertation.tex is the parent file. In addition to load all the necessary packages and macros, it defines the format and structure of your dissertation. In accordance with NYU GSAS requirements, it creates the following pages in this specific order: 

1. Title
2. Copyright
3. Dedication
4. Acknowledgments
5. Abstract
6. Table of Contents
7. List of Figures
8. List of Abbreviations
9. List of Appendices.  

Each of these pages may be completed in the apposite section of the parent file. If you don't want a list of Figures or a list of Abbreviations, delete the corresponding sections. However, if you don't need a List of Appendices, you will also need to delete the macro that makes this list appear independently. 

To keep the parent file as concise as possible, all the chapters of your dissertation, including the introduction and the conclusion, are distributed in subdirectories. You can add/retrieve chapters in the parent file.

The Bibliography too is in a separate file and will appear at the end of the dissertation. If you need to separate primary and secondary sources, make sure that your .bib file includes this information.
