# Unity-ReleaseNotes  [![cron](https://github.com/sator-imaging/Unity-ReleaseNotes/actions/workflows/cron.yml/badge.svg)](https://github.com/sator-imaging/Unity-ReleaseNotes/actions/workflows/cron.yml)

Update job starts on everyday 00:00 UTC. It may be delayed an hour or more due to busy time of GitHub Actions.


## Official Site (Alpha)

There is official release notes archives:
https://alpha.release-notes.ds.unity3d.com/



# Usage

`"<Package> Fixed"` to search fixed issues.
`filename:known <Package>` to search known issues.

`path:Unity<Version>` to specify version searching for.

> Note that GitHub search sometimes says "nothing found", reloading page will show correct result.


Examples:

- Recently fixed URP issues, except for alpha release:  
  https://github.com/sator-imaging/Unity-ReleaseNotes/search?o=desc&q=%22URP+Fixed%22+-alpha&s=indexed

- To see known URP issues in Unity 2021:  
  https://github.com/sator-imaging/Unity-ReleaseNotes/search?o=desc&q=URP+filename%3Aknown+path%3AUnity2021&s=indexed

- Recently fixed XR issues:  
  https://github.com/sator-imaging/Unity-ReleaseNotes/search?o=desc&q=%22XR+Fixed%22&s=indexed

- URP issues in Unity 2021, ascending order:  
  https://github.com/sator-imaging/Unity-ReleaseNotes/search?o=asc&q=URP+issue+path%3AUnity2021&s=indexed





&nbsp;  
&nbsp;  

## Devnote

How to delete all the releases and tags from remote repository.[^1][^2]

[^1]: [GitHub CLI](https://cli.github.com/) must be installed and authorized.
[^2]: Linux-compatible CLI environment is required on windows.


1. delete all releases.  
   `git tag | xargs -t -n 1  gh release delete`

2. delete all tags remaining on remote repository.  
   `git tag | xargs -t -n 1  git push --delete origin`

3. delete local repository tags if necessary.  
   `git tag | xargs -t  git tag -d`
