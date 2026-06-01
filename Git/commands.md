
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

Build > stage > commit with a quirky message 

