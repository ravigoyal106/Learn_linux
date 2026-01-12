## `timedatectl`
#### with the help of `timedatectl` command you can chenge the timezone of your linux server.
```
timedatectl status                 # Check current timezone of the System

timedatectl list-timezones           # List all time Zones

sudo timedatectl set-timezone Asia/Kolkata # Change timezone to Asia/Kolkata

sudo timedatectl set-time 'YYYY-MM-DD HH:MM:SS' # set time 
```
- Enable Auto time sync

```
 sudo timedatectl set-ntp true   # Set auto sync time using NTP(network time protocol) synchronization.

 sudo timedatectl set-ntp false
 ```
### Real-world Problems and Solutions using `timedatectl`
 P1. A newly provisioned server shows logs in the wrong timezone (e.g., UTC instead of IST), confusing developers.
 ```

sudo timedatectl set-timezone Asia/Kolkata  # Set timezone to Asia/Kolkata
```
P2. The System clock is out of sync.
```

sudo timedatectl set-ntp true # Enable NTP Synchronization
```
P3. An admin manually changed the system time, causing monitoring tools to misalign with actual events.
```
sudo timedatectl set-time '2026-01-12 01:52:00' # set correct time

sudo timedatectl set-ntp true # Enable NTP Synchronization
```
P4. In a distributed system, logs appear out of sequence because nodes are in different timezones.
```
sudo timedatectl set-timezone UTC # Standardize all nodes to UTC

timedatectl status # Check Status
