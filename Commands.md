# Tunneling Tools And Commands

## Sshuttle
[SSH Tunneling Tool] (https://github.com/sshuttle/sshuttle)

### Attacker machine:

kali@kali:~$ sudo sshuttle -e "ssh -oHostKeyAlgorithms=+ssh-dss" -r vyos@172.16.45.205 10.0.0.0/24

Then try nc to a port or nmap or the tool you need against the network you want to reach

## OpenSSH
(https://www.openssh.com/)

### Attacker machine:

kali@kali:~$ sudo ssh vyos@172.16.45.205 -p22  -oHostKeyAlgorithms=+ssh-dss -D 127.0.0.1:9050

Then use proxychains to use the tunnel against the victim; 

Example command:

$sudo proxychains impacket-psexec administrator@10.0.0.100

## Chisel

(https://github.com/jpillora/chisel)
