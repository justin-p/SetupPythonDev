# SetupPythonDev

## Installation

0. `sudo apt install curl`
1. Run `curl https://raw.githubusercontent.com/justin-p/SetupPythonDev/main/setup.sh | bash`
2. Enter sudo password.
3. Reboot the system.

## Configure repository

1. Open a bash shell as root and start pycharm-community

![](img/1start_pycharm_in_root_shell.png)

2. Follow the setup and click skip on this page

![](img/2follow_the_setup_skip_remain.png)

3. Click on `get from version control`

![](img/3get_repo.png)

4. Enter the following url `https://github.com/justin-p/impacket`

![](img/4get-repo.png)

5. Wait for `module indexing` and `Updating skeletons` to finish.

![](img/5wait_for_index_to_finish.png)

![](img/6wait_for_index_to_finish.png)

6. Ensure Python 3.8 is selected as the interpreter

![](img/7ensure_python38.png)

7. double click on the file `impacket/smbserver.py` and wait for `Analyzing` to finish.

![](img/8wait_for_analyze.png)

8. Click on `Install requirements`

![](img/9install_requirements.png)

9. Click on `Install`

![](img/10install_requirements.png)

10. Click on `Add Configuration`

![](img/11add_config.png)

11. Click on the plus sign, then `Python`


![](img/12Add_new.png)

12. Set up the configuration as the example below.

![](img/13setup_config.png)

Script path: `/root/PycharmProject/impacket/examples/smbserver.py`

Parameters: `test $PWD -smb2support -debug -spoofed_username USER -spoofed_logon_domain DOMAIN -spoofed_logon_server DC`

Note, update the `-spoofed_` values to match the user you want to spoof.

Working Directory: `/root/PycharmProjects/impacket`

13. Press the green play button to start the script.

![](img/14.png)
