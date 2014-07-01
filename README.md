githooks
========

post-merge_checkinstall
-----------------------
Installation via checkinstall (http://checkinstall.izto.org/).
To use the scripts provided here in the githooks/post-merge it makes the most sense to work with symbolic links.

```ln -s  [githooks-checkout-path]/post-merge/post-merge_checkinstall [path-to-git-project]/.git/hooks/post-merge```

Parameters can be passed via a configuration ([path-to-git-project]/.git/hooks/postmergerc) in json format.

postmergerc:

```{
  "autogen": "",
  "configure": "",
  "make": "",
  "checkinstall": "--exclude /usr/local/lib/python2.7/dist-packages/easy-install.pth"
}```

post-merge_4_atom
-----------------
Automatic creation of a deb package for atom (https://github.com/atom)
To use the scripts provided here in the githooks/post-merge it makes the most sense to work with symbolic links.

```ln -s  [githooks-checkout-path]/post-merge/post-merge_4_atom [path-to-git-project-atom]/.git/hooks/post-merge```
