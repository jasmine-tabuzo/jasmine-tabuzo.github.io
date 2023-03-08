# Title: How to Host a Resume on Github Pages using VSCode and Jekyll

## Purpose
This guide will teach you how to host a resume on GitHub Pages using Visual Studio Code and Jekyll. 

Additionally, this guide will teach you some of Etter's key principals in technical communication, namely:      

1. Use a lightweight markup language
2. Format a document with a static site generator
3. Share/host documents on a distributed version control system.

## Prerequisites
- A GitHub account 
- A resume in markdown 
    - You can find a Markdown tutorial in the [More Resources](https://jasmine-tabuzo.github.io/README.html#more-resources) section of this guide.
- Visual Studio Code
- Windows OS

## Instructions

> Throughout this section, I will refer to Andrew Etter's book, *Modern Technical Writing: An Introduction to Software Documentation* to describe some key principals in technical communication. 
> 
> To find Etter's book, see the [More Resources](https://jasmine-tabuzo.github.io/README.html#more-resources) sub-section.

### 1. Create your GitHub Page

> Etter's Key Principal: Share/host documents on a distributed version control system.   
> 
> GitHub is a type of distributed version control system. Etter states that "DVCS have better performance, allow for offline work, and are superior for concurrent work on the same file." 

1. Login to GitHub 
2. Create a new repository 
3. Set the repository name to `[your GitHub username].github.io`
    - For example, my username is `jasmine-tabuzo`, so my repository name would be `jasmine-tabuzo.github.io`.

### 2. Create a Jekyll site

> Etter's Key Principle: Format a document with a static site generator    
> 
>  As Etter describes, static sites have "speed, simplicity, portability, and security."  

1. Install Ruby by following steps 1 & 2 of these [instructions](https://jekyllrb.com/docs/installation/windows/)
2. Install Jekyll by following steps 3 & 4 of these [instructions](https://jekyllrb.com/docs/installation/windows/)
3. Create a new Jekyll site by following [steps 2-6](https://jekyllrb.com/docs/) 

### 3. Add your Resume to the site

> Etter's Key Principle: Use a lightweight markup language
>
> As the prerequisites have stated, your resume must be in markdown format. According to Etter, Markdown is the most widely used lightweight markup language in the world. Lightweight markup makes it easier to build websites using human-readable content. Additionally, Etter mentions the separation between content and style. By using markdown, you can easily apply various themes and styles to your content!

1. Open the folder of your project 
2. Add your resume markdown file to the folder 
3. Open the folder in Visual Studio Code
4.  Open your resume file
5.  Add the following lines of code to the top of your resume file, including the dashed lines:    
```
---    
layout: page    
title: Resume    
permalink: resume.html    
---
```
1.  **Save** the file

### 4. Add the Jekyll theme

> Etter's Key Principle: Format a document with a static site generator    
> 
>  In addition to using a static site generator, Etter recommends to take some time to customize the theme. Etter states to "focus on navigation and approachability." This is your chance to differentiate your resume from other ones out there!  

1. Open the `_config.yml` file
2. Add this line to the end of the file `remote_theme: pmarsceill/just-the-docs` 
3. Save the `_config.yml` file
4. Open the `Gemfile` file
5. Change `gem "minima"` to `gem "just-the-docs"`
6. Save the `Gemfile` file

### 5. Upload your Jekyll site to GitHub

1.  Go to your repository on GitHub
2.  Select **Add file** 
3.  Select **Upload files**
4.  Drag your Jekyll site folder to your repository 
5.  Commit the changes 
6.  Wait 10 minutes for the page to build. 
7.  Navigate to `[your GitHub username].github.io` in your browser. 

Congratulations! You have successfully hosted your resume on GitHub Pages using Jekyll and Visual Studio Code. 

You should now have a hosted resume that looks like the one shown below: 
![resume](images/resume.gif)

### More Resources

- Andrew Etter's [Modern Technical Writing: An Introduction to Software Documentation](https://www.amazon.ca/Modern-Technical-Writing-Introduction-Documentation-ebook/dp/B01A2QL9SS)
- [Markdown Tutorial](https://www.markdowntutorial.com/)
- 

## Authors and Acknowledgements

- Template: [Just the Docs](https://github.com/just-the-docs/just-the-docs)
- Group 16: 
    - Sahilpreet Sidhu 
    - Eric Shu 
    - Kha Pham 


## FAQs

- Where can I find more Jekyll themes? 
    - You can find more Jekyll themes [here](https://jekyllrb.com/docs/themes/)

- Can I add pictures to my site?
    - Yes, you can add pictures to your site. To learn how to add pictures using markdown, follow this [lesson](https://www.markdowntutorial.com/lesson/4/)
