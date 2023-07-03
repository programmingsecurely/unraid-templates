# Quick set up guide 

## In Github
* Go to your personal repository on Github.
* Click on the "Settings" tab.
* Click on "Actions" in the left sidebar.
* Click on "Add runner".
* Copy the token and url  that shows up in the configure section. Ex: 

```

./config.cmd --url --> [URL] <---  --token --->[TOKEN]<--->
```
## In Unraid


* set URL and Token to above the above information
* set /tmp/github-runner-your-repo to some share on your unraid NAS


Pro-Tip: Make sure the working patch is unique of you have multiple containers. Example Below: 

/mnt/user/misc/actions-runner/user/project/1/
/mnt/user/misc/actions-runner/user/project/2/
/mnt/user/misc/actions-runner/user/project/.../

