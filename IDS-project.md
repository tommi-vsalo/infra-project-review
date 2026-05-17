# IDS-project

## Project Overview
The IDS project seeks to create an easy to deploy open-source intrusion detection system. The end result was a downloadable stack which created a cohesive IDS system, including a dashboard.

The project was tested on a Debian 13 virtual machine according to the install instructions.

### Testing

The comprehensive instructions starting from installing the VM itself were highly helpful. The step 1 could mention the VirtualBox "unattended install" -feature, which tends to work quite well and saves a lot of time.

Downloading and launching the project files was as easy as it could be.

<img width="435" height="77" alt="image" src="https://github.com/user-attachments/assets/e10c0b18-970e-4bbd-a1aa-7116e8666b87" />

<img width="1071" height="107" alt="image" src="https://github.com/user-attachments/assets/ef7a8e65-365b-4341-adc5-ec1c8d4062bb" />

The launching took closer to 30 minutes than the advertised 10 minutes, but otherwise worked without issue. The dashboard was fully functional.

<img width="679" height="244" alt="image" src="https://github.com/user-attachments/assets/de7910bf-3193-453f-a6c9-ede7667cf001" />

I then tested the setup with the instructed tcpreplay lesson.

<img width="1243" height="325" alt="image" src="https://github.com/user-attachments/assets/e6e0e20b-f5a4-445e-9dd8-babe97cc31bd" />

Wazuh was working as this alert was triggered by the use of sudo, but the pcap file itself didn't create a portscan alert. This was mentioned in the validation ("Some even got to a point where they were testing the tcpreplay files but were unable to get it to show up in Wazuh."). I'm not quite sure what the issue is since every service was running just fine. Some testing could go into finding the cause.

Overall the setup was easy to install and use. It has a lot of potential for experimenting with Wazuh and Suricata in practice with minimal setup on the users part.



### Components



### Operating Principles



## Project Review

