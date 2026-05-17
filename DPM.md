# DPM - Dumb Packet Manager

## Project Overview
The DPM project seeks to create an tool which sets up command-line tools automatically for use in workshops, CTF competitions etc. The end result was a downloadable binary which could download tools or apply profiles reliably and reproducibly.

The project was tested on a Debian 13 virtual machine.

### Testing

The installation process was smooth and minimal. I simply curled the file and exported the path.

<img width="872" height="334" alt="image" src="https://github.com/user-attachments/assets/32cac044-d12b-4da5-bfb1-fe89e764028a" />

There were a number of tools as well as some profiles available for download via DPM.

<img width="999" height="547" alt="image" src="https://github.com/user-attachments/assets/5eb2238a-7fa7-4658-8ac1-476ba46b98d2" />

Compared to the "install" -command, the, the DPM tool catalog is compiled into the binary, so DPM resolves installs offline and picks the right package manager per tool automatically.

<img width="1002" height="189" alt="image" src="https://github.com/user-attachments/assets/d06dd2d0-cd02-45a5-a81a-e01552fdb437" />

The more powerful use is applying entire profiles in this fashion.

<img width="1160" height="387" alt="image" src="https://github.com/user-attachments/assets/7fd3f829-c303-41fb-97fc-6942fe44d2c0" />


This profile for an example applied all the tools used in the Beginner CTF event.

In addition to these features, there is also DPM bubble, which acts as a temporary isolated environment and DPM doctor, which diagnoses issues with installations.


### Components
The project consisted of:

- DPM and dpm tui binaries
- YAML catalog tool definitions compiled into the binary
- Inbuilt profiles and community profiles available for download from Github


### Operating Principles

DPM sits above the system package manager. When installing a tool, it consults the built-in catalog to determine the correct install method (apt, pip, cargo, binary download) and applies it. Profiles allow an entire toolkit to be applied in one command, producing the same result on multiple machines.

## Project Review

The project was very easy to use and the instructions were equally straightforward. The website provides all the additional necessary information such as the features and commands. The project has direct use cases in situations where each machine taking part in an event, course etc. needs the exact same setup. This could be used with infra-as-code to setup 20 workstations for an course from a single machine, for an example.

The workings of the project on a binary level are a black box to me, but I didn't come across any issues while testing it. The project also has inbuilt longevity and expansion with community profiles and support for new tool versions.
