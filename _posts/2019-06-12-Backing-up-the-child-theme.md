---
layout: post
title: "Backing up child theme"
date: 2019-06-12
---
1. Login using your credentials at [kmit.in/emagazine/wp-admin/](http://kmit.in/emagazine/wp-login.php?redirect_to=http%3A%2F%2Fkmit.in%2Femagazine%2Fwp-admin%2F&reauth=1)
2. Go to WP File Manager at bottom left corner
3. Browse into emagazine/wp-content/themes/
4. Press right click on baskerville-child, press download and save the .zip file
5. Fork the [baskerville-child-backup](https://github.com/kmitemagazine/baskerville-child-backup) onto your profile.
6. Clone your fork (For instance, I would enter git clone [https://github.com/iambrj/baskerville-child-backup](https://github.com/kmitemagazine/baskerville-child-backup))
7. Enter the baskerville-child directory and replace the .zip file present with the one downloaded in step 4
8. Make a new commit with mentioning month of backup (for instance I entered “June backup” for the latest commit)
9. Push changes onto github using `git push origin master` and open a pull request.

