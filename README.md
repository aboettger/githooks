githooks
========

post-merge_checkinstall
-----------------------
Installation via checkinstall (http://checkinstall.izto.org/)
To use the scripts provided here in the githooks/postmerge it makes the most sense to work with symbolic links.

e.g.
ln -s  [githooks-checkout-path]/post-merge/post-merge_checkinstall [path-to-git-project]/.git/hooks/post-merge

postmergerc
-----------

Parameters can be passed via a configuration ([path-to-git-project]/.git/hooks/postmergerc) in json format.

e.g.
{
  "autogen": "",
  "configure": "",
  "make": "",
  "checkinstall": "--exclude /usr/local/lib/python2.7/dist-packages/easy-install.pth"
}
