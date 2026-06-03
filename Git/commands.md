
Repository: A folder where Git tracks your project and its history.
Branch: Work on different versions or features at the same time.

1) Know the version post installation -  git --version
2) VS code as default editor - git config --global core.editor "code --wait"
3) Global mail and name - git config --global user.name "Your Name" ; git config --global user.email "you@example.com"

I made a repo on github first and cloned into it to begin with, created a folder called gitclones on my local and started working in that
alternate- just mkdir and git init, init is simply initialise 

4) Which file is pushed and not pushed, tracked or not - git status 

Now the best practice is staging and checking for problems but mostly i can afford pushing the wrong stuff, not interferring with any main branches obv 

5) To stage- Git add {Filename}
6) To unstage- Git restore --staged {filename}
7) To change the message- git commit --amend -m "Corrected message"
8) The Tag, Version adding a tagged bookmark to notify version- git tag -a v1.0 -m "Version 1.0 release"
9) Tag with commit or on specific 1 commit- git tag v1.1 <Commit hash >
10)See all tags- git tag
11) Delete a tag locally- git tag -d v1.0    
12) Delete remote tag- git push origin --delete tag v1.0
13) Difference between staged and in repo-  git diff --staged
14) Compare Two Commits- git diff <commit1> <commit2>
15) Show a Branch Graph- git log --graph
16) To create a new branch- git branch
17) To switch between branches- git checkout 
18) To see what is different from main- git status

Build > stage > commit with a quirky message 


Merging only when i am satisfied? 

19) git merge 

Switch Branch to main > merge with branch name

