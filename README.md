# hugo-portfolio
Started learning Hugo on June 16 2021 6 PM - 9 PM at Robotic Systems, Australia from the Newcastle Coders Group, tutorial hosted by Sora and Sharlene. After that night, I have continued building it up and learning how to use it such as integrating a headless CMS Ghost and tuning different themes.

## What I have Learned
### June 17 2021
1. hugo serve
2. "echo" and ">>.env" is not needed in .env to call on Ghost CMS URL and Key.
3. `git commit` -> `git pull` -> `git push` in solving the deployment failure with Netlify 
4. `git submodule update --force --recursive --init --remote` to refresh submodule
5. Problem: Netlify could not deploy site, Solved - modified Netlify.toml to have a simple command `hugo` instead of `hugo && npm run build:functions`.
6. Goal: to have Netlify automatically updated when Ghost CMS has a new post - figured that netlify.toml must have a command at their [Build] called `run npm start && hugo` with `start` being the build script in package.json. 

## Useful Websites
- [Hugo Tutorial by Sora and Sharlene](https://tutorial-blog.netlify.app)
- [When retrieving a remote repo (needed for the theme of Hugo)](https://docs.github.com/en/github/getting-started-with-github/getting-started-with-git/about-remote-repositories)
- [Ghost CMS with Hugo](https://www.gojamstack.dev/posts/ghost-cms-hugo/)
- [Using git submodule to host on Netlify](https://gohugo.io/hosting-and-deployment/hosting-on-netlify/#use-hugo-themes-with-netlify)
