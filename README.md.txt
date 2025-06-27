Task 4 – Setup and Use a Firewall on Windows

Objective :
To configure and test basic Windows Firewall rules to allow or block traffic on specific ports and understand how firewall filtering works.



Tools Used :
- Operating System: Windows 10
- Firewall Tool: Windows Defender Firewall with Advanced Security
- Telnet Client: Enabled via Windows Features to test blocking on Port 23
- Command Prompt (cmd): Used to test firewall rules



Steps Performed :

1. Open Windows Firewall with Advanced Security.
- Accessed via "Start > Windows Defender Firewall with Advanced Security".


2. Listed Current Firewall Rules
- Explored "Inbound" and "Outbound Rules" tabs.


3. Created New Inbound Rule to Block Port 23 (Telnet)
- Navigated to "Inbound Rules > New Rule > Port > TCP > 23".
- Selected "Block the connection".
- Applied to all profiles and named it "Block Telnet".


4. Enabled Telnet Client on Windows
- Used "Control Panel > Programs > Turn Windows features on or off".
- Checked "Telnet Client" box.


5. Tested Rule by Running Telnet on Port 23
- Ran "telnet localhost 23" in Command Prompt
- Connection was "blocked", confirming rule works


6. Added Inbound Rule to Allow Port 22 (SSH)
- Followed same steps but selected "Allow the connection" for "Port 22".


7. Deleted the Block Rule for Telnet (Restored Original State)
- Right-clicked "Block Telnet" rule and chose "Delete".


Summary:

This task demonstrated how to configure and test firewall rules using Windows Defender Firewall. I successfully:
- Blocked inbound traffic on Telnet port (23).
- Allowed SSH port (22).
- Verified rule behavior using Telnet command.
- Removed the rules to restore original settings.

These steps highlight the importance of managing network traffic securely and how basic firewall configurations can prevent unauthorized access.



Outcome :
- Gained hands-on experience in setting up basic firewall rules.
- Learned how firewall filters traffic based on ports and protocols.