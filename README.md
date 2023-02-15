# CHEM 120 E-Textbook

## About
The project contains a game to quiz about the understanding of isomers in organic chemistry for students of CHEM 120 at DePauw University.

## Setting up
1. Installation
  + Download the appropriate version of [VSCode](https://code.visualstudio.com/download) for your operating system.
  + (**For MacOS**) Install `Homebrew` and use it to install `npm` and `nvm`.
  + (**For Window**) Install `nodejs`and add it to path.
  + (**For Linux**) Install `npm` and `nvm` from terminal.
  
2. Add the [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) extension to `Visual Studio Code` for debugging.

3. Set up the SSH key on your computer
  
  - Follow steps 1-4 of the instruction to [Generate a new SSH key](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent#generating-a-new-ssh-key)
  - Follow steps 1-9 of the instruction to [Add a new SSH key to your GitHub account](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent#generating-a-new-ssh-key)

4. Fork the repo to your GitHub account (click `Fork` on the top right of the screen)
![image](https://user-images.githubusercontent.com/71036845/205376704-712cf395-3bbf-497c-abca-05d0e5137dda.png)

5. Clone the repo to your local computer

        git clone git@github.com:<your-username>/chem120-game.git
        cd chem120-e-textbook
        git remote add upstream git@github.com:anhphuongdo34/chem120-game.git
        git remote set-url --push upstream DO_NOT_PUSH
        
## For Jeff
To **updates the changes** made by students on your local computer

        git pull
        
To **send your changes** to GitHub so the students can use them

        git push


## Contribution
(replace anything with the `<>` with your own content)

1. Before making any changes run `git fetch upstream` then `git rebase upstream/master`. The make changes in the code on the `master` branch

2. Create a new branch. If the changes associate with a specific `issue`, name the branch after the number of the issue.

        git checkout -b <new_branch_name>

3. Pull all the updates from upstream before commit new changes

        git stash
        git fetch upstream
        git rebase upstream/master

4. Add, commit, and push the changes

        git stash apply
        
Might need to resolve merge conflicts. Follow the instruction on the terminal.

        git add .
        git commit -m "<a short description of the changes>"
        git push origin <branch_name>

5. Make a Pull Request (PR) on GitHub.

## Acknowledgement
- This project uses ChemDoodle Web Components. The link to [web.ChemDoodle.com](https://web.chemdoodle.com/) and/or [www.ChemDoodle.com](https://www.ChemDoodle.com).
- Thank you Dr. Jeff Hansen, Professor of Chemistry and Biochemistry at DePauw University, for designing the game for the introductory Chemistry courses.
