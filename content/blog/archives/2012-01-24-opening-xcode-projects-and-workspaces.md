---
layout: post
title: opening xcode projects and workspaces
categories:
- "on"
updated_at: 2012-01-24
uuid: F4F0718A-4DB4-4026-820C-DF7C7BA1CA5C
---


In honour of [CocoaPods](https://github.com/CocoaPods/CocoaPods), which I've been experimenting with lately I figured 
it was time to update an old bash script I was using multiple times daily. It started off extremely simple as an alias.


```
alias openx="open *.xcodep*"
```


And ended up turning into a script that checks for whether there are any xcworkspaces, and if so loading the first of 
them only. Failing that it looks for an xcode project. As this is in general the order you should be opening them. 
It's useful to me. Could be for you.


```
openx(){ 
  if test -n "$(find . -maxdepth 1 -name '*.xcworkspace' -print -quit)"
  then
    echo "Opening workspace"
    open *.xcworkspace
    return
  else
    if test -n "$(find . -maxdepth 1 -name '*.xcodeproj' -print -quit)"
    then
      echo "Opening project"
      open *.xcodeproj
      return  
    else
      echo "Nothing found"
    fi
  fi
}
```
