# Network-Scanning-Nmap-Network-Mapper
# **Vulnerability Scanning with Nmap**

**Nmap ("Network Mapper")** is an open-source tool for network exploration and security auditing. It quickly scans large networks but also works on single hosts. Nmap uses raw IP packets to identify available hosts, the services they offer (including versions), their operating systems, and their security measures. While mainly used for security audits, it is also helpful for network inventory, service upgrade management, and monitoring uptime.

## 1 Verify the **Installation and Version** of Nmap.

Double-click on the **Terminal Icon** to open the **Terminal Window**.

Enter **nmap --version** in the **Terminal Window** and press Enter

Observe: **Nmap version 7.80**| Observe **Platform: x86\_64-pc-linux-gnu**

The _correct version is important_ for compatibility, running scripts, plug-ins, or features.

Enter **clear** to erase the screen.

## 2 Access the **Help Feature and Man Page** for Nmap.

Enter **nmap --help** and press Enter. You can the same results when you enter **nmap**.

Observe: The **Nmap manual |** Observe: **EXAMPLES** at the bottom of the screen

Observe the bottom of the screen. You can press **h for help** or press **q to quit**.

Enter **clear** to erase the screen.

## 3 Run a **Basic Nmap Scan on a Target**.

Enter **nmap** and then go to the TARGET SPECIFICATION area

Enter **nmap scanme.nmap.org** Observe the output.

Press the up-arrow **key two times**. Observe that your last command appears. Add **/30** to the command

This **/30 cider block** specifies the network is 30 bits long and leaving only two bits for the host.

Enter **nmap scanme.nmap.org/30**. Observe both the top and bottom of the output.

Enter **clear** to erase the screen.

## 4 Run an **Nmap scan on an Authorized Target** and Reference the Man Page as needed.

Enter **ifconfig** to locate IP Address. Copy and Paste IP Address

Enter **nmap 172.18.X.XX** to scan. Observer output for open ports.

## 5 Run an **Nmap scan using Options** from the Man Page.

Enter **man nmap** and then go to Example 1. A representative Nmap scan.

Copy and paste **-A -T4 scanme.nmap.org** on the command line and press Enter.

\*\*Scan failed\*\* revisit later.

## 6 Output Nmap scan results to a File.

Enter **nmap -p 80 -A -oN scan.txt scanme.nmap.org/30**. Observe scan, commands, and switches.

Enter **ls** to list files. Observe **scan.txt**. Enter **cat scan.txt** to show the content of the file.

##7 Run a Customized Scan on a Target.

Perform a nmap scan, scanning **ports 22-80**, on target: **scanme.nmap.org**

Use the appropriate option to **enable OS and version detection, script scanning, and traceroute**. -A

Set your scan to **-T3** for the **timing execution** of the scan.

Output the scan results to a txt file named: output.txt

**Verify** the contents of the output.txt file

Be sure to reference your nmap man page for help.

Enter **nmap -p 22-80 -A -T3 -oN output.txt scanme.nmap.org**

Enter **ls** to list the files. The file is output.txt

Enter **cat output.txt** to show file content.
