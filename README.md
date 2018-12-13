
#### Branch 1.7.4

djgoku$ git status
On branch 1.7.4
nothing to commit, working tree clean
djgoku$ pre-commit run -c .pre-commit.yaml --all-files
Terraform docs...........................................................Failed
djgoku$ git status
On branch 1.7.4
nothing to commit, working tree clean


#### Branch 1.7.3

djgoku$ git checkout 1.7.3
Switched to branch '1.7.3'
djgoku$ git status
On branch 1.7.3
nothing to commit, working tree clean
djgoku$ pre-commit run -c .pre-commit.yaml --all-files
Terraform docs...........................................................Failed
hookid: terraform_docs

Files were modified by this hook.

djgoku$ pre-commit run -c .pre-commit.yaml --all-files
Terraform docs...........................................................Passed
djgoku$ git checkout master
error: pathspec 'master' did not match any file(s) known to git.
djgoku$ git status
On branch 1.7.3
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

  modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")
