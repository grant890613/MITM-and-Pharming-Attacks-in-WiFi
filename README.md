# MITM-and-Pharming-Attacks-in-WiFi

## Redirect Victim’s traffic to Attacker
1. MITM attack: split the encrypted sessions
2. Pharming attack: redirect HTTP requests to a phishing web page

## MITM
1. Obtain all other client devices’ IP/MAC addresses in a connected WiFi network
2. ARP spoofing for all other client devices in the WiFi network
3. Split SSL/TLS encrypted sessions and get the inputted username/password strings from HTTPS sessions

## Pharming attack
1. Obtain all other client devices’ IP/MAC addresses in a connected Wi Fi network
2. DNS spoofing attack for web services

## Solution
1. Use static ARP⁠: The ARP protocol lets us define a static ARP entry for an IP address, and prevent devices from listening on ARP responses for that address. For example, if a workstation always connects to the same router, we can define a static ARP entry for that router, preventing an attack.
2. Use packet filtering⁠: Packet filtering solutions can identify poisoned ARP packets by seeing that they contain conflicting source information, and stop them before reaching devices on our network.
3. Use VPN⁠: VPN allows devices to connect to the Internet through an encrypted tunnel. This makes all communication encrypted, and worthless for the ARP spoofing attacker.
