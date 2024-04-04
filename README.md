# Next Blogger Content Repo

## How to Set-up
Use this repo as Content-Repo for your Next Blogger Project
We use Tina CMS to handle and provide content to blog via github repo.

- [ ] Create a Accound and Project on the Tina CMS using this Content-Repo
  - [ ] Use this Content-Repo to create project on Tina CMS
  - [ ] For Site Urls : Add localhost Or url of your Next-Blogger Project where you have hosted it ( vercel or netlify )
  - [ ] Copy CLIENT ID and Tokens from tina-cms project and paste it to .env file of the Next-Blogger Project
  - [ ] Media section of project and enable and sync it. 

We will be using github action to ping Next-Blogger project, to build the site on every update to this Repo.
which means each time you update the blog content through /admin, it will trigger the build process on Next-Blogger.
- [ ] ( Vercel ) Go to Vercel deployment, Settings > Git > Deply Hooks. 
  - [ ] Create a hook with any name and with main branch
  - [ ] Copy the Hook api url ( we will call it HOOK_API)
- [ ] Go to github Content-Repo.
  - [ ] Settings > secreats and variables > variable > Repository Variables
  - [ ] Add new repository Variable with name DEPLOY_HOOK and value as HOOK_API ( what we copied on vercel site )

- [ ] And All Set!

