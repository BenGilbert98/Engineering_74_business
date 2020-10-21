# This is the guide to create git and github connection with SSH key
## Windows Guide
create a github account

copy the ssh key from localhost with
```
cat id_rsa.pub
```
-paste the public key on your github in settings GPG SSH key option in your profile manue
-once saved go back to your terminal
-run the git hub command
```
git add .
git commit -m " msg"
git push -u origin main
```

- Download Git or GitBash
- Run GitBash
- `cd`
- Make a folder 
- Enter the folder
- Generate a key
- `ssh-keygen -t rsa -b 4096 -C "your_email@email.com"`
- Save as "key.ssh"
- Make a passphase
- `SHA256:YOUR_KEY_HERE your_email@email.com`

a random art image should then be displayed


- Check that `key.ssh` exists with `ls`
- Ensure you have git-agent `eval $(ssh-agent -s)`
- Add the key `ssh-add key.ssh`
- Go to your [Github](www.github.com) and go to `Settings`
- "SSH and GPG keys" => "New SSH Key"
- Back to terminal `cat key.ssh.pub`
- Copy into terminal
- Paste it in your New SSH Key window and add a title
- Back to terminal test your SHH to GitHub

- Go to [Github](www.github.com) make a new repo
- With your folder from before open in Bash
- To initialize a repo use `git init`
- If you have files in that folder use `git add <file_name>`
- If you want to add all files `git add .`
- If you want to make a file `touch FILE_NAME.FORMAT`
- Edit the file
- or use `nano README.md` => Save with `CTRL + X`
- `git commit -m "commit name"` => Commit all the files
- `git branch -M main` => Makes the "main" branch
- `git push -u origin main` => Uploads all files


## Making Changes to files:
- You need to add those files again `git add .`
- Make a new commit `git commit -m "Message"`
- Push to origin ` git push -u origin main`


## Common Commands
Create file 
`touch file_name`

Delete file
`rm file_name`

Delete directory
`rm -rf directory_name`

Move file
`mv file_name new_location/`

Rename file
`mv file_name new_file_name`

Copy file
`cp file location/`

Edit file (using editor such as vi, nano)
`editor file_name`

See what is in the directory
`ls directory/`

See hidden files in directory also
`ls -a directory/`

Add image to file
`![](file_location)`

to create markdown name_of_file.md
