subtreeTest
===========

git remote add subtree git@github.com:nomadmonad/subtreeOrigin.git

git subtree add --prefix subtree subtree master --squash

この状態でsubtreeOriginを取り込めた

取り込んだsubtreeOriginに変更を加え、pushしたところ、大本のsubtreeOriginには変更は反映されていない。

-----------

subTreeでブランチを作成する場合、以下のコマンドを実行する
git subtree split --prefix subtree/ -b  subtreeSplitBranch

変更した内容は、以下のコマンドでリモートのリポジトリにpushできる
git subtree push --prefix subtree/ subtree  subtreeSplitBranch

このコマンドを実行後、リモートのリポジトリには新しくsubtreeSplitBranchが作成される
マージはsubtreeOriginのリポジトリ側で実施する。



