# Quick set up guide 

## Generate a PAT 

To generate a Personal Access Token (PAT) from GitHub, follow these steps:

* Go to your GitHub account settings.
* Click on "Developer settings" in the left sidebar.
* Click on "Personal access tokens".
* Click on "Generate new token".
* Give your token a name and select the scopes you want to grant it.
* Click on "Generate token".
* Copy the generated token to a safe place, as you won't be able to see it again.



The token should have the following prermissions( [Title](https://github.com/myoung34/docker-github-actions-runner/wiki/Usage) )

* repo (all)
* admin:org (all) (mandatory for organization-wide runner)
* admin:enterprise (all) (mandatory for enterprise-wide runner)
* admin:public_key - read:public_key
* admin:repo_hook - read:repo_hook
* admin:org_hook
* notifications
* workflow

## In Unraid

* Set the PAT to your org token
* set the org name to ORG_NAME(for example: https://github.com/pta org name is pta ) 
* set /tmp/github-runner-your-repo to some share on your unraid NAS


Pro-Tip: Make sure the working patch is unique of you have multiple containers. Example Below: 
* /mnt/user/misc/actions-runner/user/project/1/
* /mnt/user/misc/actions-runner/user/project/2/
* /mnt/user/misc/actions-runner/user/project/.../

## All credit goes to myoung34. 
