---
title: NetlifyCMS configuration
---
# NetlifyCMS configuration
In '.vuepress/public/config.yml' change the repo name

```
backend:
  name: github
  repo: capriosa/vuepress-deploy
  branch: master
```
Then add an Oauth app to your github account: https://github.com/settings/developers
For the Authorization callback URL, enter https://api.netlify.com/auth/done.

When you complete the registration, you’ll be given a Client ID and a Client Secret for the app. You’ll need to add these to your Netlify project:

    Go to your Netlify dashboard and click on your project.
    Navigate to Settings > Access control > OAuth.
    Under Authentication Providers, click Install Provider.
    Select GitHub and enter the Client ID and Client Secret, then save.

Now you can loggin to your NetlifyCMS with '/admin' after the URL of your site.

