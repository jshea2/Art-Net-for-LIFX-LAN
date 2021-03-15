# Art-Net-for-LIFX-LAN
### Standalone App that Converts [Art-Net](https://art-net.org.uk/) Data into RGB Values for LIFX Bulbs on your Local Network
#

<img width="170" alt="Screen Shot 2021-03-14 at 6 36 51 PM" src="https://user-images.githubusercontent.com/70780576/111092794-4e91d980-84f4-11eb-92b0-e97d077766ba.png">


<img width="370" alt="Screen Shot 2021-03-14 at 6 36 51 PM" src="https://user-images.githubusercontent.com/70780576/111093928-556e1b80-84f7-11eb-9338-96ddf4b8ef7b.gif">

#
## [Download Now](https://github.com/jshea2/Art-Net-for-LIFX-LAN/releases/)

Requires: Any [LIFX Color Bulb](https://www.lifx.com/pages/lightbulbs) & Any [Art-Net Software](http://dmxking.com/m/support/13-control-software/80-artnet-sacn-software)
## Setting Up Physical LIFX Bulbs
 - Install LIFX Bulbs and Connect to WIFI (Only works on 2.4Ghz, not 5G)
   - If you're having trouble connecting refer to [LIFX Troubleshooting Website](https://support.lifx.com/hc/en-us/categories/200238164-Set-Up-Troubleshooting)
 - DO NOT name/label your lights as just a number, because it will show up blank
    - *Example:* naming your bulb "1A" or "A 1" is OK, but naming it just "1" or "23" will NOT work

## Setting Up *'Art-Net for LIFX' App*'


<img width="317" alt="Screen Shot 2021-03-14 at 6 36 51 PM" src="https://user-images.githubusercontent.com/70780576/111092799-55b8e780-84f4-11eb-9461-d1194683fd98.png">



- Click "Get LIFX Bulbs"
   - This will open the "DevTools" window and if connected will log all available LIFX Bulbs on your Local Network.
   - If you do not see this make sure it's on the **"Console"** tab, not "Elements"
   - You'll also notice a drop-down list of populated available LIFX bulbs 
- Now to "Patch" these bulbs to our Art-Net universe
   - Select LIFX bulb from drop-down list and input starting "Address"
   - Click "Patch/Add LIFX Bulb" button
   - This will patch and also log below
      - You can also patch **more than one** bulb to the **same** address for grouping multiple LIFX bulbs to one patched fixture in your lighting software
    - "Auto-Patch" takes all available LIFX bulbs and patches them in alphebetical order 
- Input your Art-Net's "Subnet, Universe, and Net" ([0, 0, 0] is usually the default)
- Click "Start" and send some Art-Net!

## Patching External Art-Net Software
- ETC Nomad & QLab Settings Example:
<img width="400" alt="Screen Shot 2021-01-29 at 11 37 29 PM" src="https://user-images.githubusercontent.com/70780576/106350597-33904080-628b-11eb-9760-5746e11c9f48.png">

<img width="400" alt="Screen Shot 2021-01-29 at 11 36 50 PM" src="https://user-images.githubusercontent.com/70780576/106350632-6c301a00-628b-11eb-8a9e-66f25e18bc37.png">
 
- Each LIFX Bulb is set up to be a 3-channel fixture (Red, Green, Blue)
   - You can use generic 3-channel RGB profiles to patch
   - *Fun Fact:* The Free version of QLab lets you do 16-channels, so you can control 5 LIFX fixtures separately

## Acknowledgements
- Inspired by: [lifxe131](https://github.com/cpuchip/lifxe131/blob/master/e131_receive.py)
- npm library: [dmxnet](https://www.npmjs.com/package/dmxnet)
- npm library: [node-lifx-lan](https://www.npmjs.com/package/node-lifx-lan)
- and a special thanks to Lightsteed for beta testing

## Notes:

### This Application is for the LAN API. For the HTTP API check out [Art-Net for LIFX-HTTP](https://github.com/jshea2/Art-Net-for-LIFX-HTTP)


- Other features not available, but currently in the works:
   - Deleting "Patched" Bulbs

## Support:
Join the Discord server Community: 

<a href="https://discord.gg/FJ79AKPgSk">
        <img src="https://img.shields.io/discord/308323056592486420?logo=discord"
            alt="chat on Discord"></a>

## [Download "Art-Net for LIFX-LAN" Now](https://github.com/jshea2/Art-Net-for-LIFX-LAN/releases/)
