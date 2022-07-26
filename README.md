# C-MOOR Website Template

This is a template for C-MOOR students to use to create their own portfolio websites.  It enables students to create a professional website which they can manage through the GitHub GUI (no need to install or render anything locally).

- Uses the [Hugo setup](https://github.com/marketplace/actions/hugo-setup) and [GitHub Pages](https://github.com/marketplace/actions/github-pages-action) actions to render a Hugo static site hosted with GitHub pages.
- Theme was forked from [lxndrblz/anatole](https://github.com/lxndrblz/anatole/) and modified by Katherine Cox for use by C-MOOR learners.

This template uses the Hugo static site generator, so students interested in further customization can consult the [Hugo documentation](https://gohugo.io/) and dive as deep as they like into web development :)

## Create GitHub Account

To use this template, you must have a GitHub account.  If you do not yet have an account, this video ([video](https://link.c-moor.org/video-join-github))([slides](
https://docs.google.com/presentation/d/1c4sb5CLpvKjgnTVIuNGYTSr8WWNgeSfC8TUGrxktu64/)) shows you how to create an account.  You can follow along with the video, or follow the steps below.

1. Open [github.com](https://github.com/) in a web browser and click “Sign up”.
1. Choose a username and password.  It is a good idea to choose a username that you would not mind sharing with future employers, as they may view your GitHub profile.  Some good options include your name, or some variation of it, or something to do with the type of projects you’re working on.
1. GitHub will ask you a few questions and then ask you to choose a plan.  Unless you’re sure you need something from the paid plans, select the free plan.  You can always upgrade later.
1. Check your email and click on the verification link.
1. Update your GitHub profile.
    - You can access your GitHub profile from the dropdown menu on the right side of the screen, by clicking on your user icon.
    - It’s generally a good idea to add a little bit of information about yourself, so people can see who you are and verify they’re connecting with the right person.  From your profile page, you can upload a picture and enter some basic information about yourself.  This information will be public, so enter whatever information you’d like others to be able to see.

## Setup Website

The first steps in creating your website are to:

1. Create your own copy of this template,
1. Configure the settings so it runs in your GitHub repository
1. Confirm that when you make edits to the content, your website updates to reflect those changes

This video ([video](https://link.c-moor.org/video-student-website-setup))([slides](
https://docs.google.com/presentation/d/13chl2zYU1NbWCZmD_daqiKcLoJZAtILMqjXgew3TR6c/)) shows you how to set up your own copy of the website with some example content.  You can follow along with the video, or follow the steps below.

### Copy Template

First, you need to create your own copy of the website template.

1. Find the [C-MOOR website template](https://github.com/C-MOOR/cmoor_website_template/) on GitHub.  Click the green “**Use this template**” button  to make your own copy.
    - This will open up a page for setting up your new project.  On GitHub, projects are called “repositories”.
1. Choose a name for your new repository.  This name will be part of the URL for your website, so it’s a good idea to make it short and descriptive.
    - You can change it later, but it’s a bit of a pain, so try to pick something that you will stick with.  You can also add a short description if you would like.
1. If you are using the free GitHub plan, you must set the repository as **Public** for your website to work.
1. Click the “**Create repository from template**” button.

You should now have your own copy of the website repository (source code) that you can edit as you please, though it won't yet look like a website.  

### Configure Settings

The next step is to set things up so that this collection of files gets turned turn into a proper website.

There are two important settings you need to set up to get your website working:

1. Set up GitHub pages, which will tell GitHub to treat your repository as a website (so it will display properly)
1. Update the URL so it points to your copy of the site, rather than the C-MOOR template

#### Setup GitHub pages

1. In your repository, click on the “**Settings**” tab in the upper right.
1. Within the “Settings” tab, select “**Pages**” from the left menu.  You may have to scroll down to find it.
1. Check the “**Source**” for your site.  The branch should be `gh-pages` and the folder should be `root`.
1. Click "**Save**".

While you’re here, copy the URL for your site (shown in the blue box).  You’ll need it for the next step.

#### Update URL

1. From the main page of your repository, click on the folder named `config/_default`.
1. Click on the file named `config.toml`
1. Click on the pencil icon in the upper right to edit this file
1. Update the `baseURL` (first line of this file)
    - Right now, this has the URL for the C-MOOR template website.  Replace the URL with the address of your website (the address you copied from the GitHub Pages Settings).  This should have your GitHub username followed by the name of your repository.
    - Make sure to keep the quotation marks around the new URL.
1. Save your changes by scrolling down to the “**Commit changes**” box.  Enter a brief description of the change, then click “Commit changes”.

It will take little while for your website to update, but shouldn’t take more than a minute or so.  From the main page of your repository, you can see an orange dot indicating that GitHub is working.  You can click on this dot to see more information.  When GitHub is done, the orange dot will change to a green checkmark.  If it’s been more than a minute and it hasn’t changed, try refreshing the page.  Sometimes the status indicator doesn’t update right away.

#### View Site

To view your website, you can either enter your website’s URL directly in your browser, or, from the main page of your repository, you can click on the `github-pages` Environment (bottom right).

- If you clicked on `github-pages`, you will end up on the Deployments page.  This has information about every time your website gets updated.  There should be a recent new deployment.  Click “**View deployment**” to see your website.

If you don’t see a website or the website looks weird, the first thing you should do is to try [clearing your browser cache](https://github.com/C-MOOR/cmoor_website_template/blob/main/README.md#clear-browser-cache).  Your browser may have stored an old version of the website instead of getting the latest version.

### Confirm You Can Edit

Finally, try making a small change to the website content, and make sure that your website updates correctly to reflect that change.

1. From the main page of your repository, click on the folder named `config/_default`.
1. Click on the file named `params.toml`
1. Click on the pencil icon in the upper right to edit this file
1. Change the title and/or description to say something about yourself.
    + ![](https://docs.google.com/presentation/d/13chl2zYU1NbWCZmD_daqiKcLoJZAtILMqjXgew3TR6c/export/png?id=13chl2zYU1NbWCZmD_daqiKcLoJZAtILMqjXgew3TR6c&pageid=gd7ff47b35c_0_236)
1. Save your changes by scrolling down to the “**Commit changes**” box.  Enter a brief description of the change, then click “Commit changes”.
1. View your website.  Remember that it may take a minute to update.  If you don’t see any changes, try [clearing your browser cache](https://github.com/C-MOOR/cmoor_website_template/blob/main/README.md#clear-browser-cache) and then refreshing the page.


## Personalize Website

Once you have a functioning website, you will want to replace the example content with information about you.  You will also want to customize some settings.  Here we provide instructions on how to 

- Update the profile information
- Update the About page
- Update language options
- Update site preview

Note that there are several other settings you can change, including things like

- Display of dates and math
- Comments and a contact form
- Site Analytics
- Multilingual content

If you would like to learn more about other ways you can configure your website, visit the [GitHub repository](https://github.com/lxndrblz/anatole) for the website theme and look through the README file.

### Update Profile

This video ([video](https://link.c-moor.org/video-student-website-personalize-profile))([slides](
https://docs.google.com/presentation/d/1Fvf-pp35kzthJawqHwNVg8fTA5YDOWSOD88hVBFs840/)) shows you how to update the profile information displayed on the left side of the website, including the text, image, and social media links.  You can follow along with the video, or follow the steps below.

#### Update Title and Description

1. From the main page of your repository, click on the folder named `config/_default`.
1. Click on the file named `params.toml`.
1. Click on the pencil icon in the upper right to edit this file.
1. Update the `title` and `description` to say something about yourself.
1. Save your changes by scrolling down to the "**Commit changes**" box.  Enter a brief description of the change, then click "Commit changes".
1. View your website. Remember that it may take a minute to update.  If you don’t see any changes, try [clearing your browser cache](https://github.com/C-MOOR/cmoor_website_template/blob/main/README.md#clear-browser-cache) and then refreshing the page.

#### Update Profile Image

1. Upload a new image
    1. From the main page of your repository, click on the folder named `static/images`.
    1. Click the "**Add file**" button and choose "**Upload files**".
    1. Upload an image file, then scroll down and commit your changes to save them.
1. Set the profile image
    1. From the main page of your repository, click on the folder named `config/_default`.
    1. Click on the file named `params.toml`.
    1. Click the pencil icon in the upper right to edit this file.
    1. Change the file name of the `profilePicture` to match the the image file you want to use.
        + Make sure they match exactly, including the extension, or your website won’t be able to find the image.
        + Make sure to keep the quotation marks around the new file name.
    1. Save your changes by scrolling down to the "**Commit changes**" box.  Enter a brief description of the change, then click "Commit changes".
    1. View your website. Remember that it may take a minute to update.  If you don’t see any changes, try [clearing your browser cache](https://github.com/C-MOOR/cmoor_website_template/blob/main/README.md#clear-browser-cache) and then refreshing the page.

#### Update Social Media Links

1. From the main page of your repository, click on the folder named `config/_default`.
1. Click on the file named `params.toml`.
1. Click on the pencil icon in the upper right to edit this file.
1. For each social media account that you would like to add, enter the `url` of your profile.  Don’t change the `icon` or `title`.
    + If you do not have an account or don’t want to link your account, you can remove the icon by inserting a hash symbol (`#`) before each line for that platform.  Make sure you do this for all four lines.  The hash tells your website to ignore these lines.  They should turn grey when you add the hashes in front of them.
1. Save your changes by scrolling down to the "**Commit changes**" box.  Enter a brief description of the change, then click "Commit changes".
1. View your website and click on the social media icons to confirm they link to your accounts. Remember that it may take a minute to update.  If the links haven’t changed, try [clearing your browser cache](https://github.com/C-MOOR/cmoor_website_template/blob/main/README.md#clear-browser-cache) and then refreshing the page.

### Update About Page

The About page gives you a chance to tell people a little bit about yourself.  A couple of paragraphs is generally appropriate.  You might describe how and where you’ve been studying or working, or what kinds of projects you find exciting and why.

This video ([video](https://link.c-moor.org/video-student-website-personalize-about))([slides](
https://docs.google.com/presentation/d/1qg3i5WhpqiPrLPdLdJoiVaCmZALNpPrlbHwBigbtfYo/)) shows you how to update the About page of your website.  You can follow along with the video, or follow the steps below.

1. From the main page of your repository, click on the folder named `content`.
1. Click on the folder named `english`.
1. Click on the file named `about.md`.
1. Click on the pencil icon in the upper right to edit this file.
1. Change the `description`.  "About *Your Name*" is a good choice.  You can also update the date, though this is not important.
1. Replace the content of the page (below the row of plus signs) with some information about yourself.  You can use markdown to add formatting, such as bold or italic text, links, and lists.  This [commonmark tutorial](https://commonmark.org/help/tutorial/) provides a walkthrough of how to use markdown if you need it.
1. Save your changes by scrolling down to the "**Commit changes**" box.  Enter a brief description of the change, then click "Commit changes".
1. View your website and look at the About page to see if it looks the way you want. Remember that it may take a minute to update.  If it hasn't changed, try [clearing your browser cache](https://github.com/C-MOOR/cmoor_website_template/blob/main/README.md#clear-browser-cache) and then refreshing the page.

### Update Language Options

This website template is able to support multilingual content, but setting it up is a bit complicated. The instructions below show you how to disable the Arabic language option, leaving only the English option.  If you're interested in setting up multilingual content, you can find out more in the README of the [GitHub repository](https://github.com/lxndrblz/anatole) for the website theme (scroll down to find the section on multilingual content).

This video ([video](https://link.c-moor.org/video-student-website-personalize-languages))([slides](
https://docs.google.com/presentation/d/1jLbdARLPvVnEl0HA18Jli0qQ90Bg9JFbenRqLBSeovk/)) shows you how to remove the Arabic language option, leaving on the the English option.  You can follow along with the video, or follow the steps below.

1. From the main page of your repository, click on the folder named `config/_default`.
1. Click on the file named `languages.toml`.
1. Click on the pencil icon in the upper right to edit the file.
1. Remove the Arabic option by inserting a hash symbol before each line.
    + Make sure you do this for all seven lines.  The hash tells your website to ignore these lines.  They should turn grey when you add the hashes in front of them.
1. Save your changes by scrolling down to the "**Commit changes**" box.  Enter a brief description of the change, then click "Commit changes".
1. View your website and look at the top navigation bar to see if the Arabic option has been removed. Remember that it may take a minute to update.  If it hasn't been removed, try [clearing your browser cache](https://github.com/C-MOOR/cmoor_website_template/blob/main/README.md#clear-browser-cache) and then refreshing the page.

### Update Site Preview

This video ([video](https://link.c-moor.org/video-student-website-personalize-preview))([slides](
https://docs.google.com/presentation/d/1r3PPXaHUnZfzeKe4hZisaVM7Edz5VLw6hnKHzvifoWE/)) shows you how to update the preview of your site that is displayed when you post the link somewhere, such as a messaging app or forum.  You can follow along with the video, or follow the steps below.

#### Update Title

1. From the main page of your repository, click on the folder named `config/_default`.
1. Click on the file named `config.toml`.
1. Click on the pencil icon in the upper right to edit this file.
1. Change the `title` to your name
1. Save your changes by scrolling down to the "**Commit changes**" box.  Enter a brief description of the change, then click "Commit changes".
1. View your site preview by posting the link to your site in a messaging app or forum.

#### Update Description

Note that the description displayed in the site preview is the same as the description displayed in the profile section of your website.  Choose a description that works for both places.

1. From the main page of your repository, click on the folder named `config/_default`.
1. Click on the file named `params.toml`
1. Click the pencil icon in the upper right to edit this file.
1. Edit the description as you like.
1. Save your changes by scrolling down to the "**Commit changes**" box.  Enter a brief description of the change, then click "Commit changes".
1. View your site preview by posting the link to your site in a messaging app or forum.

#### Update Preview Image

Although the default image displayed in the site preview looks like a screenshot of the website, it does not automatically update to match changes you make to your website.  You get to choose what image is used as a preview for your website.  A screenshot of the whole website is usually a good option, but you could also zoom in on a particular section if you’d like.

1. Take a screenshot of the part of your website you’d like to use for the preview.
1. Upload the new image.
    1. From the main page of your repository, click on the folder named `static/images`.
    1. Click the "**Add file**" button and choose "**Upload files**".
    1. Upload the image file, then scroll down and commit your changes to save them.
1. Set the site preview image.
    1. From the main page of your repository, click on the folder named `config/_default`.
    1. Click on the file named `params.toml`.
    1. Click the pencil icon in the upper right to edit this file.
    1. Change the file name of `images` to match the the image file you want to use.
        + Make sure they match exactly, including the extension, or your website won’t be able to find the image.
        + Make sure to keep the quotation marks around the new file name.
    1. Save your changes by scrolling down to the "**Commit changes**" box.  Enter a brief description of the change, then click "Commit changes".
    1. View your site preview by posting the link to your site in a messaging app or forum.

## Add Posts

The following instructions show you how to add a post to your website, and how to add and link to additional media in your posts.

### Structure of a post

+ Posts live in the `content/english/post` folder of your repository.
    + This folder contains all the posts that will show up on your website.  To start with, it’s been filled with some example posts.  Each folder listed here is a different post.
    + If you click on one of these folders you can see what makes up a post.
+ All posts will have an index.md file which contains the main content of the post.
    + The `index.md` file for each post begins with a header section surrounded by rows of 3 plus signs.
        + This header section contains information that helps your website display the post correctly.
        + The `title` is what your post will be named on your home page
        + Posts are sorted by `date`, so if you want a particular post to show up at the top, make sure to give it the latest date.
        + You can also add tags to help organize your posts.
    + Below the header is the main text of the post.
	    + You can write anything you like here, and can format it using markdown.
+ Some posts may also include additional files such as images you want to include or files you want to link to.

### Add Basic Post

This video ([video](https://link.c-moor.org/video-student-website-post-basic))([slides](
https://docs.google.com/presentation/d/1mLi7a-tZQLWp9RoOLhz90c_SDX2loBuXnwI7LfNJtcQ/)) shows you how to add a post to your website.  You can follow along with the video, or follow the steps below.

1. From the main page of your repository, click on the folder named `content`.
1. Click on the folder named `english`.
1. Click on the folder named `post`.
1. Click the "**Add file**" button, and choose "**Create new file**".
1. Enter the name for your post, followed by a forward slash (`/`), then `index.md`.
    + This will create a new folder and put a file named `index.md` inside.
    + This file must be named `index.md` or your post will not show up correctly.
    + The name of the folder will be used for the URL of the post, so it can’t have spaces.  Instead of spaces use hyphens or underscores.
1. Add a header to your post.  This should start and end with 3 plus signs.
	+ Make sure to include at least a `title` and `date`.
1. Add the content of your post.
    + You can add styling, such as bold, italics, or bullet points to your post using markdown.  If you’re not familiar with markdown, this [commonmark tutorial](https://commonmark.org/help/tutorial/) is a good place to learn the basics. 
    + You can preview your post with the preview tab.  This won’t look exactly the same as it will on your website, but is a good way to quickly check that your markdown styling is working correctly and you haven’t made typos.
    + You can also look through the example posts that came with the template website to see some other ways you can make your posts more interesting.
1. Save your changes by scrolling down to the "**Commit new file**" box.  Enter a brief description of the change, then click "Commit new file".
1. View your website and check to make sure you can see your new post, and that it looks the way you want. Remember that it may take a minute to update.  If the post hasn’t appeared, try [clearing your browser cache](https://github.com/C-MOOR/cmoor_website_template/blob/main/README.md#clear-browser-cache) and then refreshing the page.

 
Once you have some content of your own, you can go ahead and delete the example content that came with the website template.  To delete a post
1. Go to the `post` folder (`content/english/post`).
1. Click on the folder for the post you want to delete.
1. Within the folder for the post, click the `...` menu in the upper right and choose "**Delete directory**".
1. You will see one or more boxes indicating that the files were deleted, but they will not really be deleted until you save your changes.  Scroll down to the "**Commit changes**" box and click "Commit changes" to delete the files.
1. View your website, and check to make sure the post was deleted.  Remember that it may take a minute to update.  Remember that it may take a minute to update.  If the post hasn't disappeared, try [clearing your browser cache](https://github.com/C-MOOR/cmoor_website_template/blob/main/README.md#clear-browser-cache) and then refreshing the page.


### Add Assets

This video ([video](https://link.c-moor.org/video-student-website-post-assets))([slides](
https://docs.google.com/presentation/d/1iXwuC7qz3LuvIA1QXzHvUVCUn2OvkEoFdkLFoJgj8Dk/)) shows you how to add different types of media assets to your posts, including
+ documents such as PDF or text files
+ images
+ existing web content such as YouTube videos or Tweets

#### Add documents and files

1. Upload file
    1. From the main page of your repository, click on the folder named `content`.
    1. Click on the folder named `english`.
    1. Click on the folder named `post`.
    1. Navigate to the folder for the post that will link to the file.
        + It is important that the file lives in the same folder as the `index.md` file of the post that will link to it.
    1. Click the "**Add file**" button and choose "**Upload files**".
    1. Upload the file(s), then scroll down and commit your changes to save them.
1. Link to file
    1. Navigate to the folder for the post that will link to the file.  It should now have the file(s) you uploaded in addition to the `index.md` file.
    1. Click on the `index.md` file
    1. Click the pencil icon in the upper right to edit this file.
    1. To insert a link in your post, use square brackets around the text you want to act as a link, followed by parentheses around the name of the file you want to link to.  For example: `[click here](my_file.pdf)`  will make the words "click here" act as a link to the file `my_file.pdf`.
        + Make sure the link destination inside the parentheses matches your file name exactly, or your website won’t be able to find the file.
    1. Save your changes by scrolling down to the "**Commit changes**" box.  Enter a brief description of the change, then click "Commit changes".
    1. View your website and check to make sure the link shows up and correctly links to the file. Remember that it may take a minute to update.
        + If the post hasn’t appeared, try [clearing your browser cache](https://github.com/C-MOOR/cmoor_website_template/blob/main/README.md#clear-browser-cache) and then refreshing the page.
        + If the link shows up but gives an error when you click on it, double check that the link destination inside the parentheses exactly matches your file name.

#### Add images

1. Upload file
    1. From the main page of your repository, click on the folder named `content`.
    1. Click on the folder named `english`.
    1. Click on the folder named `post`.
    1. Navigate to the folder for the post that will contain the image.
        + It is important that the image lives in the same folder as the `index.md` file of the post that will contain it.
    1. Click the "**Add file**" button and choose "**Upload files**".
    1. Upload the image file(s), then scroll down and commit your changes to save them.
1. Link to image
    1. Navigate to the folder for the post that will link to the file.  It should now have the file(s) you uploaded in addition to the `index.md` file.
    1. Click on the `index.md` file
    1. Click the pencil icon in the upper right to edit this file.
    1. To insert an image in your post, use an exclamation point followed by square brackets, then parentheses around the name of the file you want to link to.  For example: `![](landscape.jpg)`.
        + Make sure the link inside the parentheses matches your file name exactly, or your website won’t be able to find the image.
    1. Save your changes by scrolling down to the "**Commit changes**" box.  Enter a brief description of the change, then click "Commit changes".
    1. View your website and check to make sure the image shows up and correctly links to the file. Remember that it may take a minute to update.
        + If the post hasn’t appeared, try [clearing your browser cache](https://github.com/C-MOOR/cmoor_website_template/blob/main/README.md#clear-browser-cache) and then refreshing the page.
        + If the image does not show up properly, double check that the link destination inside the parentheses exactly matches your file name.

#### Web assets

Hugo "shortcodes" extend markdown to enable easy inclusion of existing web assets (among other things).

+ To insert a YouTube video, use `{{< youtube w7Ft2ymGmfc >}}`.  Replace the ID with the ID from the video you want to include.
+ To insert a Tweet, use `{{< tweet 877500564405444608 >}}`.  Replace the ID with the ID from the tweet you want to include.

There are several other shortcodes available, you can learn about them in the [Hugo documentation](https://gohugo.io/content-management/shortcodes/).


## Troubleshooting

### Clear browser cache

Sometimes when you make edits to your website, you won't be able to see them (even though they were successful) because your browser has stored the old version of the website and is showing you that instead of getting the latest version.  You can fix this and get the latest version of your website by clearing your browser cache.

This will look a little different depending which browser you are using, but generally, you will

1. Open your browser preferences / settings
1. Look for an option labeled something like "**clear browsing data**".  It will probably be located under **Privacy or Security** settings.
1. Select the option labeled something like "clear cached files and images" or "clear cached web content".
    - You do not have to clear your cookies or browsing history.  It won’t cause problems with your website if you do, but you may get logged out of other sites if you clear your cookies, so it can be inconvenient.  You only *need* to clear the cached version of the website.
1. Click the button to clear the data
1. Once you’ve cleared your browser’s cached files, try revisitng your website and check if you see the updates you expect.



