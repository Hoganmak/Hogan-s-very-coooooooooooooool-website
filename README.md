## Setup

We don't want to keep your profile within `fullstack-challenges` because we want to version it with `git` as a separate project. So let's copy your profile as an independent folder and jump into it:

```bash
cd ~/code/challenges/04-Front-End/01-HTML-and-CSS/04-Responsive-profile
cp -r profile ~/code/profile
cd ~/code/profile
```

## Create the Github repo

Let's create our Github repository by [going here](https://github.com/). All you need to do is create a new repository with the plus button on the top right.

Set your repository to `Public` so everyone can see your work.

Now you can **init**(ialize) a git repository, commit your changes, and create the associated Github repo:

```bash
git init
git add .
git commit -m "my profile page"
git remote add origin git@github.com:<github_username>/<repository_name>.git  
git push -u origin master
```

`git remote add origin git@github.com:<github_username>/<repository_name>.git` will set where to add your code.

## Github Pages

[Github Pages](https://pages.github.com/) is a sub-service of Github that makes it easy to deploy any **static website** in 10 seconds. It is based on a "magic" branch, you define. When Github detects this branch, it puts your website online. Awesome right? Let's create this magic branch and push it. ✨🌿✨

First let's setup our Github pages:

1) Select `Settings` in your repository
2) Scroll all the way down to `GitHub Pages`
3) Select the `source` as `master branch` (the first option)
4) Done! ✨

Now you can build the URL `http://<user.github_nickname>.github.io/profile/` (this is the URL built automatically by Github) and have a look at your masterpiece online! Share the link on Slack with your buddies.

From now and until the end of the day, you can keep working in your `~/code/<user.github_nickname>/profile` directory AND on the `master` branch. This means any updates of your profile can be pushed on `http://<user.github_nickname>.github.io/profile/` through usual git commands:

```bash
git add .
git commit -m "make my profile prettier"
git push origin master
```
