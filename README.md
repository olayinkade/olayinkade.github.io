# How to Host Your Formatted Resume on GitHub Pages


### Description
This tutorial shows how you to convert your Resume from a word document to a [Markdown](https://www.markdownguide.org/) document using an editor like Atom. Also, this tutorial shows how [Jekyll](https://jekyllrb.com/) is used to format your Markdown resume. Jekyll is a tool that transforms plain Markdown Resumes into static websites that can be access anywhere. We are going to us Jekyll themes on GitHub to format the structure of your resume content.  Additionally, this tutorial shows how to host formatted Resumes on [GitHub](https://github.com/) Pages.

### Benefit
**What will you gain?** This tutorial will help transform and customize your resume to make it look more appealing. Also, it shows you how to host your customized resume online, so that it can be accessed by anyone at anytime. Having your resume online potentially could be useful when you are talking to a prospective employer and you dont have your hard-copy resume to handout. You could share the link and to allow the employer access to your resume anytime

### Prerequisites
You dont need to have any prior knowledge of Jekyll, Markdown or Atom for this tutorial
Caution : This tutorial assumes you have some knowledge of GitHub. For example, what it means to Clone a Repository, push to a Repository and Pull down from a Repository.

This tutorial also assumes that:
* You have a Resume in word
* You have a [GitHub account](https://github.com/join?source=header-home.
### Atom
[Atom](https://flight-manual.atom.io/getting-started/sections/installing-atom/) is an editor that allows you to create Markdown files and preview how it is going to look like rendered. To create a markdown file you need to save the file with extension .md or .markdown. Then to preview the file, select packages -> Markdown preview -> Toggle preview.
### Markdown instruction

You are going to learn about 3 basic Markdown element that can be the start point to writing any resume in Markdown. The are many types of Markdown, but we are going to learn the GitHub Flavored Markdown (GFM). The GFM is the Markdown that GitHub recognizes and the standard that all Markdown file hosted on GitHub has to followed, so as to be rendered correctly
#### 1. Headings
  > This can help you separate the section you have in your Header. There are 6 types of heading sizes in markdown.
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
 In your resume you might need a list to should the other an event happened using a list. I am going to show you 2 types of list, Ordered list and unordered list
 1. Unordered List
`* Milk `
`* Eggs `
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
Result : A new page where you have to fill out the information about the Repository
2. Name the Repository username.github.io where username is your username on GitHub
 * Warning: The username in the Repository name has to be the same as your GitHub username for tutorial to work
3. Select **Public** Repository
4. Click on the create Repository button
 Result : You have created the Repository that you would host your Resume on
5. Clone the Repository
 ~~~
 git clone https://github.com/username/username.github.io
 ~~~
 Result : username.github.io would be a directory on computer
6. Navigate to username.github.io directory
7. Put markdown Resume in the directory
8. Rename Resume file to index
Warning: If you do not rename the resume to 'index' GitHub will not display your resume on GitHub page as it looks for a index.md file to host
9. Push changes to your master branch online Repository
~~~
git add --all
git commit -m "Initial commit"
git push -u origin master
~~~
Warning: The resume you want to be on your website must be on the master branch
10. Navigate to the username.github.io Repository on GitHub
11. Click settings
12. Scroll down to GitHub pages
13. Select a change Theme button
14. Choose a Theme
15. In a browser navigate to https://username.github.io./

### FAQ

1. When I want to create a heading does the space have to be there ?

2. can I  italicize  or bolden on a

3. What is a YAML file?

4. Why is there a YAML file in my Repository after I choose a theme?

5. Can I create my own theme using Jekyll

6. Can I host other things apart from a markdown file on GitHub?

7. Does my resume have to be a word document before I can convert it to Markdown?

8. After I change themes, I can see the new theme applied on my resume ?

### Acknowledgement
Christina Penner, and members of Group 10.
