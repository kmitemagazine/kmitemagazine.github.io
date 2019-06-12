---
layout: post
title: "Using Jekyll"
date: 2019-06-12 
---

  1. Fork the [kmitemagazine.github.io](https://github.com/kmitemagazine/kmitemagazine.github.io) repository onto your profile. For instance, I would fork it onto my profile, “iambrj”.
  2. Open up a terminal/command prompt, create a temporary directory (say temp) and cd into it.
  3. Enter `git clone <url to forked repo>`. For instance, I would enter 'git clone [https://github.com/iambrj/kmitemagazine.github.io](https://github.com/iambrj/kmitemagazine.github.io)'. You should now have a directory named ‘kmitemagazine.github.io’ inside the temp directory. If you do not, delete everything and start over again. Rename this directory to `_site`
  4. Once again, enter `git clone <url to forked repo>`. Now your temp directory should have two subdirectories, ‘kmitemagazine.github.io’ (which you just cloned) and ‘_site’ (which you cloned and renamed in step 3). 
  5. Change into ‘kmitemagazine.github.io’ subdirectory and enter `git checkout sources`. The terminal should say something along the lines

       * Switched to a new branch ‘sources’
       * Branch ‘sources’ set up to track remote branch ‘sources’ from ‘origin’
 
  6. Move the _site subdirectory into current directory using `mv ../_site ./`
  7. Add a new blog post. See this for help regarding writing a blog post. Please use markdown only.
  8. After writing a blog post, change to temp/kmitemagazine.github.io directory and enter `jekyll build`
  9. While in "temp/kmitemagazine.github.io" directory, add and commit new blog post to git using "git add _posts/YEAR-MONTH-DAY-title.markdown" and `git commit -m “add new blog post etc“`. Please use a more descriptive commit message.
  10. Now enter the _site directory, add and commit all changes using `git add *` and `git commit -m “added new blog post etc”`. Once again, use a descriptive commit message.
  11. Push your local changes onto your fork of the repository using `git push origin sources` (while in temp/kmitemagazine.github.io) and `git push origin master` (while in temp/kmitemagazine.github.io/_site)
  12. Go to your fork on github and press on “New pull request”. You’ll have to open two pull requests, first with both base and compare set to sources and second with both set to master. Sit back and wait for someone with write access to review and merge it.
  13. If you should get stuck at any point, before asking a question make sure you have followed all the instructions carefully. I suggest you delete whatever you have worked on and start over again before asking a question.

**Some links you may find useful**
  1. My [fork](https://github.com/iambrj/kmitemagazine.github.io) of the repo (step 3). You’ll have something similar if you do everything correctly
  2. My commits after updating [master](https://github.com/iambrj/kmitemagazine.github.io/commit/f44b3aa391ddea099bc1a3d809a94192c0ae5cbc) and [sources](https://github.com/iambrj/kmitemagazine.github.io/commit/17658ea971964341717de7a2e02db2a245ec5f8f) branches respectively (after steps 9, 10 & 11). Your diff files should look the same if you’ve followed the instructions correctly.
  3. Pull request [#13](https://github.com/kmitemagazine/kmitemagazine.github.io/pull/13) & [#14](https://github.com/kmitemagazine/kmitemagazine.github.io/pull/14) - I opened these to merge my master branch and sources branch respectively (step 12). If you have followed all the instructions, your pull requests should look like this.
  4. [Tutorial for writing Jekyll posts](https://jekyllrb.com/docs/posts/)
  5. [A useful cheatsheet for git](https://education.github.com/git-cheat-sheet-education.pdf)
