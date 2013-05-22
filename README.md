Razorfish Playground
========

#### What is it ####

Razorfish playground is a place where we can access, or quickly build experiments exploring a particular technology.


### Examples ###
[![Wonderwall](http://raw.github.com/andrevenancio/razorfish-playground/master/wonderwall/preview.png)](http://andrevenancio.github.com/razorfish-playground/wonderwall/wonderwall.html)
[![Simple Noise](http://andrevenancio.github.com/razorfish-playground/preview.png)](http://andrevenancio.github.com/razorfish-playground/wonderwall.html)
[![Simple Noise](preview.png)](wonderwall.html)


### Dependencies ###

This git repo makes use of 3 other external git repositories. Stats.js, dat-GUI and Razor. If you just download a zip file of this repo, you wont be able to run it. Always make a clone on your machine.


### Submodules ###

If any of the tools used are git repositories from other authors, we should install them as a submodule.

To install a new submodule, Open the Terminal, go to the razorfish-playground root folder and type the following :
```
git submodule add <remote-repository.git> <local-path>
```
An example could be: `git submodule add https://github.com/mrdoob/stats.js.git template/lib/stats.js` hosted on github or `git submodule add https://code.google.com/p/dat-gui/  template/lib/dat-gui` hosted on Google Code.
If you wish to just update a submodule to the latest version, go to the root of the submodule and type:
```
git pull origin master
```
If you wish to remove any submodule:
* Delete the relevant section from the .gitmodules file.
* Delete the relevant section from .git/config.
* Run the following in the Terminal:

```
git rm --cached path_to_submodule (no trailing slash).
```
* Commit to git, and then delete the now untracked submodule files, finally on Terminal:
```
rm -rf path_to_submodule
```


### Change Log ###
2013 05 22
* added simple noise example.
* added wonderwall example.

2013 05 17
* added `razor` submodule, hosted on github.
* added `stats.js` submodule, hosted on github.
* added `dat.GUI` submodule, hosted on google code.
* added base html, css and javascript templates.
