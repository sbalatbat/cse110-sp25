# Lab Week 1 - VSCode, Markdown, and Git Part 1

For your first lab assignment, you will be creating a GitHub User Page about yourself for your GitHub account. The purpose is to give an introduction of who you are as a programmer, who you are as a person, and any other interesting things you'd like to share with the kind of person who might be taking a look at your profile (think potential employers, open source devs, generally just the kinds of people who would be looking at the source code for a project you made).

## Part 1. Installing Visual Studio Code and Extensions
We'll be supporting VSCode as the main IDE for this class. One of the strengths of VSCode is the ecosystem of extensions that helps increase your efficiency as a developer and allows you to customize the experience of your IDE.

1. Download and install VSCode here: https://code.visualstudio.com/download
2, Install VSCode extensions ([instructions here](https://code.visualstudio.com/docs/editor/extension-gallery)). Here are a few suggestions that may be useful for this course:
- [Draw.io](https://marketplace.visualstudio.com/items?itemName=hediet.vscode-drawio)
- [LiveShare](https://marketplace.visualstudio.com/items?itemName=MS-vsliveshare.vsliveshare)
- [Markdown All In One](https://marketplace.visualstudio.com/items?itemName=yzhang.markdown-all-in-one)
- [CodeStream](https://marketplace.visualstudio.com/items?itemName=CodeStream.codestream)

Also feel free to explore and install any other extension that suits your needs and optimize your experience!

## Part 2. (Re)Familiarizing Ourselves with Git
Throughout the project, you will use git to access and modify your repository on GitHub. To ensure everyone has a working knowledge of git, you will use it to modify your repository using both the command prompt and the VS Code source control UI. Install Git on your system [here](https://git-scm.com/downloads) if you do not have it already. 

First, create the GitHub repository for your GitHub Pages project. Make sure the repository is public and includes a "README.md" file.

### Command Line
For the following steps, perform each step using the command line unless otherwise stated. If anyone is fuzzy on git commands and their uses, [this is a great resource](http://guides.beanstalkapp.com/version-control/common-git-commands.html) describing common commands.

1. **clone** the repository onto your local machine using the command line. For an explanation of how to do this, see [GitHub's documentation](https://docs.github.com/en/free-pro-team@latest/github/creating-cloning-and-archiving-repositories/cloning-a-repository#cloning-an-empty-repository).
2. **cd** into the repo folder and create a new git **branch** called "add-read-me" (can be done either locally or through GitHub) and **checkout** that branch into your local repository.
3. Add the text "`<Your name>`'s User Page" to the "README.md" file (e.g. "Powell's User Page"). This can be done using a separate text editor.
4. **add** the new file to git.
5. **commit** the files with the commit message "Update readme file".
6. **push** the commit to the remote branch. (You may need to use the **set-upstream** flag if you created the branch locally).

Take a screenshot of **ALL** the git commands (from steps 1, 2, 4, 5, and 6) being performed as a deliverable.

### VSCode UI
Secondly, we will go through a similar process in VS Code, as you may find it easier to use its built-in version control UI. For an overview of how to use VS Code version control, consult the [documentation](https://code.visualstudio.com/docs/editor/versioncontrol#_git-support).

Open the repository in VS Code, create a new branch and switch to it. In the README file, add a line about your favorite programming language.

In the newly created branch, create a file titled **PRIVATE.txt**. In this file, place your name and PID. Once this is done, create a **.gitignore** file in the root of your repository and add the path to this PRIVATE.txt file (just the name of the file if PRIVATE.txt is in the root). The idea is that you want to include any files you want git to ignore in the .gitignore file (files such as node_modules, .DS_Store, etc...). Read more about .gitignore [here](https://git-scm.com/docs/gitignore).

Under the `Source Control` tab, stage the changes and add an appropriate commit message.

****Before committing** and pushing the change, take a screenshot of the staged commit, commit message, and current branch as a deliverable.

These are the details which your screenshot should include. Please submit a **single image** with all these details.

![Example commit staged details](./img/commit-example.png)

![Example commit branch detail](./img/branch-detail.png)

 

## Part 3. Using Markdown
Markdown is a commonly used markup language for formatting plain text. You can learn more about its uses and syntax [here](https://www.markdownguide.org/getting-started/). 

Create a new file called **index.md** in whatever branch you like. This is where you'll create your User Page, which should include content that introduces who you are as a programmer and as a person. Your User Page must be made with Markdown. For this assignment, your page must include the following:
- Pictures
- All the core Markdown constructs in [GitHub Flavored Markdown](https://docs.github.com/en/free-pro-team@latest/github/writing-on-github/basic-writing-and-formatting-syntax)
  - Headings
  - Styling text
  - Quoting text
  - Quoting code
  - External Links (Link to another webpage)
  - Section links (Link to a header in the same .md file)
  - Relative links (Link to another .md file or an image in your repo. If linking to an image, encode it as a regular link rather than an image.)
  - Ordered and Unordered Lists
  - Task lists

Once you are finished, **publish your web page** through Github Pages - instructions [here](https://docs.github.com/en/github/working-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site). Include the URL to the published site in your README.md file.

 

OPTIONAL:

If you find yourself wanting to go above and beyond, here are some things you can add:

- A GitHub Pages theme
- Custom domain name for this page 

You can read about setting up a theme [here](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/adding-a-theme-to-your-github-pages-site-using-jekyll) and creating a custom domain [here](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site). 

Submit to Gradescope:
- **Link to your GitHub Repository.** Inside your repo, make sure you have:
  - A folder called **screenshots** in your root directory with
    - Screenshot of command line git transactions
    - Screenshot of staged commit in VS Code
  - **.gitignore**
  - A **README** file with the **URL of your published GitHub pages** site
  - Any other files you created for this assignment (Except **PRIVATE.txt**)