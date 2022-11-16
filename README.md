# Gitpod workspace for exploring Gitpod

Getting to know Gitpod is the objective of this repository. 

For starters - open this reposutory in a Gitpod workspace.
[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/lucasjellema/gitpod-handson-workspace)

The link under this button is `https://gitpod.io/#https://github.com/lucasjellema/gitpod-handson-workspace`. It is composed from the base URL for Gitpod (https://gitpod.io/), then the # followed by the full URL (including https://) of the GitHub repository for which this workspace should be opened.

You can do the same thing with any other repository on GitHub. Browse around - pick a repository (one of your own, one for your favorite open source project) and copy its URL. Then paste in the location bar of your browser: `https://gitpod.io/#<URL for the GitHub repo you selected>` and see a brand new Gitpod workspace open up for that repository. Note: you can make this a more focused operation by opening the workspace for a specific branch, (release) tag or PR.
![image](https://user-images.githubusercontent.com/1296324/202258047-23155a52-6b8c-4fd7-9c34-425f68328a2f.png)


## Workspace Customization
The workspace you opened from the button in this document is not entirely unprepared. It is based on the Gitpod default image - which has a lot of stuff installed out of the box. You will find the language runtimes for Go, Java, Node.js, C/C++, .Net, Python, Ruby, Rust & PHP, Clojure. Additionally among the many tools included in this image are git, Docker, Docker Compose, Maven, Gradle, npm, jq, Nix, Homebrew, Tailscale, Nginx. 

In addition to the contents of the base image, and the sources from the GitHub repository for which the workspace was created there are some additional things installed. The installation took place when the workspace was started - when Gitpod executed the instructions in file `.gitpod.yml`. Check out this file and see how it installs ...

## 

The handson suggests you try to open a workspace in your local VS Code desktop for the smoothest dev experience (using port forwarding for services and web applications). We also briefly look at collaboration (sharing a workspace) and workspace snapshots.

Finally, the handson will briefly refer to GitHub Codespaces as an alternative to Gitpod.
