# Sysadmin-Cheatsheat
Some commands to use in no particular order after getting access to a dedicated server to benchmark/stress test before fit for use.

```lspci```  
  
```dmidecode```  

```lsblk```  
```smartctl -a /dev/sda```  
```smartctl -a /dev/sda | Pwr```  
  
```smartctl -a /dev/sda -d megaraid,00```  
accessing SAS disks behind Dell RAID controller  
  
```smartctl -a /dev/sg0```  
some HP RAID Controllers```  
  
```screen -dmS stress stress-ng --cpu 10 --vm 1 --vm-bytes 32G```  
  
```ipmitool sensor```  
```ipmitool sensor | grep Fan```  
```sensors```  

```wget https://proof.ovh.net/files/10Gb.dat -O /dev/null```  
  
```speedtest```  
```speedtest -s 24215```  
  
```wget http://speedtest-lon1.digitalocean.com/5gb.test -O /dev/null```  
