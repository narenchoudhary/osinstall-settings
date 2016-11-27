# Bashrc Alias

Append these to `~/.bashrc`.

    alias activate="source venv/bin/activate"
    alias py="python"
    alias py3="python3"
    alias user="ssh user@ip"
    
    # clear alias
    alias x="clear"
    alias c="clear"
    alias clea="clear"

    # vim alias
    alias vi="vim"
    alias vmi="vim"
    
    # explore current folder in nautilus
    alias explore='nautilus .'
    
    # open the file using default app (the one used for double-click opening)
    alias try='gnome-open'

    alias ..='cd ..'
    
    # rm protection
    alias rm='rm -i'

    # apt-get
    alias aptdate='sudo apt-get update'    
    alias aptgrade='sudo apt-get upgrade'    
    alias aptinst="sudo apt-get install"
    
    alias gitcl="git clone"
    alias gitcm="git commit"
    alias gitp="git push"
    alias gitl="git log --oneline"
    alias gitst="git status"
    alias gitb="git branch"

