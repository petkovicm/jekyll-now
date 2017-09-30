---
layout: post
title: How to fix No GitHub API Authentication error in Jekyll
---

Hi there. I recently switched jobs, so I was busy making a transition, and also got myself a new gear (MB Pro yummy). I was *Windows* user for about 15 years, and actually, remember running Aladin game from *MS-DOS* prompt window. Now, the time has come to step on the dark side and explore possibilities of a new environment for work and personal projects.

I started setting up *Jekyll* again (which is really easy when you are on Mac, so one point there). However, when I ran my local server I got an error in my terminal:
```
GitHub Metadata: No GitHub API authentication could be found. 
Some fields may be missing or have incorrect data.
```
<!--more-->

So, as I was googling the solution, I came to realize that this was more of a warning than an error. However, it bothered my OCD, and I started jumping back and forth to find a solution. I am actually writing this instruction for personal reference as well if I switch to another environment in the future or something like that. 

**Step 1:**

Create a personal access token for the command line. You can find instructions on GitHub [help page](https://help.github.com/articles/creating-a-personal-access-token-for-the-command-line/ "GitHub").

**Step 2:**

Open the bash_profile file. If you are on Mac OS, run the *terminal* and enter:
```
touch ~/.bash_profile; open ~/.bash_profile
```
It will open up the file with TextEdit. You can also use other editors:
```
nano ~/.bash_profile
mate ~/.bash_profile
vim ~/.bash_profile
```
**Step 3:**

Now, inside the ```bash_profile``` define new environment variable with variable name ```JEKYLL_GITHUB_TOKEN``` and GitHub access token as variable value (you generated it in Step 1). You can do this by addiing the following line :

```
export JEKYLL_GITHUB_TOKEN ='your_token_here'
```

**Step 4:**

Reload the terminal, and to make sure you did everything right, enter this into your command line:
````
echo $JEKYLL_GITHUB_TOKEN
````
You should be getting back token you generated in Step 1.

Now, when you run:
````
bundle exec jekyll serve
````
you shouldn't be getting any errors.




