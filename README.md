# Server-Checklist
Some commands to use in no particular order after getting access to a dedicated server to benchmark/stress test before marking it fit for my use.

## Dedicated Server specific commands
The following commands will make much more sense and give appropriate results when ran on a dedicated server. They are to essentially check or benchmark some specific hardware information in a dedicated server. 
Those who are using VPS or Cloud environments need not do this. You can skip to the VPS section.

```lspci```  
  
```dmidecode```  

```lsblk```  
```smartctl -a /dev/sda```  
```smartctl -a /dev/sda | Pwr```  
  
```smartctl -a /dev/sda -d megaraid,00```  
accessing SAS disks behind Dell RAID controller  
  
```smartctl -a /dev/sg0```  
some HP RAID Controllers
  
```screen -dmS stress stress-ng --cpu 10 --vm 1 --vm-bytes 32G```  
  
```ipmitool sensor```  
```ipmitool sensor | grep Fan```  
```sensors```  

```wget https://proof.ovh.net/files/10Gb.dat -O /dev/null```  
  
```speedtest```  
```speedtest -s 24215```  
  
```wget http://speedtest-lon1.digitalocean.com/5gb.test -O /dev/null```  

## Dedi + VPS commands
The following commands can be ran on a VPS as well as a dedicated server. They are for checking general compute performance.

## Misc Commands

### How to upgrade Debian 11 to 12
```
sed -i 's/bullseye/bookworm/g' /etc/apt/sources.list
apt-get update
apt-get upgrade -y
```
