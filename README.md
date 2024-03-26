# PLPBasicGitAssignment
How you can document the steps and commands used in a text file or README.md in your repository:
# Pushing Code to Repository Using SSH

This guide explains how to push code to a Git repository using SSH authentication. Follow these steps:

1. **Generate SSH Key**:
   If you haven't already generated an SSH key, use the following command:
   ```bash
   ssh-keygen -t rsa -b 4096 -C “samuelmwai031@gmail.com”
Add SSH Key to Your SSH Agent: Add your private key to the SSH agent with the following command:
ssh-add ~/.ssh/id_rsa
2.	Add SSH Key to Git Service: Copy the contents of the public key (~/.ssh/id_rsa.pub) and add it to your Git service account (e.g., GitHub, GitLab, Bitbucket).
3.	Clone the Repository: Clone the repository using the SSH URL:
git clone git@github.com:Samuel-06M/PLPBasicGitAssignment.git
4.	Make Changes and Commit: Make changes to the files in the repository, then add and commit those changes:
git add hello.txt
git commit -m "Add hello.txt with a greeting"

5.	Push Changes: Push your changes to the remote repository:
git push origin main

6.	Enter SSH Passphrase: If you've set up an SSH passphrase, you'll be prompted to enter it.
That's it! Your changes should now be pushed to the remote repository using SSH authentication.


