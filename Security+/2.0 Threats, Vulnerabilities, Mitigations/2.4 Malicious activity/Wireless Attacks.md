## Wireless deauthentication
- A [[Denial of Service|DoS]] attack that continuously disconnects a user from the wireless network
- Takes advantage of [[Introduction to WLAN (802.11)|802.11]] management frames as they are sent in clear text with no authentication or validation (pre 802.11ac)
- 802.11ac has been updated to encrypt only "important" management frames
## Radio frequency (RF) jamming
- A [[Denial of Service|DoS]] attack to prevent multiple devices' from communicating on a wireless network by transmitting noise to the network, making legitimate devices unable to get a good signal to connect to
- Can be unintentional, caused by microwaves or fluorescent lights
#### Wireless jamming
- Sending constant, random bits / constant, legitimate frames
- Data sent at random times - random data and legitimate frames
- **Reactive jamming** - jamming signals are only sent when someone tries to communicate
- **Fox hunting** - determining the source of the jamming signal
## Bluetooth attacks
#### Bluesnarfing
- An attacker gains unauthorized access to information on a Bluetooth-enabled device
- Occurs when a device's Bluetooth connection is left unsecured
#### Bluejacking
- An attacker sends unsolicited messages ("jacks") to nearby Bluetooth enabled devices
- These messages can be sent to a device's Bluetooth address, appearing as a contact or text message
- Used to annoy or spam victims; does not steal data
## Evil twin
- An attacker sets up a rogue access point that mimics a legitimate network
- Users connect to this fake access point, because it may have a similar SSID (network name) to the legitimate one
- The attack can intercept sensitive data with this rogue AP