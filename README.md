# Welcome to my monolith repo

I call it that because it is my first repo of git submodules

> The use case that I find appealing to submodules is how I am able to write custom logic for a interacting with libraries, but they can be isolated from my client code. How ever, I want to retain full access to source code.. And most importantly of all, I want some server files that are unique to this project.  It turned out that git submodules were a way to that, and bundle up all my code for passing it along to another developer.
>
> For a refresher on submodules:  https://www.youtube.com/watch?v=gSlXo2iLBros

`git submodule add [git url]`


## To get started run this command with the recurse flag

`git clone https://github.com/williamowen65/ghost-committee-web-app.git --recurse-submodules`


This will download 3 repos.
- 2 root level reops
- 1 nested repo.

Make sure to run `npm i` in each of those repo.

## Starting up the project

```

# Compile the web-app
cd ghost-glitch-deployment;
npm run dev;  # You can now view the local deployment (But it isn't wrapped in GAS)
# I prefer to push changes and view the deployment in GAS. 
# but you still need to run `npm run dev` to compile the web-app changes

# Deploy the web-app
# Push changes to 'https://042e05ef-7e72-41b3-a44f-e16f7cbd6383@api.glitch.com/git/few-right-mandible' 
# Which is the Glitch deployment - (Click to see the editor - https://glitch.com/edit/#!/few-right-mandible )
# If the app ever needs it, go to the terminal in the Glitch editor and run `refresh`






```






