# Exercise 3 - Configuring your first repository

1. Enable color

        git config --global color.ui auto

2. Set your name

        git config --global user.name "John Doe"

3. Set your email address

        git config --global user.email "john.doe@somewebsite.com"

4. Why did we use the `--global` flag?  (What does that do?)
        
        We use global level configurations so that entries are user specific. These values are stored in a file located un the user's home directory.


5. Check your git config to show the changes you have made

        git config -l
        C:\cisw17\my_repository>git config -l
        diff.astextplain.textconv=astextplain
        filter.lfs.clean=git-lfs clean -- %f
        filter.lfs.smudge=git-lfs smudge -- %f
        filter.lfs.process=git-lfs filter-process
        filter.lfs.required=true
        http.sslbackend=openssl
        http.sslcainfo=C:/Program Files/Git/mingw64/ssl/certs/ca-bundle.crt
        core.autocrlf=true
        core.fscache=true
        core.symlinks=false
        pull.rebase=false
        credential.helper=manager-core
        credential.https://dev.azure.com.usehttppath=true
        init.defaultbranch=master
        user.name=Stefania Castaneda
        user.email=steffcastaneda18@gmail.com
        color.ui=auto
        core.repositoryformatversion=0
        core.filemode=false
        core.bare=false
        core.logallrefupdates=true
        core.symlinks=false
        core.ignorecase=true
        remote.origin.url=https://github.com/chefsteff3/my_repository. git
        remote.origin.fetch=+refs/heads/*:refs/remotes/origin/*

For more information, check out [Customizing Git Configuration](https://www.git-scm.com/book/en/v2/Customizing-Git-Git-Configuration)