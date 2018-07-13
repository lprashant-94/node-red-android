

#Tools:
- Termux - Terminal emulator to run node red 
- Node-Red - Flow based programming for IOT devices
- Termux-api - Gives command to get hardware information of android device. Need to install its app and apt package both.
- Hacker's Keyboard - for using alt, ctrl keys on termux
- Autostart - Android app to boot termux on restart as well.


Useful link - 
https://nodered.org/docs/platforms/android

```
apt update
apt upgrade
apt install coreutils nano nodejs termux-api
npm i -g --unsafe-perm node-red
node-red
```

##Steps
1) Install termux, termux-api, autostart.
2) Run above commands, last command start node-red.
3) At this point node-red server will be running on your mobile. Its configuration page can be opened from IP:1880. Now start configuring device using flow language. battery-status.json file contains configuration.

## Visualisations
![Current Values](Current_Values.png?raw=true 'Current Values')
![Trend](Trend.png?raw=true 'Trend')

## Next steps
- Calculate moving derivatives of battery percentage and temperature.
- Calculate charging time and discharging time.
- Find trends in charging.
- Analyse charging trends and Predict charging time, discharge time. Find insight.
- Add instructions for switching to power saving mode in night and in events when its use is minimal. Use temperature parameter to detect usage.
- Add instructions to take actions when temperature goes high.
- Test if restart correctly start node red and termux or not. Also check if terminating termux, terminates nodered session or not...


