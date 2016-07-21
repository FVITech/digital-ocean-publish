#Publishing to Your Digital Ocean space with Git

As an FVI student, one of the benefits we provide you with is the ability to use our digita ocean virtual machine. In here, you can run node processes, php servers, and regular html sites. It's critical that you make use of this facility so that we have something to show prospective employers when we try to help you find jobs.

#Instructions to Publishing

1. First you have to ssh into our virtual machine. You do this by running the following command:  

```bash
ssh [yourusername]@fvi-grad.com
```
Note: your username is usually first initial and last name. For example if your name is Ash Oak, your username would be aoak.  

2. Once you are logged into the shell of the virtual machine, you can create the git remote repo by running the following command, which we have created for your convenience:  

```bash
fvigit [reponame]
```
Replace [reponame] with the name you want to give your remote repo. It's usually wise to choose the same name you gave your folder locally.  

3. Back on your local machine, add this newly created repo as a remote to your local repo:  

```bash
git remote add digi ssh://[yourusername]@fvi-grad.com/home/students/[yourusername]/[yourusername].fvi-grad.com/[remotereponame]
```

4. Publish to the remote repository by running the following command from your local machine:

```bash
git push digi master
```

You can push whichever branch you want, not just master.
