# How to Host Your Formatted Resume on GitHub Pages


### Description
This tutorial shows you how to convert your Resume from a word document to a [Markdown](https://www.markdownguide.org/) document using an editor like [Atom](https://atom.io/). Also, this tutorial shows how [Jekyll](https://jekyllrb.com/) is used to format your Markdown resume. Jekyll is a tool that transforms plain Markdown Resumes into static websites that can be access anywhere. We are going to use Jekyll themes on GitHub to format the structure of your resume. Additionally, this tutorial shows how to host your formatted resume on [GitHub](https://github.com/) Pages.

### Benefit
**What will you gain?** This tutorial will help transform and customize your resume to make it look more appealing. Also, it shows you how to host your customized resume online, so that it can be accessed by anyone at anytime. Having your resume online potentially could be useful when you are talking to a prospective employer and you dont have your hard-copy resume to handout. You could share the link and to allow the employer access to your resume anytime.

### Prerequisites
You dont need to have any prior knowledge of Jekyll, Markdown or [Atom](https://flight-manual.atom.io/getting-started/sections/installing-atom/) for this tutorial  
**Caution** : This tutorial assumes you have some knowledge of GitHub. For example, what it means to clone a Repository, push to a Repository and Pull down from a Repository.

This tutorial also assumes that:
* You have a Resume in word
* You have a [GitHub account](https://github.com/join?source=header-home)

### Atom
Atom is an editor that allows you to create Markdown files and preview how it is going to look like rendered. To create a Markdown file you need to save the file with extension .md or .markdown. Then to preview the file, select packages -> Markdown preview -> Toggle preview.

### Markdown instruction
You are going to learn about 3 basic Markdown elements that can be the starting point to writing any resume in Markdown. There are many types of Markdown, but we are going to learn the GitHub Flavored Markdown (GFM). The GFM is the Markdown that GitHub recognizes and the standard that all Markdown file hosted on GitHub has to follow to be rendered correctly.  
  
#### 1. Headings
  > This can help you separate your resume into section. There are 6 types of heading sizes in markdown.  
  > &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1. `# Heading`
  > # &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Heading
  >&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;2. `## Heading`
  > ## &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Heading
  >&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;3. `### Heading`
  >### &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;  Heading
  >&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4. `#### Heading`
  >#### &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Heading
  >&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;5. `##### Heading`
  >##### &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Heading
  >&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;6. `###### Heading`
  >###### &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Heading

#### 2. _Italics_ and bold
  This can help emphasize and bring attention to different portions of your resume.
  1.  `_italics _` _italics_
  2.  `**BOLD**` **BOLD**

#### 3. Lists
 In your resume you might need a list to show the order an event happened. I am going to show you 2 types of list, unordered list and unordered list
 1. Unordered List      
  `* Milk`      
  `* Eggs`      
  `* Bread`    

    which renders in Markdown as

      * Milk
      * Eggs
      * Bread

 2. Ordered List  
  `1. Milk `  
  `2. Eggs `  
  `3. Bread`  

    which renders in Markdown as  
    
        1. Milk  
        2. Eggs  
        3. Bread  

There are many other Markdown element that could be useful. Check out [Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) for more Markdown element.


### Jekyll and GitHub instructions
1. Click on the New Repository button on GitHub  
  **RESULT** : A new page where you have to fill out the information about the Repository

2. Name the Repository username.github.io where username is your username on GitHub  
  **WARNING**: The username in the Repository name has to be the same as your GitHub username for Github to host your resume

3. Select **Public** Repository

4. Click on the create Repository button

5. Clone the Repository  
   ~~~
   git clone https://github.com/username/username.github.io
   ~~~
     
   **RESULT** : username.github.io would be a directory on computer
 
6. Navigate to username.github.io directory

7. Put your Markdown Resume in the directory

8. Rename your markdown resume to index.md  
  **WARNING**: If you do not rename your resume to 'index', GitHub will not display your resume on GitHub page. GitHub looks for a index.md file to host

9. Push changes to your master branch online Repository  
    ~~~
    git add --all
    git commit -m "Initial commit"
    git push -u origin master
    ~~~  
      
    **WARNING**: The resume you want to be on your GitHub pages must be on the master branch

10. Navigate to the username.github.io Repository on GitHub

11. Click settings

12. Scroll down to GitHub pages

13. Select the change Theme button

14. Choose a Theme

15. In a browser navigate to https://username.github.io./

Now you have your resume on GitHub pages and can view it anywhere at anytime.


### FAQ

1. When I want to create a heading does the space between the hashtag and my header need to be there?  
  > Yes, there has to be a space bettween the hashtag and your heading. This is mainly because Github need it to be formatted this way to render it properly

2. Can I  italicize  or bolden a heading?  
> You can italicize a heading, but you can bolden a heading. By default heading are already **bold**

3. What is a YAML file?  
  > YAML which stands for YAML Ain't Markup Language and It allows you to provide powerful configuration settings. [Read More...](https://learn.getgrav.org/16/advanced/yaml)

4. Can I Use other themes than the one GitHub provides?  
> Yes, you can either import an existing theme that someone else created or you can create your own Jekyll theme to format your resume how you want it. On how to create a theme [Read More ..](https://www.chrisanthropic.com/blog/2016/creating-gem-based-themes-for-jekyll/)

4. Can I host other things apart from a markdown file on GitHub?
> Yes, you can host more things apart from a Markdown file. You can host personal blogs, and websites with  functionality


### Acknowledgement
Christina Penner, and members of Group 10.
