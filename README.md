# Welcome to my monolith repo (Ghost Committee Web App)

I call it that because it is my first repo of git submodules

> The use case that I find appealing to submodules is how I am able to write custom logic for a interacting with libraries, but they can be isolated from my client code. How ever, I want to retain full access to source code.. And most importantly of all, I want some server files that are unique to this project.  It turned out that git submodules were a way to that, and bundle up all my code for passing it along to another developer.
>
> For a refresher on submodules:  https://www.youtube.com/watch?v=gSlXo2iLBros

Create a submodule
`git submodule add [git url]`

Keep your submodule up to date with their repos
`git submodule update --remote --merge`


## To get started run this command with the recurse flag

`git clone https://github.com/williamowen65/ghost-committee-web-app.git --recurse-submodules`

This will download 3 repos.
- 2 root level reops
- 1 nested repo.

Make sure to run `npm i` in each of those repo.

Also, it may be helpful to make sure each submodule branch is set to `main` rather than being a detatched head.


> IMPORTANT NOTE: If you are cloning this project to a new google account, these steps and links below won't work. They only work for a specific Google account.  
> Also see the `README.md` associated with each repo. 


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

# Update the app specific config for the Google Server
cd ghost-server-configuration
clasp login # make sure to have the correct chrome browser open
npm run push; # Pushes and deploys a new version of the GAS web-app


```

## Links

[GHOST Google Integration Spreadsheet](https://docs.google.com/spreadsheets/d/1sAka-Rs4LhHhkX3J4s7SaDlpIXEdv5R5Qm7meGIL6Wk/edit?gid=0#gid=0)

[GAS Editor](https://script.google.com/u/0/home/projects/1tXR1MZfheGId3kRfpmw4E4SSgdymw21h7lfeQTKdDhRjeQWHVSe86Hn8/edit)

[Google Cloud Project](https://console.cloud.google.com/welcome/new?hl=en&inv=1&invt=AblRKw&project=ghost-d319b)

[Netlify Deployment](https://app.netlify.com/sites/musical-meerkat-beaded/overview)

[Glitch Deployment](https://glitch.com/edit/#!/few-right-mandible)

[Squarespace](https://jaguar-sunflower-y9fm.squarespace.com/config/)

[Firebase](https://console.firebase.google.com/u/0/project/ghost-d319b/overview)

[live deployment](https://members.gigharboropenstudiotour.org/)

## Related Article

[“Put some GAS on it”](https://medium.com/@william.owen.dev/put-some-gas-on-it-51b1612f5444)
