# Network-Based Threats and Mitigations

## Concepts Learned

### How Data Moves Around a Network

A network exists when you have two or more devices that share data. As you saw in the previous unit, a network is composed of many different physical parts that work together to ensure your data gets to where it's needed. This transmission of data across a network is enabled by a suite of communication protocols, often referred to as TCP/IP. It's named after the two main protocols: Transmission Control Protocol (TCP), which handles the connection between two devices, and Internet Protocol (IP), which is responsible for routing information across the network.

Every network on the planet shares and moves data every second of the day. This data comes in every shape and size, from a simple message to images, and even the movies that are streamed to your home.

#### The datagram or packet
Networks exist to help make device-to-device or system-to-system communication easier. Whatever the size of data, it all needs to be broken down into tiny, uniform chunks. These chunks are called datagrams but are also more commonly known as packets.

Imagine that you want to stream a movie to your device. Given the enormous size of the data involved, the streaming server can't give you the whole movie in one go. Instead, the movie is broken up into billions of packets. Each packet contains a small part of the movie, which is then sent to your device. Your device has to wait until enough packets have been received before you can start watching the movie. In the background, the server continues to send a steady stream of packets to your device just ahead of what's being displayed. If your network speed slows down, then the packets may not reach you in time. The picture you see might become distorted or blocky and there may be gaps in the sound.

#### IP addresses
When you want to send a letter to a friend, you'll first write it out before putting it in an envelope. Next you'll write your friend's address on the envelope before posting it. The postal service collects the letter, and through various sorting offices, eventually delivers it.

Networks operate in a similar manner. The message is contained in the packet, like an envelope. Then the sender and recipient addresses are added to the packet.

The primary function of the Internet Protocol (IP) is to ensure that every device on a network can be uniquely identified. Before a packet is sent across the network, it must be told the IP address of where it's going, and the IP address of where it's come from.

There are presently two standards of IP address: the IPv4 and the IPv6. The details are beyond the scope of this module, but the most common type of IP address, and the one you may be familiar with, is IPv4. This is made up of four groups of digits separated by a dot, for example: 127.100.0.1.

#### DNS
Just like every device on a network needs a unique IP address, every public facing website has its own IP address. You could use the IP address to visit your favorite online retail store, bank, or streaming video service. But with so many websites available, that would be difficult to remember. Instead, you type the name of the service you're looking for into your browser and it takes you to the website you want. This is all thanks to the domain name service or DNS.

The DNS holds a table that has the name of the website, for instance microsoft.com, which maps to its corresponding IP address. Your browser uses this to find the actual website in much the same way as you might use a phone book to find a telephone number.

Diagram that shows a simplified representation of a DNS lookup table, where the domain microsoft.com has been found and gives the corresponding IP address.

Each time your device connects to the internet, it uses a local DNS server to find the name of the website you're looking for. If the DNS can’t find the site, it checks other DNS servers. If the site can't be found, or the request times out, you'll get an error message such as "DNS server not responding."

#### Routing
When the IP addresses have been added to the packet, it's ready to be transmitted across the network. If the IP address exists on your network, the packet is sent directly to the device. However, if the IP address is outside of your network, it needs to go via a router. A router is a physical device that connects one network to another.

Using our letter scenario, if your friend was only a few streets away, you might decide to deliver the message by hand. Your friend is within your local network.

However, if your friend is in a different city or country/region, you need to post the letter and let the mail service deliver it. In this instance, the postal service is the router. It takes the message from your network, then finds the best route to get it to your friend's network for delivery.

### Threats to Network Security

#### Common network attacks

> `Man-in-the-middle or eavesdropping attack:` this type of attack can occur when cybercriminals compromise or emulate routes in the network, allowing them to intercept the packets of information. Think of this as a form of wiretapping. This allows attackers to not just steal data but also compromise its integrity.

> `Distributed denial of service (DDoS) attack:` the objective of a DDoS attack is to compromise the availability of the targeted network or service. Attackers do this by bombarding the targeted network or service with millions of simultaneous requests, from sources that are distributed across the network, overwhelming it and causing it to crash.

#### Common DNS attack
A DNS attack looks to exploit weaknesses in the DNS server because they're designed for efficiency and usability, and not with security in mind. A common DNS attack is DNS poisoning. This is where the attacker changes the IP addresses in the DNS lookup tables to divert traffic from a legitimate site to a bad site that might contain malicious links or other malware.

