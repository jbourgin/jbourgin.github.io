## To clone
```
git clone git@github.com:jbourgin/jbourgin.github.io.git
```
Add submodule

```
git submodule update --init --recursive
```

## If submodule is buggy

Delete all elements related to the submodule

* Delete the relevant section from the .gitmodules file.
* Stage the .gitmodules changes git add .gitmodules
* Delete the relevant section from .git/config.
* Run git rm --cached path_to_submodule (no trailing slash).
* Run rm -rf .git/modules/path_to_submodule (no trailing slash).
* Commit git commit -m "Removed submodule "
* Delete the now untracked submodule files rm -rf path_to_submodule

Then

```
git submodule add -b master https://github.com/<USERNAME>/<USERNAME>.github.io.git public
```

## To update

Before adding changes :

```
./custom_pull.sh
```

or

```
git pull --recurse-submodule && git submodule update --recursive
```

Do changes, then :

```
./deploy.sh
```

Commit on master

```
git commit -a -m "blabla"
```
```
git push
```
