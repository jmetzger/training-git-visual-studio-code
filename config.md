# git config

## How to delete an entry from config 

```
# Important: Find exact level, where it was added --global, --system, --local 
# test before
# should contain this entry 
git config --global --list 

git config --unset --global alias.log
```

## How set a value globally (for my user) 

```
git config --global user.name "Jochen Metzger"
git config --global user.email "j.metzger@t3company.de"
```
