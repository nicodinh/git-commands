- http://stackoverflow.com/questions/1270514/undoing-a-git-push
- http://stackoverflow.com/questions/35330868/what-is-the-best-practice-for-using-git-on-multiple-projects-with-the-same-base
- https://coderwall.com/p/_8dxjw/merging-a-pull-request-locally
- use "git reset HEAD <file>..." to unstage
- merge local master to dev branch: http://stackoverflow.com/questions/20101994/git-pull-from-master-into-the-development-branch
- merge local dev branch to master: http://stackoverflow.com/questions/5601931/best-and-safest-way-to-merge-a-git-branch-into-master and rebase

# demo pull request
- a partir du master repo et branch
- git ls-remote origin
- git fetch origin refs/pull/30/head
- git merge --no-ff FETCH_HEAD (git checkout -b nicodinh-meteor1.3 FETCH_HEAD)
- fix conflict
- git rebase -i (drop etc..)
- git push origin meteor1.3
