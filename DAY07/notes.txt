where the cretentials will store?

windows: credential manager


SSH KEYS
=========

How to generate ssh_keys?

ssh-keygen  

~/.ssh/
Id_rsa → private key
Id_rsa.pub —> public key

How to change algorithm ?

ssh-keygen -t dsa
Id_dsa
Id_dsa.pub

Explain the process how to generate?
—---------------------------------------------------
Step 1: ls -la ~/.ssh/ —-> check generated or not
Step 2: display cat ~/.ssh/known_hosts
Step 3: rm -rf ~/.ssh/known_hosts
Step 4: ssh-keygen —-> pls check if it is different , pls change with below command, delete existing one
Step 5: ssh-keygen -t rsa
Step 6: ssh-keygen -t rsa -f ~/.ssh/my_rsa_key  # Generates "my_rsa_key" and "my_rsa_key.pub" —--> Generates based on custom name.
step 7: cat ~/.ssh/id_rsa.pub —-> Take the content.
ste p 8:  click on profile→ settings → SSH and GPG keys—-> New ssh key—> paste the key —> save
Step 9: verify connection is established or not from your local to remote

   ssh -T git@github.com

It will ask yes , becz we deleted known_hosts.


Step 10: Go to the project folder and run the git remote -v
      [ It is pointing to HTTPS]

Step 11: git remote add sshurl git@github.com:jio-5g-india/Airtel-5g.git

Step 12: go and delete git hub credentials[ credentials manager / keychainaccess]

step 13: push the code now
      Git push <AN> <BranchName>


IQ: I am in a stage branch, how to create a branch(uat) from master without switch?
ANS: stage> git checkout -b uat master


Pull Request(PR)
================

readme.md file
==============

Branching strategy
------------------
