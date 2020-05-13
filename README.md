# Raspberry Pi

## cec-client example to schedule TV on/off times
1. Terminal
```
crontab -e
```

2. Add the following
```
# Turn TV on 6am M-F
0 06 * * 1-5 echo 'on 0' | /usr/bin/cec-client -s -d 1

# Turn TV off 3pm M-F
0 15 * * 1-5 echo 'standby 0' | /usr/bin/cec-client -s -d 1
```

## Updating and upgrading Pi
```
sudo apt update
sudo apt full-upgrade
```

