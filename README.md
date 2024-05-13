# SOC-Home-Lab
# Installed Ubuntu VM 1
# SOC-Home-Lab
The purpose of this project is to host a basic SOC environment locally.

This project contains the steps to configure a SOC environment locally on your home computer using Virtual Machines and some basic networking concepts. We will make use of the following services:
  1. Virtualbox along with Virtual machines Including Ubuntu, Windows-10, Kali-Linux
  2. Wazuh Siem
  3. Shuffle
  4. Mimikatz (Malware)
  5. Sysmon (For Windows)
  6. VirusTotal
  7. Discord
  8. Hydra (Script in Kali)


In summary, we will achieve the following:

A. Phase 1:
  1. Detect threats on our Windows virtual machine with Wazuh SIEM
  2. Forwarding the detected threat to shuffle for enrichment
  3. Automatically forwarding an alert message to a Discord server for specific threats
     
B. Phase 2:
  1. Detecting threats on our Ubuntu virtual machine with Wazuh SIEM
  2. Simulating a SSH brurte force attack on our Ubuntu machine using a Kali Virtual machine as our attackbox
  3. Mitigating the adversity of the SSH brute force attack using "active response" capability of Wazuh SIEM


# Windows VM
1. We Installed Mimikatz on the Windows VM and a Wazuh Agent
2. We Configured Sysmon to send Logs to the Wazuh SIEM
![Windows Mimikatz](https://github.com/dicedealer/SOC-Home-Lab/assets/74645710/a1d7bac8-ec25-46c3-bdb7-1b0138161e98)
![Discord Message](https://github.com/dicedealer/SOC-Home-Lab/assets/74645710/7db70f29-5fa2-4d66-852b-9c66ba5ecb9d)
![Mimikatz Detected](https://github.com/dicedealer/SOC-Home-Lab/assets/74645710/3edf1569-b17e-43e0-a621-3c7c510145c3)
![Shuffle Workflow](https://github.com/dicedealer/SOC-Home-Lab/assets/74645710/d160170e-5676-448e-93db-e30c6cdea9e1)
