# Tunneling Tools And Commands

## Sshuttle
[SSH Tunneling Tool] (https://github.com/sshuttle/sshuttle)

###Attacker machine:
kali@kali:~$ sudo sshuttle -e "ssh -oHostKeyAlgorithms=+ssh-dss" -r vyos@172.16.45.205 10.0.0.0/24

Then try nc to a port or nmap or the tool you need against the network you want to reach
