# Plain Text and git for group project

[TOC]

## Intro

I began this project, when my group startet splitting our documents into smaller Google Docs documents, to be combined into Word docx' once in a while. This was a huge mess, with inconsistent indenting and paragraphs included in the table of content, and I feel there's a much better way. So this article aims to help me in future projects, as well as others who might find similar issues.

### What is Plain Text

To understand plain text, one has to understand rich text. Rich text is text that has formatting magically hidden from you, Word and Google docs comes to mind as text editors, which uses rich text. So plain text is only "plain" characters, with no hidden data as to how it should be displayed graphically.

### But Why

I've heard once, that a lector at my university was dissatisfied with a website in out system was dissatisfied with the fact, that it's plain text, and doesn't have a wisywig editor. The lector felt that plain text is old school. But big systems uses plain text formatting, reddit, squarespace and even Facebook Messenger on the web allows for plain text formatting.

Writing your projects in plain text has a few advantages. First off, it's plain, so if you copy something from another document, with a different formatting, then the other format won't have a negative impact on the document you're currently writing. Paired with the right plain text processor, you get to organise your project in files, instead of having one monolith, which can help with focusing on the segment you're currently writing on, instead of jumping around the entire project.

If you're into open science, you can have your projects on [GitHub](github.com), or other such sites, and have your project on display, and even receive input from other authors. More on this later.

## You Can Still Do Formatting

Plaintext doesn't necessarily mean there's no formatting. If you've been around me long enough, you've probably heard me mention Markdown, which is a great formatting tool for begginners. There's also LaTeX, and I've recently taken a liking to various versions of roff.

This article assumes no prior plaintext editing knowledge and will continue with markdown, as it has the simplest syntax, that's readable even when editing, yet, with the right preprocessor, has the same flexibility of LaTeX.

### Software And Formatting

There's a few formatting languages that's well suited for documents, and each of these languages has their own sets of software and processors, each with a variyng degree of difficulty of use and accessibility.

#### Markdown

The beforementioned This article itself is written entirely in Markdown and uses git for version control. On my Mac I write in Sublime Text, and on any other device I use IA Writer, these software are paid, and there are a tonnes of great _free_ software. For Windows [MarkPad](http://code52.org/DownmarkerWPF/) looks pretty great. Before using IA Writer, I used [Typora](https://typora.io) and is easily the editor I recommend anyone who want to do a deep dive into Markdown.

Typora is backed by [Pandoc](http://support.typora.io/Install-and-Use-Pandoc/), meaning you can do some truly powerfull stuff with it. By dipping down to [the terminal](https://tex.stackexchange.com/a/298385), you can even do advanced and beautiful referencing. I'll get into terminal stuff later, and this article should be good even without the terminal. 

#### LaTeX 

I can only recommend going forward with LaTeX when comfortable with plaintext editing. LaTeX is much more powerful than Markdown, but also has a more complex syntax to do simple stuff.

In terms of software, I can only recommend [Overleaf](https://www.overleaf.com). Overleaf also allows local editing with git, if someone in your group _really_ loves that on software they use, or you need to edit without internet.

#### roff

On Unix based systems, such as macOS, roff is preinstalled, and I highly encourage people more adept with the terminal to at least check it out. On most systems roff is called groff, some systems do have troff instead. I haven't found a way to use roff on Windows, and would by no means recommend it to people who aren't adept using the terminal.

## Calloboration With Git

Git is a version control and calloboration system _made_ for code, which are inherently plaintext, making it a great tool for this purpose. Even if you're writing on your own, git still is a great version control system, so you can see your changes through the history of the project.

In terms of collaboration, git gives powerfull tools such as diff, a tool to see changes, blame, which tells you who wrote what, so you can ask them for clarifications.

The nature of git is so, that each writer has a local copy of their work, and they push to a remote repository, as they are called, whith all the changes, and once in a while each writer has to pull the changes. This may seem cumbersome at first, but once one is used to pull before beginning to write, and push every now and then, it will soon feel natural. The biggest advantage of this is, everyone can write on their parts, without having to make sure everyone is up to date with the right Word document, or obstruct eachothers view by making new lines all the time in Google docs.

### Git Clients

There's a bunch of great git clients, and my favourties are [Fork](https://fork.dev) for Mac and Windows and [WorkingCopy](https://apps.apple.com/us/app/working-copy/id896694807?ign-mpt=uo%3D6) for iOS. I unfortunately don't know any good GUI clients for either Android or Linux, so there I have to ask you to look yourself. On Unix based systems such as Linux and Mac, you can look at the cli git tools, which are great nonetheless.

Fork allows the user to specify which part of the edits to include and exclude, cherry picking, when pulling from remote as well as when pushing.

### Git Hosting

I personally use [Atlassin Bitbucket](https://bitbucket.org/product/) as host, because they had free private repos before [GitHub](http://github.com), but either are okay. There's also [GitLab](http://gitlab.com), which lets you host on your own machine and a bunch of other systems. Most of what I write is applicable for all three, and you can choose whichever you like the most. GitHub has the best system to search for other peoples project by far, another reason why I prefer Bitbucket. The better search is why I recommend going with GitHub, if you're a proponent of open science, as mentioned earlier, it allows for other people to make corrections and even comment on your work.
