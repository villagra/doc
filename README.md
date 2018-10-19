# Relevant docuemntation & links

## GIT
Git lol: http://uberblo.gs/2010/12/git-lol-the-other-git-log (log abreviation)  
git config --global --add alias.lol "log --graph --decorate --pretty=oneline --abbrev-commit --all"  

## Use keys on windows
1. Create a key for your github account  
ssh-keygen -t rsa -C "your-email-address"  

The following will show:
~~~~
Generating public/private rsa key pair.
Enter file in which to save the key (/c/Users/your_username/.ssh/id_rsa):
~~~~
Save the key in your username folder typing:
~~~~
c/Users/your_username/.ssh/id_rsa_IDENTIFIABLE_NAME_HERE
~~~~
For exmple:
~~~~
c/Users/villagra/.ssh/id_rsa_villagra
~~~~
This will generate two files, a id_rsa_villagra and a id_rsa_villagra.pub

2. Add the pub's file contents in your github account => settings => ssh and gpg keys.
3. Navigate to the repository you want to connect via ssh ahd type
~~~~
git config core.sshCommand "ssh -i c:/Users/villagra/.ssh/id_rsa_villagra"
git config user.name "test"
git config user.email test@test.com
~~~~
4. The git config file should loke like:
~~~~
[core]
	repositoryformatversion = 0
	filemode = false
	bare = false
	logallrefupdates = true
	symlinks = false
	ignorecase = true
	sshCommand = ssh -i c:/Users/villagra/.ssh/id_rsa_villagra
[remote "origin"]
	url = https://github.com/villagra/vue-resources.git
	fetch = +refs/heads/*:refs/remotes/origin/*
[branch "master"]
	remote = origin
	merge = refs/heads/master
[user]
	name = test
	email = test@test.com
~~~~

IMPORTANT: the url of the remote needs to be in the format of: git@github.com:test/test.com (ex: git@github.com:villagra/project.git). If the url is in a format of https://.... this won´t work.

## Nuget
NuGet Package Project https://marketplace.visualstudio.com/items?itemName=NuProjTeam.NuGetPackageProject

## Unity / Hololens
Streaming player plugin: http://renderheads.com/product/avpro-video  
Tutorials: https://www.raywenderlich.com/category/unity  
HoloToolkit-Unity: https://github.com/Microsoft/HoloToolkit-Unity  
HoloLensCompanionKit: https://github.com/Microsoft/HoloLensCompanionKit  
Unity3d + json.net: http://naplandgames.com/blog/2017/01/29/data-serialization-part-2-unity3d-json-net-and-twitter-rest-api/  
coroutines: http://twistedoakstudios.com/blog/Post83_coroutines-more-than-you-want-to-know  
Vectors tutorial: https://www.youtube.com/watch?time_continue=5&v=7DK8aA2qee8 (https://unity3d.com/learn/tutorials/topics/scripting/vector-maths)  

## UWP controls / demos
EasyCarousel https://github.com/validvoid/UWP_EasyCarousel  
What's new: https://github.com/EdiWang/WhatsNew.UWP  

## Xamarin links / docs
https://github.com/MarcBruins/awesome-xamarin

## Fonts
http://atipofoundry.com/fonts/noway
