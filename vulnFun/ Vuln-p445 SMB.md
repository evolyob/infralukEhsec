SMB CIFS
```php
TCP Ports

139    ( NetBIOS Session Service )
445    ( Microsoft-DS )
UDP Ports

137    ( NetBIOS Name Service )
138    ( NetBIOS Name Service )
#locate smb.conf
#emum4linux <target>

Mount shares
mount -t cifs -o user=USERNAME,sec=ntlm,dir_mode=0077 "//10.10.10.10/My Share" /mnt/cifs
mount shares 2
sudo apt-get install cifs-utils
mkdir /mnt/Replication
mount -t cifs //10.10.10.100/Replication /mnt/Replication -o
username=<username>,password=<password>,domain=active.htb
grep -R password /mnt/Replication/
```