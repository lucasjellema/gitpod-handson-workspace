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

## Open Gitpod Workspace in local VS Code Desktop

Try to open a workspace in your local VS Code desktop for the smoothest dev experience (using port forwarding for services and web applications). 
![image](https://user-images.githubusercontent.com/1296324/202265821-1faa9cc3-21fa-4cc2-8add-163ec5b83e9b.png)

You need the MS Remote SSH extension for VS Code:
![image](https://user-images.githubusercontent.com/1296324/202265701-ffe9492d-ff60-40e7-96c5-203d1ecedb70.png)

Also install the VS Code extension Gitpod Remote
![image](https://user-images.githubusercontent.com/1296324/202265866-5ac13ef4-3db9-4f2f-9c42-ca6ab900dcc6.png)

Open the command palette in VS Code in the browser. Select Gitpod - Open in VS Code.
![image](https://user-images.githubusercontent.com/1296324/202265911-37a26892-3d50-4258-95bc-d8cfc18d537c.png)

You will be asked:
* Open Visual Studio Code?
* Copy the this temporary password
* Allow an extension to open this URL?
* Enter password for remote connection

as shown in this picture.
![image](https://user-images.githubusercontent.com/1296324/202266010-244eeff3-1a53-4d4d-a997-64eb159f8c0a.png)

Please comply and provide as requested.

You can now work locally against the CDE (Cloud Development Environment) - the cloud based Gitpod workspace environment. Try to type in the local editor and quickly check the browser based editor - and vice versa. Be really quick! They seem pretty well synchronized.

Note: If you run a web application or a service that opens ports, you may want to forward ports - make sure that attempts to access localhost:SOME_PORT are forwarded correctly over the SSH connection to the Gitpod workspace environment.

![image](https://user-images.githubusercontent.com/1296324/202266756-39b4b3cb-dbd8-4b9e-b4ee-a8e8450a29d6.png)


## Collaborating in your Workspace

You can invite othes to come and join you in your workspace. It is similar to collaborating on Google Docs, in that you can see who is online and look at the same code and processes. It is like others working on your machine at the same time as you. You do not actually live share an editor though. 

See: [Gitpod Docs on Sharing a running Workspace](https://www.gitpod.io/docs/configure/workspaces/collaboration#sharing-running-workspaces).

Now invite a colleague to visit your place - and get a feel for working together.

## Workspace Snapshots

A snapshot of a workspace is the workspace with all its files in all directories - the result of all your manual steps. A snapshot can restore a workspace in that exact same state (including files that were not committed to git and/or were installed outside of the /workspace directory. A URL can be retrieved for a snapshot - and that URL can be shared with others. Snapshotting a workspace is useful when you want to create reproducible workspace state for reporting support issues, or when giving training, or presentations. You can create up to three snapshots from any workspace.

Note: a snapshot does not have any running processes (besides what is defined in tasks to run for workspace restart).

See [Gitpod Docs on Snapshots of Workspaces](https://www.gitpod.io/docs/configure/workspaces/collaboration#sharing-snapshots).

Create one or two files in this workspace. Change one of the files already there. Do not commit any file. Now create a snapshot:

Run "Gitpod: Share Workspace Snapshot" from the hamburger menu at the top left of VS Code, from the Gitpod menu at the bottom, or via the VS Code command palette. Once you execute the command, the snapshot is taken and the URL is shown in a dialog.

Share the URL with a colleague, ask them to open the URL and verify that see the workspace as you defined it. Alternatively or additionally, open a new browser window and navigate to the snapshot URL. Check that you see the exact same situation as in the original workspace.

Note: the snapshots are a capture of a specific point in time. From this point on, the workspace forks from the snapshot. Changes in the workspace will not affect the snapshot. Any workspace opened from the snapshot is also a clone from the snapshot that is immediately cut loose from it.


## GitHub Codespaces
In November 2022 (10th November to be exact) GitHub Codespaces broke out of limited preview into general availability. 
![image](https://user-images.githubusercontent.com/1296324/202263296-16d750fb-be12-46b0-ae57-a2a1a5aae7a2.png)

We can use a GitHub Codespace in a similar way to a Gitpod Workspace - although only for GitHub repositories and not like Gitpod for GitLab repos or other git repositories. The definition of a GitHub Codespace environment is not defined in a .gitpod.yml file but instead in a devcontainer.json file that serves a very similar purpose in a quite similar way.

You can open a GitHub Codespace for this current repository with the following steps:

Open the GitHub Repository [https://github.com/lucasjellema/gitpod-handson-workspace](https://github.com/lucasjellema/gitpod-handson-workspace). Click on the `<>Code` button. Then select the `Codespaces` tab. Click on button `Create codespace on main` to create the Codespace.   

![image](https://user-images.githubusercontent.com/1296324/202264071-c023d0a8-2f91-48f8-8998-c713ed41c6e9.png)

After a few seconds, VS Code will appear in the browser with the contents from the GitHub repository. You can open terminals (running Bash in an Ubuntu VM) and do more or less the same things as in the Gitpod.

You can open the Codespace in VS Code desktop as well. This requires you to install the GitHub Codespaces extension in VS Code. Once you have installed the extension, the Remote Explorer will show Codespaces as an option.

![image](https://user-images.githubusercontent.com/1296324/202265029-93737dfb-f0bf-4244-9c59-710962fa00aa.png)

When you select the option GitHub Codespaces, you will be invited to sign in to GitHub:
![image](https://user-images.githubusercontent.com/1296324/202265133-2020c4f8-33ab-4e19-a210-c284c1678d4f.png)

Go through the MFA steps to confirm the operation. 
![image](https://user-images.githubusercontent.com/1296324/202265242-e3bfdb28-1d90-48b6-a7c8-27991360ae2e.png)

When the connection is established, a list is shown of your GitHub Codespaces 
![image](https://user-images.githubusercontent.com/1296324/202265322-d47868b1-641b-4e13-8bfb-797af2f2d2c9.png)

And you can select on to open in VS Code desktop - which will take a little while:
![image](https://user-images.githubusercontent.com/1296324/202265369-12ad66a6-2351-4285-be5f-b46369b9ef3c.png)

As in Gitpod, ports can be forwarded from local laptop to GitHub codespace in the cloud:
![image](https://user-images.githubusercontent.com/1296324/202265477-878e74e5-1223-4379-9f20-368270fc6044.png)



