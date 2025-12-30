# Bandit Level 29 → 30

## Goal
Clone the Git repo on localhost, explore branches, and find the password hidden in a non-master branch.

---

## Process

1. Go to home directory  ->   `cd~ `

2. 1. Clone the Git repo through SSH on port 2220:

   ` git clone ssh://bandit29-git@bandit.labs.overthewire.org:2220/home/bandit29-git/repo`

3. Move into the cloned repository:

   `cd repo`

4. List all available branches

     `git branch -a`    

5. Switch to the dev branch

    `git checkout dev` 


6. View files in dev branch

    `ls`

7. Read the file that stores the password:

     `cat README.md`


## Password Found:

  qp30ex3VLz5MDG1n91YowTv4Q8l7CDZL


## Screenshot:
screenshots/Level29-30.png

## Notes:

 -Password was found in a non-main branch (dev), not in main/master.
 -Learned branch enumeration and switching in Git repositories.
 -Sensitive info can exist in hidden or developer branches.
