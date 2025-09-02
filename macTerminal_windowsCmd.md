# MacTerminal / Windows Cmd

#### Create new directory

    - mkdir [folderName]

#### Open Directory

    - cd [folderName]
    - cd [folderName]/[anotherFolderName]
    - cd [path]

#### Goto previous directory

    - Win: cd ..

#### Goto root directory

    - Win: cd ~

#### To get previous executed command

    - Mac: up and down arrow keys
    - Win: up and down arrow keys

#### Open specific Drive (Below eg. of D drive)

    - Win: cd D:
           d:

#### clear terminal

    - Mac: clear
           command + K

#### List all files and folders

    - Mac: ls
    - Win: dir or ls

#### List all files including hidden

    - Mac: ls -a
    - Win: ls -a

#### List all files with extra details

    - mac: ls -la
    - Win: ls -la

#### List all files folders including permissions

    - Mac: ls -l

#### Move 2 levels back

    - Cd . - ./..
    - Win: cd ../..

#### Create files

    - Mac: touch [fileName]
    - Win: edit [fileName]

#### Create multiple files

    - Mac: touch [fileName] [fileName2] ….
    - Win: edit [fileName] [fileName2] ….

#### multiple commands using semicolon

    - Mac: mkdir [folderName]; touch [folderName]/[filename]

#### Open files

    - Mac: open [fileName]

#### Deleting files

    - Mac: rm [fileName]
    - Win: del [fileName]

#### Deleting multiple files

    - Mac: rm fileName fileName2 …
    - Win: del fileName fileName2 ….

#### Deleting all files

    - Mac: rm \*

#### Move files

    - Mac: mv fileName path(mv mapty.js - ../)

#### Move multiple files

    - Mac: mv fileName path(mv mapty.js - ../)

#### Delete Directory

    - Mac: rm -r [directoryName]

#### Delete empty directory

    - Mac: rmdir folder - Name

#### Delete directory and all files within

    - Mac: rm -R folde - rName

#### To set permission

    - sudo chown -R $USER /Users/visheshparab/Desktop/Projects/JavaScript/complete-javascript-course-master/17-Modern-JS-Modules-Tooling/starter/node_modules

#### Display information about the machine’s hardware architecture.

    - Mac: uname -m

#### Check started services

    - Win: net start

#### prints entire path till current location

    - Mac: pwd

#### Read Write full Permissions

    - Mac: sudo chmod 777 [path or fileName/folderName]

#### Move cursor fast through command to edit

    - Mac: option + leftArrow/RightArrow

#### Clear typed command

    - Mac: control + U

#### Move cursor to start of the command

    - Mac: control + A

#### Move cursor to end of the command

    - Mac: control + E

#### check which ports are open

    - Mac: lsof -i -P -n | grep LISTEN
    - Win: netstat -ano | findstr "LISTENING"

#### Rename file

    - Mac: mv [oldFileName] [newFileName]
    - Win: ren [oldFileName] [newFileName]

#### Rename Folder

    - Mac: mv [oldFolderName] [newFolderName]
    - Win: ren [oldFolderName] [newFolderName]
