---
name: pdf-to-latex
description: Decompile a PDF into LaTex to make it easier to understand for Agents
disable-model-invocation: true
user-invocable: true
metadata:
  author: paperbenni
  version: "0.1.1"
  opencode/slash: "true"
  opencode/autoinvoke: "false"
---

Agents are better at understanding and navigating LaTeX source code than they are at understanding compiled LaTeX. 

I want you to convert a PDF file to LaTeX in order to make it easier for Agents
to read. If the file is long and has structure, then create a sensible folder
structure with individual files for the sections/chapters/helpers/whatever.
Short PDF files can go in a single.tex file. Regularly compile your LaTeX and
compare with the original to catch mistakes in your decompilation.  

If the PDF is really long, then create the rough structure and then dispatch
subagents to convert individual parts into LaTeX. 

If the PDF was not created with modern LaTeX and instead is an old scan of a
paper book, then you might have to resort to reading images (if you are an image
model). Keep in mind that images in the context increase the size of your calls,
so reading them to often might make your request size so big that the session no
longer works. For that reason, dispatch subagents for reading a collection of
images and have the subagent return a LaTeX conversion or textual
understanding/summary to you instead of reading the images yourself. 

In the case the PDF was not originally created with LaTeX, I don't want you to
recreate the exact styling of the original, I care more about the actual content
and meaning. The original style might also have been odd, while modern latex is
more pleasant to read. 


After you're finished, the original PDF should be called something like
..._original.pdf to make it clear it is not the one Agents should be looking at,
and the decompilation should be done in a way were agents can quickly understand
the contents and answer questions or wishes the user has about the original PDF. 

