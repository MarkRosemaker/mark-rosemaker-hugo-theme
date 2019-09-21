# Mark Rosemaker Hugo Theme

This is the theme I use for (some of) my Hugo websites.
I created it because I wanted to have a minimalist, yet very powerful theme.
Thanks for checking it out.

## How To Install

1. Create a folder with the name of your site, create a subfolder named 'themes'.
2. Navigate to your themes folder and copy this theme and the themes it is based on as modules with the following commands:
  - git clone https://github.com/lgaida/mediumish-gohugo-theme
  - git clone https://github.com/JeremyLikness/jeremylikness-blog
  - git clone https://github.com/MarkRosemaker/mark-rosemaker-hugo-theme
3. Move the contents from themes/mark-rosemaker-hugo-theme/exampleSite to your site folder.
1. Put your logo.png in "content/uploads/".
2. Upload your logo to https://www.favicon-generator.org/, select "Generate icons for Web, Android, Microsoft, and iOS (iPhone and iPad) Apps", create favicon, download and copy all the file in the zip into "/static/img/favicons/".
3. Customize the config files etc. to your needs.

### Pro tip

Instead of cloning the themes into your project, clone all themes into a seperate folder called "hugo-themes". Then make symbolic links so that all in your files in "hugo-themes" are exactly the same as the theme folders of all your sites.

- mklink /j "%UserProfile%\OneDrive\Documents\GitHub\my-site\themes" "%UserProfile%\OneDrive\Documents\GitHub\hugo-themes"
- mklink /j "%UserProfile%\OneDrive\Documents\GitHub\another-site\themes" "%UserProfile%\OneDrive\Documents\GitHub\hugo-themes"
- mklink /j "%UserProfile%\OneDrive\Documents\GitHub\third-site\themes" "%UserProfile%\OneDrive\Documents\GitHub\hugo-themes"

**BUT** I've recently learned that [this is the way to do it](https://discourse.gohugo.io/t/hugo-modules-for-dummies/20758). I will update this guide to that effect.
