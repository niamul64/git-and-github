# command for git:

### Make directory/ folder: 
                                                            mkdir [folder name]
### See all the file or folder in a directory(for windows):
                                                            dir
### See all the file or folder in a directory(for ubuntu):        
                                                            ls
### See all the file or folder in a directory(for mac):        
                                                            ls
### Make file:                                              
                                                            touch [file name with extension]
### initialize a directory as git directory:          
                                                            git init
### change directory:
                                                            cd [folder name]    
### go back: root directory:                                          
                                                            cd ..


#################################################################################

### Cloning an online repository: 
                                                            git clone [repository URL]
### see what changed in the directory: 
                                                            git status 
#################################################################################
# local working directory to --> stage
### if we want too add all to stage--> good practice--> go to root folder and :
                                                            git add .
### Add from local directory to to git stage (all changes "--all"):
                                                            git add --all
### or 
                                                            add -A
### Add from local directory to to git stage only the contents in the folder we are currently located (all changes "--all"):
                                                            git add .
### Add from local directory to to git stage new changes without deleted changes (all changes "--all"):
                                                            git add *
### Add from local directory to to git stage (only selected files):
                                                            git add [file_name.extension]
### Add from local directory to to git stage (only selected files in a perticular folder):
                                                            git add [folder_name/file_name.extension]
### Add from local directory to to git stage (only specific extension files):
                                                            git add [git add *.extension]
### (undo add) Take back, stage to local directory(all changes "reset"):
                                                            git reset
### after deleting a file if I add, and now if I want to Undo the add and I want to take back the deleted file too then:(need to make hard reset '--hard', this is called: reset with hard flag)
                                                            git reset --hard
#################################################################################
# commit, upload to github 
### Commit or upload all files the changes to github: 
                                                            git commit -m "[comment]"
### (Undo commit) take back, stage to local (all changes "reset"):
                                                            git reset HEAD~

#################################################################################
### delete/ remove a file, and add the changes to stage:( rm = remove)
                                                            git rm [file_name.extension]
### Now if I made any changes and before commiting the change, if I want to delete the file then it ont work by simple rm command
### If I want to delete that file frocefully then I Have to include '-f' flag, which means frocefully remove
                                                            git rm [file_name.ext] -f
### If I want to delete that file and make it staged, but don't want to delete the acctual file from local directory then I need to use a flag '--cached'
                                                            git  rm --cached [file_name.ext]
### remove folder: 
                                                            git rm [folder_name]
### remove folder: recursivly 
                                                            git rm -r [folder_name]   
#################################################################################   
# Brancing 

