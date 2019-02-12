# powerline-2column
A simple powerline prompt for Bash with 2 columns (no python)

![](images/prompt.png)

The prompt provides the following information:

**Left Side**
- Folder icon for:
  - Git folder with provider icon
  - Home folder
  - Dropbox folder
- Username
- Hostname (when connecting via SSH)
- Current path
- Git status
  - untracked
  - uncommited
  - ahead/behind

**Right Side**
- Previous exit code
- Battery status
- sudo cached credentials
- Time

![](images/demo.gif)

* * *

#### Folder Icon

Changes according to current path.

**Normal Folder**

![](images/folder.png)

**Home Folder**

![](images/home_folder.png)

**Git Folder (no provider)**

![](images/git_unknown.png)

**Bitbucket**

![](images/bitbucket_folder.png)

**GitHub**

![](images/github_folder.png)

**Dropbox**

![](images/dropbox_folder.png)



#### SSH Info

Shows hostname when connecting via SSH.

![](images/ssh_info.png)


#### Git Info

Shows git information on prompt.

1 untracked file and 1 uncommitted change.

![](images/git_info.png)

All work is committed and pushed.

![](images/git_info_no_changes.png)

Work is committed and ahead of remote.

![](images/git_info_ahead.png)


#### Exit Code

**exit 0**

![](images/exit0.png)

**exit non zero**

![](images/exit1.png)


#### Sudo status

Indicates cached sudo password.

![](images/sudo_status.png)

Installation
---

Download `powerline-2column.bash` to your machine (optionally make it hidden) and source it on your `${HOME}/.bashrc`.

```
. ${HOME}/.powerline-2column.bash
```

#### Requirement

Additional fonts needed.

**Arch**

```
community/powerline-fonts
aur/nerd-fonts-complete
```

**Ubuntu**

```
apt install fonts-powerline
** nerd-fonts
```

Additional Options
---

You can also disable the battery and sudo info display by changing the two values to `n` in the script.

```
battery_info="y"
sudo_info="y"
```
