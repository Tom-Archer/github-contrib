# So you've found a bug and want to do something about it?

All the libraries for Pimoroni products are available online and can be modified by anyone, so let's go!

First things first, head over to the [Pimoroni GitHub page](https://github.com/pimoroni). On this page you'll find a listing of all the wonderful repositories maintained by the folks at Pimoroni. Generally there's one for each product/board that they produce, so go ahead and select the relevant repository. The examples on this page refer to the [Mote repository](https://github.com/pimoroni/Mote) which is pinned to the Pimoroni landing page.

![Pimoroni Home Page](/images/2-Pimoroni-Github.png)

## Repository Homepage
The repository homepage shows an overview of what's going on with the repository. For now we're interested in the issues list, so click "Issues" at the top of the page.

![Mote Repository Home Page](/images/3-Pimoroni-Github-Mote.png)

## The Issues List
The issues page shows a list of the 'active' issues that have been raised against the repository. These may be bugs, suggestions or new functionality. First check that the issue you've found isn't already present in this list.

![Mote Issues List](/images/4-Pimoroni-Github-Mote-Issues.png)

## Raising an Issue
If the issue you've found is new, click "New issue" - at this point go ahead and create a GitHub account if you haven't already. Fill in as much information as you can about the issue. For example you might include the steps required to reproduce it. 

![Raise an Issue](/images/5-Pimoroni-Github-Mote-Issues-Raise.png)

Once you've submitted the issue anyone is free to attempt to fix it, that could be the people of at Pimoroni, another GitHub user or yourself! If you know how to fix the issue, continue reading...

## Forking the Repository

In order to make changes to the code, we first need to fork the repository. On the repository home page, click the 'Fork' button in the upper right. This creates a copy of the repository under your user account. 

## Fixing the Code (Raspberry Pi)

![Clone Repository](/images/6-Personal-Github-Mote.png)

First we need to download the code to our Raspberry Pi, so create a folder and navigate to it using the terminal. (I normally use the 'Python' folder for this.) Then enter the following, replacing the URL with the appropriate repository location from your GitHub account: 

```bash
git clone https://github.com/Tom-Archer/mote.git
```

After a short moment the code should finish downloading. Now you can modify the code without affecting the original repository. Next we're going to create a branch to contain all the changes related to this issue. This isn't strictly necessary but it's good practice to segregate changes if you're working on multiple issues.

```bash
git branch issue-description
```

Finally we're going to tell Git that we want to work on the new branch:

```bash
git checkout issue-description
```

Now we can make the changes! Once you've done and the changes have been tested, it's time to submit them.

## Submitting the Changes

```bash
git status
```

```bash
git add filename.py
```

```bash
git commit -m 'Helpful message describing the change.'
```

```bash
git push origin issue-description
```

## Creating a Pull Request





# Glossary
## What is GitHub?
GitHub is one of the most widely-used websites for storing and maintaining code. 

## What is a repository?
A GitHub page will generally contain a number of repositories, you can think of these as project folders. 
