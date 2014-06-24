subtreeTest
===========

git remote add subtree git@github.com:nomadmonad/subtreeOrigin.git
git subtree add --prefix subtree subtree master --squash

この状態でsubtreeOriginを取り込めた
取り込んだsubtreeOriginに変更を加え、pushしたところ、大本のsubtreeOriginには変更は反映されていない。

