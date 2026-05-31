# Task 1: Scan Your Local Network for Open Ports

## Objective

To discover open ports on devices in my local network and understand network exposure using Nmap.

## Tools Used

* Nmap
* Command Prompt (Windows)

## Local Network Range

* IPv4 Address: 192.168.29.6
* Subnet Mask: 255.255.255.0
* Network Range: 192.168.29.0/24

## Command Used

nmap -sS 192.168.29.0/24

## Scan Results

| IP Address     | Open Ports                          | Services                  |
| -------------- | ----------------------------------- | ------------------------- |
| 192.168.29.1   | 53, 80, 443, 1900, 7443, 8080, 8443 | DNS, HTTP, HTTPS, UPnP    |
| 192.168.29.238 | 2869                                | ICSLAP                    |
| 192.168.29.6   | 135, 139, 445, 2968                 | MSRPC, NetBIOS, SMB, ENPP |

## Potential Security Risks

* Open ports may expose services to unauthorized access.
* UPnP can be risky if improperly configured.
* SMB (Port 445) has been targeted by malware in the past.
* Unnecessary services should be disabled when not required.

## Conclusion

Using Nmap, I successfully scanned my local network and identified active hosts along with their open ports. This task helped me understand network reconnaissance, TCP SYN scanning, and potential security risks associated with exposed network services.
