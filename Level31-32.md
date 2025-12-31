# Bandit Level 31 → 32

## Goal
Clone the Git repository and submit the required key file to unlock the next level password.

## Process

1. **Clone the repository**

   `git clone ssh://bandit31-git@bandit.labs.overthewire.org:2220/home/bandit31-git/repo`

   (Downloads the remote repo to the local machine)

2. **Enter the cloned directory**

   `cd repo`

   (Navigate into the project folder)

3. **List files**

   `ls -la`

   (View all files including hidden ones to understand repo contents)

4. **Read the README**

   `cat README.md`

   (Check instructions — reveals that we must create and submit a key file)

5. **Create the required key file**
 
   `echo "May I come in?" > key.txt`

   (Generate the file with exact required text)

6. **Force add the ignored file**

   `git add -f key.txt`

7. **Commit the file**

   `git commit -m "Submit key file to unlock next level"`

   (Save the staged file into Git history)

8. **Set default branch as main**

    `git branch -m master main`

9. **Force push to sync branch**

   `git push origin main --force`

10. Submitted and pushed the required key file via Git, the server validated it successfully and returned the password for next level.

## Password Found

   3O9RfhqyAlVBEZpVb6LYStshZoqoSx5K

## Screenshot

screenshots/Level31-32_(1).png

screenshots/Level31-32_(2).png

screenshots/Level31-32_(3).png

## Notes

- Learned how to force add ignored files using git add -f.


