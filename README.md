KernelMatchFinder
=================

KernelMatchFinder provides tools to get the best revision of an kernel blob, by diff each revision with the given one.

Quick Howto
Make a repository.
Add the (kernel) repo as remote and checkout a local branch. (git checkout -b remoteName / branchToCheckout)
Change into this repository and call the following
```
$KernelMatchFinderDir/searchBestBet $KernelMatchFinderDir/out_latest.txt ./filelist c73ed6e4d48639a298771e760083979705491c88 10901a16fe4de0f037d18d461ff5af694160dde1..omapzoom/p-android-omap-3.0 
```

Where
<br/><b>out_latest</b> contains the best matches.
<br/><b>filelist</b> contains a list of files, which as to be analyzed.
<br/>The commit is the base commit which is used as reference. <b>c73ed6e4d48639a298771e760083979705491c88</b>
<br/>The last argument specifies the search range, for example: <b>10901a16fe4de0f037d18d461ff5af694160dde1..omapzoom/p-android-omap-3.0</b>
