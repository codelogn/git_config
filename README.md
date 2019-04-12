**Git SSH setup**

 `eval $(ssh-agent -s)`
 `ssh-add ~/.ssh/id_rsa`


Sample GIT ssh config example

Location: ~/.ssh/config

	Host github
		HostName github.com
		User git	
		PreferredAuthentications publickey
		IdentityFile ~/.ssh/id_rsa
		Port 443

**.gitconfig sameple configuration**

	[user]
		name = Robiul Robi
		email = robi@linux.com
	[core]
		longpaths = true
	[merge]
		tool = kdiff3
	[mergetool "kdiff3"]
		path = C:/Program Files/KDiff3/kdiff3.exe
		trustExitCode = false
	[diff]
		guitool = kdiff3
	[difftool "kdiff3"]
		path = C:/Program Files/KDiff3/kdiff3.exe
		trustExitCode = false
	[alias]
	  st = status
	  ci = commit
	  br = branch
	  co = checkout	
