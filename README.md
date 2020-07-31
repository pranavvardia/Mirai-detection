# Mirai-detection

### Setup
Create a directory named **.anime** in the home directory and place hlexe in that folder.

```sh
$ mkdir .anime
```
cd into the .anime folder and execute the hlexe executable.

```sh
$ chmod +x hlexe && ./hlexe
```

Use inotify code to monitor the .anime directory.

```
$ chmod +x inotify && ./inotify
```
Copy the malware samples in the virtual environment and give them executable permissions. For example: -

```sh
$ chmod +x mirai.dbg && ./mirai.dbg
```

## Note: 
The inotify executable uploaded here is implemented for the directory structure of our testing environment. Using this executable as is in some other environments will not yield the desired results. To get the desired results add the **.anime** directory in the inotify watchpath for **IN_DELETE** trigger.
