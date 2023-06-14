# permission denied

chmod +x ./scripts/npm-basic-package.sh

# run sh file

./scripts/npm-basic-package.sh

To copy the contents of a private repository into a new public repository on GitHub, you can follow these steps:

1. Create a new public repository on GitHub.
2. Clone the original private repository to your local machine using Git.
3. In your local repository, remove the remote origin that points to the private repository by running the following command in your terminal:
```
git remote remove origin
```
4. Add a new remote origin that points to your new public repository by running the following command in your terminal:
```
git remote add origin <new repository URL>
```
Replace `<new repository URL>` with the URL of your new public repository.
5. Push the contents of your local repository to the new public repository by running the following command in your terminal:
```
git push -u origin master
```
This will push the master branch of your local repository to the new public repository.

Note that this process will copy the contents of the original repository to the new repository, but it will not copy any of the history or commit messages from the original repository. If you want to preserve the commit history, you can try using Git's `git clone --mirror` command to clone the original repository, and then push the mirrored repository to your new public repository.
