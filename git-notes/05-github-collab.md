## Github

<https://github.com/ucla-data-archive/ucla-py-notes/blob/master/git-notes/05-github-collab.md>
<http://swcarpentry.github.io/git-novice/07-github/index.html>

* create a repo for planets

**Objectives: collaborate pushing to common repo**

1. Pair up students, one will be `owner` and another `collaborator`
1. In the **owners** planet's repo on GitHub, click settings, select collaborators, enter partner's git username
1. Partner should `cd` to another directory (Desktop) and make copy of partner's repo:
   * `cd ~/Desktop`
  ~~~
   git clone https://github.com/vlad/planets.git (replace vlad with your partner's name)
  ~~~
1. Collaborator should make changes, add, commit, git push origin master, e.g. add a new file called `pluto.txt` with text
1. Owner can pull changes onto their machine

**Change roles and repeat**

## Dealing with conflicts

1. Continuing from above (the repo you are working together in) -
1. Each partner adds a (different) line to `mars.txt`, adds, commits, pushes to github
1. The first push will get in and the second push will fail
1. Failed pusher should:

~~~
git pull origin master
~~~

1. reconcile change and remove markers (you can accept the remote or local changes or add something else)

~~~
git add, status, commit, push
~~~

1. other partner can pull without additional changes needing to take place

## Collaboration Exercise

1. collaboration tool: https://github.com/jt14den/git-collaboration
1. students can fork the repo
1. explain forking: making own copy of a repo that isn't owned by you
1. make changes to one of the countries (do this on github)
1. submit pull request to original owner
