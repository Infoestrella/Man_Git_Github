---
title: "Git manual"
author: "Juan Moreno"
date: "2025-01-18"

source: https://www.youtube.com/watch?v=ANF1X42_ae4&list=PLU8oAlHdN5BlyaPFiNQcV0xDqy0eR35aU<

---

# Git manual
Control version software. Open. Save log of changes of files.

## How does it work?

Git takes file snapshots:

1. Name file ```[code0]+"Start"```
2. Change1 -> Rename it ```[code2]+"Comments1"```
3. Change2 -> Rename it ```[code3]+"Comments2"```

We can revert changes and recover previous state of multiple files.

## Branches
Git works with Branches. One per developer?. Each one has its own snapshots.

Finish, Git merge all branches in a final version.

Git detect if both developer has worked in same code.

## Git tool
First install and open **Git bash**.

### ```git init```
When you start proyect. Git create 2 zones:

- **Staging area**: Temp area. We can file status with Git tracking.
- **Local repository**: It stores files snapshots.

### ```git add```
Sintaxis:
>```git add [fileName]```

>```git add .``` (all files in Working folder

Move the file from working directory to Staging area. Git tracks this file.

### ```git commit```
Sintaxis:
>```git commit -m "[myDescription]"```

>```git commit -am "[myDescription]"``` (add + commit at the same time)

Move the file from Staging Area to Local repository.

<table border="1">
<tr>
	<td>Working Directory</td>
	<td><code>-> git add -></code></td>
	<td>Staging Area</td>
	<td><code>-> git commit -></code></td>
	<td>Local Repository</td>
</tr>
</table>

### ```git status -s```
Returns files and folders in working directory. Only files in Sating area and not added.

- ```?? [filename]```: Not tracking
- ```?? [foldername]/```: Not tracking
- ```A [filename]```: Tracking
- ```M (red) [filename]```: Tracking with changes but no backup. It needs ```add```
- ```M (green) [filename]```: Tracking with changes but no backup. Ready for ```commit```

### ```git log --oneline```
Returns versions in Local Repository

### ```git reset --hard```
>Sintaxis: ```git reset --hard [snapshotCode]```

### ```vim```
Sintaxis:
>```git commit --amend``` (open commit in text editor)

## Github
1. Create Repository online
























