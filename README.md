# How to Host Your Resume on GitHub Pages

## Introduction
### Purpose
This tutorial shows you how to convert your Resume from a Word document to a [Markdown](https://www.markdownguide.org/) document using an editor like [Atom](https://atom.io/). Also, this tutorial shows how [Jekyll](https://jekyllrb.com/) is used to format your Markdown resume. Jekyll is a tool that transforms plain Markdown resumes into static websites. We are going to use Jekyll themes on GitHub to format the structure of your resume. Additionally, this tutorial shows how to host your Markdown-formatted resume on [GitHub](https://github.com/) Pages.

**What will you gain?** This tutorial will help transform and customize your resume to make it look more appealing. Also, it shows you how to host your customized resume online, so that it can be accessed by anyone at any time. Having your resume online potentially could be useful when you are talking to a prospective employer and you don't have your hard-copy resume to handout. You can share the link to allow the employer access to your resume any time.

### Audience
You don't need to have any prior knowledge of Jekyll, Markdown or [Atom](https://flight-manual.atom.io/getting-started/sections/installing-atom/) for this tutorial  
**Caution:** This tutorial assumes you have some knowledge of GitHub. For example, what it means to clone a repository, push to a repository and Pull down from a repository.

### Prerequisites
This tutorial also assumes that:
* You have a Resume in Word
* You have a [GitHub account](https://github.com/join?source=header-home)

## Instructions

### Format Resume in Markdown instruction
You are going to learn about 3 basic Markdown elements that can be the starting point to writing any resume in Markdown. There are many types of Markdown, but we are going to learn the GitHub Flavored Markdown (GFM). The GFM is the variation of Markdown that GitHub recognizes and the standard that all Markdown files hosted on GitHub has to follow to be rendered correctly.  
**Are you wondering why Markdown is useful if your resume already looks fine in MS Word?** Firstly, you have to ability to edit your Markdown files with any text editor. As opposed to using only MS Word. Also, it is easy to maintain version control with Markdown files compared to Ms word documents. So you can have multiple people collaborating in one document. To read on more benefits of Markdown go to [Hackernoon article on Say yes to Markdown, no to MS Word ](https://hackernoon.com/say-yes-to-markdown-no-to-ms-word-be4692e7a8cd) has a good article on that.
1. Open Markdown Editor  
    Atom is an editor that allows you to create Markdown files and preview how it is going to look like rendered. To create a Markdown file you need to save the file with extension .md or .markdown. Then to preview the file, select packages -> Markdown preview -> Toggle preview.
2. Paste in your resume content
3. Apply Markdown elements
The three basic Markdown elements that you can use to convert your Word document resume into Markdown are
#### 1. Headings
  > This can help you separate your resume into sections. There are 6 types of heading sizes in markdown.  
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
 In your resume, you might need a list to show the order an event happened. I am going to show you 2 types of list, unordered list, and ordered list
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

There are many other Markdown elements that could be useful. Check out [Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) for more Markdown elements.


### Host resume on GitHub Pages
GitHub Pages allow us to host our Markdown-formatted resume online. So, in this section, we are going to take your resume stored on your local computer, upload it to your GitHub account and preview your Markdown resume using your GitHub Pages URL.  

1. Click on the new repository button on GitHub  
  **RESULT:** A new page where you have to fill out the information about the repository
2. Name the repository username.github.io where username is your username on GitHub  
  **WARNING**: The username in the repository name has to be the same as your GitHub username for Github to host your resume

3. Select **Public** repository

4. Click on the create repository button

5. Clone the repository on your computer
   ~~~
   git clone https://github.com/username/username.github.io
   ~~~
     
   **RESULT:** username.github.io would be a directory on your computer
 
6. Navigate to username.github.io directory

7. Put your Markdown Resume in the directory

8. Rename your markdown resume to index.md  
  **WARNING:** If you do not rename your resume file to 'index', GitHub will not display your resume on GitHub Page. GitHub looks for an index.md file to host on GitHub Pages

9. Push changes to your master branch online repository  
    ~~~
    git add --all
    git commit -m "Initial commit"
    git push -u origin master
    ~~~  
      
    **WARNING:** The resume you want to be on your GitHub pages must be on the master branch

10. Navigate to the username.github.io repository on GitHub

11. In a browser navigate to https://username.github.io./

**RESULT:** Now when your goto https://username.github.io./ you should be able to see your Markdown-formatted resume online which can be accessed anywhere at any time. This is progress, but we have one more step to make your resume look more appealing.

### Apply Jekyll theme
Jekyll is a tool that transforms plain Markdown resumes into static websites. Jekyll would give us the ability to design our plain Markdown resume. We are going to be using the default Jekyll themes on GitHub to help with formatting. Applying a default theme would improve the way your hosted resume would look on Github Pages.

1. Navigate to the username.github.io repository on GitHub

2. Click settings

3. Scroll down to GitHub pages

4. Select the change theme button

5. Choose a theme    
**Result:** If you navigate to https://username.github.io./ this theme would be applied to your resume. Also, if you check your repository, it would contain a readme of the theme and `_Config.yml` file.

6. Update the `_Config.yml` add `title: My Resume` to the file  
**Result:** This would change the  title of your hosted resume to 'My Resume' 

You have now used a Jeykll theme to make your resume look more appealing.



### More Resource
* To understand what Markdown go to https://www.markdownguide.org/
* For how to install Atom go to https://flight-manual.atom.io/getting-started/sections/installing-atom/
* For the list of top 10 editors that are good for Markdown go to https://www.shopify.ca/partners/blog/10-of-the-best-markdown-editors
* For Markdown Cheatsheet go to https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet
* For more information on Jekyll go to https://jekyllrb.com/



### FAQ

1. When I create a heading does the space between the hashtag and my header need to be there?  
  > Yes, there has to be a space between the hashtag and your heading. This is mainly because Github need it to be formatted this way to render it properly

2. What is a YAML file?  
  > YAML which stands for YAML Ain't Markup Language and It allows you to provide powerful configuration settings. [Read More...](https://learn.getgrav.org/16/advanced/yaml)

3. Can I use other themes than the one GitHub provides?  
> Yes, you can either import an existing theme that someone else created or you can create your Jekyll theme to format your resume how you want it. On how to create a theme [Read More...](https://www.chrisanthropic.com/blog/2016/creating-gem-based-themes-for-jekyll/)

4. Can I host other things apart from a markdown file on GitHub?
> Yes, you can host more things apart from a Markdown file. You can host personal blogs, and othe websites with functionality


### Acknowledgment
 Manasseh Banda and Xiangwei(Max) Zhong