#### Common wireless attacks
Wireless networks allow our devices to seamlessly connect to networks everywhere. In your home, the wireless network allows your smartphone, and always-on IoT devices to connect to the internet. The broad availability of these networks makes them the perfect target for cybercriminals. There are many different ways to attack a wireless network:

> `Wardriving:` the term Wardriving was popularized by a couple of 1980s movies. The attacker, typically operating from a vehicle, searches for unsecured wireless networks that have vulnerabilities. Most wardriving attacks seek to use your network for criminal activities, like hacking other computers and stealing personal information.

> `Spoofing Wi-Fi hotspots:` This is similar to a man-in-the-middle attack. The attacker uses their laptop, or a device connected to it, to offer a network access point that mimics a genuine access point. For example, if you're in a coffee shop looking to access the internet using their guest Wi-Fi, you might see a couple of access points that show the name of the business. One of those could be from a bad actor. If you connect to the bogus access point, anything you do over the network can be intercepted. It also allows the cybercriminal to direct you to bad websites or capture your private data.

#### Bluetooth attack
There has been a growth in Bluetooth devices, from smart watches and audio devices to device-to-device communication. Attacks on Bluetooth networks are less common than for wireless, mostly because the criminal needs to be within range of your device – but it's still a valid attack vector. A Bluejacking attack is where a criminal sends unsolicited messages to any Bluetooth-enabled device that's within range of their own. Bluejacking is similar to when someone rings your doorbell and then runs away before you can answer. It's mostly an annoyance.

### Protect your network

#### How a firewall protects your network
A firewall is typically the frontline of defense in your network. It's a device that sits between the internet and your network, and filters all traffic going in and out. A firewall can be software or hardware based, but for the best protection, it's good to have both types. A firewall monitors incoming and outgoing traffic. Using security rules, it keeps out unfriendly traffic, while allowing authorized traffic to pass freely.

#### Maintaining a healthy network using antivirus
Viruses come in all shapes and sizes and none of them are good for the devices and servers that use your network. Cybercriminals use viruses for many purposes, from obtaining user credentials so they can access your network, to more harmful types that encrypt all the data on a device or server unless you pay vast sums of money. Much like your body fights off a virus when it gets infected, computers can also be protected with antivirus software. When antivirus software is installed it runs in the background, scanning all data that arrives on the device. A detected virus will automatically be deleted to prevent the user from accidentally running it.

You can now get antivirus protection for most devices, including servers, computers, tablets, smartphones, and any other internet-connected devices.

#### Improve authentication using network access control
While a firewall keeps unwanted devices from accessing your network, you still need to control the ones that you do want to use it. Network access control (NAC) is a security solution that manages device and user access through strict policy enforcement. Device policies control what can be done on the network and limit what the user does on a device. Through NAC, you can improve security by requiring everyone to use multifactor authentication to sign in to the network. NAC allows you to define the devices and users that can access network assets, reducing threats and stopping unsanctioned access.

#### Split your network into parts
Every room in your home has a different purpose, such as the kitchen, lounge, dining room, study, bedrooms, and bathrooms. You can control access to each of these rooms by attaching digital locks to all the doors. As a guest arrives, you can grant them a key that permits them to use specific rooms in your home. You can do the same kind of thing with your network using the concept of network segmentation.

Network segmentation creates boundaries around critical operations or assets, in much the same way as you'd put your finance team in their own office. It improves the integrity of your network assets by ensuring that, even if your network is breached, the attacker can't reach the segmented areas.

#### Secure connections using a virtual private network
A virtual private network (VPN) serves as a dedicated and secure connection, between a device and a server, across the internet. A VPN connection encrypts all your internet traffic and then disguises it so it's impossible to know the identity of the original device. This type of secure connection makes it difficult for cybercriminals to track activities and obtain your data. If you've ever connected to your work network from a public Wi-Fi hotspot, such as at an airport, you most likely used a VPN. The VPN establishes a secure connection over an insecure public network. VPN providers have become very common not just for remote work scenarios but also for personal use.

#### Encrypt your wireless network
Whether you're setting up a wireless access point in your home or place of work, enabling encryption is critical to protecting against attacks. Wi-Fi Protected Access 2 (WPA2) is the most commonly used Wi-Fi encryption method. It uses the Advanced Encryption Standard (AES) to secure the connection.