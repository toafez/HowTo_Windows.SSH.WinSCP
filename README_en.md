[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Ftoafez%2FHowTo_Windows.SSH.WinSCP&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://hits.seeyoufarm.com)

# HowTo: SSH key with WinSCP for Windows

## What is this about?
The following instructions are based on my [HowTo: SSH key with PuTTY and PuTTYgen](https://github.com/toafez/HowTo_Windows.SSH.PuTTY.PuTTYgen/blob/main/README_en.md), which already described password-free SSH public key authentication from a local Linux system to a remote Linux server. **By integrating the **private key already generated with PuTTYgen into the Windows program WinSCP, **password-free access to a remote Linux server can also be achieved here.

## Install WinSCP
WinSCP can be downloaded as a Windows installer from the [WinSCP download page](https://winscp.net/eng/download.php).

## Open WinSCP
1. Launch **WinSCP** from the Windows programs list.
2. In the **Session / Transfer Protocol** section on the left, select **SCP** from the drop down menu.
3. In the **Session/Host name** and **Port number** sections, enter the IP address of the remote server you wish to connect to and, if necessary, adjust the port to be used. In this example, the IP address 172.16.1.12 and port 22 are used.
4. In the **Session / User name** section, enter the user name with which you wish to log on to the remote server. In this example the superuser **root** is used.
5. click on the **Advanced** button

    ![01_WinSCP_Configuration](/images/01_WinSCP_Configuration_en.png)

6. Select **SSH / Authentication** in the right pane and then click on the yellow marked button in the right pane **Authentication parameters / Private key file:** to search the file system for the private key that you have already created according to my instructions [HowTo: SSH-Key with PuTTY and PuTTYgen](https://github.com/toafez/HowTo_Windows.SSH.PuTTY.PuTTYgen/blob/main/README_en.md) and saved in a safe place.

    ![02_WinSCP_Configuration](/images/02_WinSCP_Configuration_en.png)

7. Select the appropriate file and click **Open**.

    ![03_WinSCP_Configuration](/images/03_WinSCP_Configuration_en.png)

8. The path including the filename should now be displayed in the yellow highlighted text box. Click the **OK** button to return to the WinSCP login page.

    ![04_WinSCP_Configuration](/images/04_WinSCP_Configuration_en.png)

9. Save your entries by clicking the **Save* button.

    ![05_WinSCP_Configuration](/images/05_WinSCP_Configuration_en.png)

10. Enter any name in **Site name:** or use the default name. Click **OK** to save the session.

    ![06_WinSCP_Configuration](/images/06_WinSCP_Configuration_en.png)

11. You can now select your saved connection destination on the left to connect to your remote server. To do this, click on the **Login** button.

    ![07_WinSCP_Configuration](/images/07_WinSCP_Configuration_en.png)



