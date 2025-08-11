# Background

**TLDR: CO2 decided to migrate the Bucket docs here to solve some problems. He is asking for your support and help to finalize this.**

----

The documentation for the #xkcd Bucket has been migrated several times.

It was originally hosted on the long-gone xkcd wiki.

When that wiki went down, we placed a copy in the legacy wiki of the Bucket source code repo ([link](https://github.com/zigdon/xkcd-Bucket/wiki/Using-the-%23xkcd-bucket)).
This only worked due to a series of coincidences:
- Github's legacy wiki allowed mediawiki formatting, making it easy to migrate the docs.
- Github's legacy wiki was built before repo-level authentication - meaning that anyone with a Github account could edit it.
  - This was convenient because zigdon is no longer involved with the xkcd IRC channel.
  - It also has a risk of vandalism, although this luckily never happened.
 
Just before the creation of this repo, a problem turned up.

While the legacy wiki is still live, it seems that Github is putting in so little effort to keep supporting it, **that recently several users have reported a rendering timeout when trying to view the docs.**

I don't think this is ideal.

I also don't think moving it into another section of zigdon's Github repo is a good idea, because he is no longer really involved in the IRC channel. Better if it is managed somewhere by an active #xkcd user, so here.

By putting it in a regular GitHub repo, it also becomes much easier to hand over if this is ever needed.

# Todo

Because the documentation has been untouched for so long, it is quite outdated in some places.

The following tasks should ideally be done, in order of priority:

- [ ] Review CO2's conversion from mediawiki format into markdown format for glaring errors. (By comparing it to the [old wiki page]([https://github.com/zigdon/xkcd-Bucket/wiki/Using-the-%23xkcd-bucket](https://github.com/zigdon/xkcd-Bucket/wiki/Using-the-%23xkcd-bucket/56e023e11fd9821e9aefde912783f6caed528cae), you may have to retry several times for it to load).
- [X] Update the links in the main Bucket factoids "newbie pack" and "docs" to link here (can be done by channel ops).
- [X] Replace the documentation page in the legacy wiki in zigdon's repo with a link to this repo (can be done by anyone with a GH account).
- [ ] Clean up the very old broken links in the documentation (marked by CO2 with a todo).
- [ ] Check for any cases where the documentation has become inaccurate due to changes in Bucket's settings etc and fix those.

# Access and updating

- If you want to help, please make a pull request. Once you do that, if I don't notice it quickly feel free to let me know on IRC.
   - If, in the PR, you complete one of the above checkboxes, please mark it as done.
- In case you want to help but don't know how to make a Github PR, hit me up on IRC and we'll figure something out.
- If you are a trusted #xkcd regular, especially ops, I am willing to give you direct edit/merge access to this repo. PM me on IRC.
