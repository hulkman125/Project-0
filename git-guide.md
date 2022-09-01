                                                                        Command Line git

	Clone

        Creates a copy of a repository that already currently exists into a new directory.

        Creates and multiple remote-tracking branches for each individual branch in the cloned repository.

        Git clone file1 file2   //To make a clone of the repository at <file1> into the folder called <file2>:


    Add

        Adds new or unchanged files in your working directory to the Git staging area.

        Updates the index using the current content found in the working tree.

            Adds the current content of existing paths as a whole

        Git add  text.txt   //To copy a text.txt file



    Rm

        Removes files from the index or from the working tree.

        Git rm  file.txt  // To remove a file named text.txt

 

    Commit

        Creates a new commit that contains the current contents of the index and the given log message describing the changes. 

        Used to save your changes to the local storage location.   

        Git commit -a    //Tells the command to automatically stage files that have been modified and deleted but new files you have not told Git about are unaffected.

        Git commit -p   // Use the interactive patch selection interface to chose which changes to commit.

        Git commit -C commit   //Take an existing commit object, and reuse the log message and the authorship info when creating the commit.


    Push 
  
        Updates remote Resilient File System (refs) using local refs, while sending objects needed to finish the given refs.

        Git push -f  // Force a push that would otherwise be blocked

        Git push -u origin [branch]   // creates an upstream tracking branch with a lasting relationship to your local branch.

        Git push –tags   // Publish tags that aren’t yet in the remote repository


   

    Fetch

        Branches and/or tags refs from one or more other digital storage locations, along with other data needed to finish their histories.

            Any tag that points to the histories being fetched is also fetched.

        Git fetch -all   // fetch all remotes

        Git fetch -append   // appends to existing fetched contents without overwriting

        Git fetch -tags   // fetch all tags from a remote


   

    Merge

        Combines 2 or more development histories together

        Incorporates changes from one data storage and merge changes into another

        Git merge b1  // To merge the current branch “master” to one called b1

 

    Pull

        Grabs from and integrate with another data storage or a local branch

        Incorporates changes from a remote data storage into the branch currently being used.

            If the current branch is behind the remote, then it will (by default) fast forward the current branch to match the remote.

        Git pull remote   // To grab the remote copy of the current branch and instantly merge it onto the local copy


  


    Branch

        List creates or deletes branches

        Git branch –list  // To list all the branches in your repository



    Checkout

        Switch branches or restore working tree files

        Updates files in the working tree to match the version in the index or the specified tree.

        Git branch  // To find out what branches are available and  to find out the name of the current branch is

        Git checkout -b Z1  // To create and check out a new branch called Z1





                                    .git files and folders
    Git folder

        Contains all the information required for version control. Can be used to clone your repo

        4 subdirectories include:

            Hooks/              :example scripts

            Info/                  : exclude file for ignored patterns

            Objects/             :all “objects”

            Refs/                   :pointers to commit objects


        4 files include:

            HEAD                   : current branch

            Config                 :configuration options

            Description

            Index                   :staging area


        Here “object” includes:

            Blobs(files)

            Trees(directories)

            Commits(reference to a tree, parent commit,etc)
        

    Gitignore file

        A plain text file where each line contains a pattern for files and directories to ignore.

        You can tell Git to ignore only a single file or a sildle folder by mentioning the name or pattern of that specific file or folder.

        Placed in the root folder of the repository 


                                                GitHub

    Pull requests

        Lets you tell others about changes you have pushed into a branch in a repository on Github.

        You can then discuss and review the potential changes with others and follow-up commits before your changes are merged into the base branch.

    SSH authentication to repositories

        Provides cryptographic strength that is normally difficult to obtain otherwise. 

            Public key authentication improves greatly at it frees the user from having to remember passwords that are normally complicated.

        Also offers usability benefits

            Allows the user to implement single sign-on across the SSH servers they connect to

            Allows automated login that does not require a password that is a key enabler for the countless secure automation processes that function within enterprise networks globally.


                                                Resources
    Pro Git Book

        A manual that builds on the hugely original edition that instructs the reader about the software of both Git and GitHub

            Written by Scott Chacon and Ben Straub
