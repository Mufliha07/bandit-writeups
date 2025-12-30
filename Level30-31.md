# Bandit Level 30 → 31

## Goal
Clone the Git repository and find the password for bandit31

---

## Process


 1. Clone the Git repo through SSH on port 2220:

   ` git clone ssh://bandit29-git@bandit.labs.overthewire.org:2220/home/bandit29-git/repo`

2. Navigate to the cloned directory:

   `cd repo`

3. List files

     `ls -al`        -> no password is found in normal files   

5. Check git tags

    `git tag`       -> A tag named secret exists
 

6. View the content stored in the tag

    `view show secret`


## Password Found:

  fb5S2xb7bRyFmAvQYQGEqsbhVyJqhnDy


## Screenshot:

screenshots/Level30-31.png


## Notes:

 -Password was stored in a Git tag, not in files or branches.

 -Learned how to enumerate and read tags using git tag and git show.

 -Tags can contain hidden sensitive information.
