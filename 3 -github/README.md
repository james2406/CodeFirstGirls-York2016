# Intro to Github

### Example 1

1. Let’s say you're working with another person on a project
2. Together you both have to create a powerpoint presentation for a semminar
3. Before you part ways, you'll create a structure for presentation
4. You work on this, Your partner will work on that...
5. ... Now, you meet again and you've chosen different colour schemes, used different fonts and styles to eachother

What if there were a way to automate the merging of your material, where you could choose what to keep and what not to keep?

### Example 2

1. Another scenario could be you working on your CV
2. Over the years, you would have made an array of edits to your CV
3. You'd have to save all the different versions across files

What if you could see exactly what changes you’ve made and where over time?

## Lesson One - version control

Version control, is the key to collaborative software development. You can work in teams on the same project, easily manage conflicts in code on the same files, work on different versions all at the same time and then decide what you want to keep and what you want to bin at the end

This is why we need version control:

* Backup and Restore - Files are saved as they are edited, and you can jump to any moment in time

* Synchronization - Lets people share files and stay up-to-date with the latest version

* Short-term undo - If you're changing a file and messed something up, throw away your changes and go back to the “last known good” version in the database

* Long-term undo - If you've made a big error, you can go back to a change a year ago

* Track Changes - As files are updated, you can leave messages explaining why the change happened. Making it easy to see how a file is evolving over time, and why

* Track Ownership - A VCS tags every change with the name of the person who made it. Helpful for giving credit / blaming

* Sandboxing - You can make temporary changes in an isolated area, to test code before commiting your changes

* Branching and merging - You can branch a copy of your code into a separate area and modify it in isolation. Later, you can merge your work back into the common area

Main elements of version control:

* Repositories - A repositories is (generaly) a single project. They can contain folders and files, including images / anything your project needs. They should include a README and a license

* Branches - Branching is the way to work on different parts of a repository at one time. When you create a repository, by default it has one branch called master

* Commits - On GitHub, saved changes are called commits, a bunch of them together read like the history of your project. Each commit has an associated commit message, which is a description explaining why a particular change was made

* Issues - An Issue is a note on a repository about something that needs attention (it could be a bug, a feature request, a question...)

* Pull Requests - When you make a pull request, you’re proposing your changes and requesting that someone pull in your contribution (aka merge them into their branch)

## Task One - using Git

You're planning a party, and want to create a shopping list containing simple text files on your computer. You don’t want to lose them incase your laptop breaks/gets lost. It would be great to see the complete history of the changes to the files over time. And you also want to allow other people to see/edit the shopping list

1. Create the shopping list folder on your computer (party-shopping-list)
2. Add the text files to the folder (drinks.txt and food.txt)
3. Commit the changes to github, attaching a comment
4. Push the repository created up to github

You want to add your friend to make changes to your repository

1. Right click the repository
2. Click ‘View on Github’
3. Clicks on ‘settings’ > ‘collaborators’ > add your partner as a collaborator

Then your friend can access this repository by

1. Opening the github app
2. Clicking the ‘+’ icon in the top left, then ‘clone’, to clone it to a folder on their computer
3. View the history of the repository
5. Update the editting some of the files
6. Commit and push to github

Now you can click sync to recieve the changes. However, what happens if you make a change at the same time

1. Both make a change to the same file at the same time
2. Commit and push, one after the other
3. Open the files in a text editor (e.g. Sublime)
3. Choose the correct lines to keep

## Lesson Two - putting your site online

We’re going to use [GitHub Pages](https://pages.github.com/) to host our site - it will provide the server where the files for our site is stored

## Lesson Three - the command line

Text
