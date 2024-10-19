# Device-Based Threats and Security Controls

## Concepts Learned

### Devices and data

Why are devices an integral part of our lives? It's largely because they collect and store information, and keep us connected to other devices and services.

Think about the convenience of receiving real-time traffic information on your cell phone or the annoyance when adverts are delivered to your device, based on your internet search history. This type of targeted content is sent because our devices, through their applications, collect enormous amounts of information about us. This includes location details, websites visited, how long we stay on a site, and much more.

Connected devices also enable us to easily access and share information. For example, you've probably used your cell phone to share family photos with your friends, access a work document, or pay for something at a store.

### Devices as threat vectors
While devices help us to get our work done, and go about our daily lives, they also present opportunities to cybercriminals who want to cause harm. This is because they're threat vectors—they provide different ways in which cybercriminals can carry out attacks. For example:

- Phone, laptop, or tablet – downloading a malicious app might result in the device being contaminated with malware that can exfiltrate sensitive data stored locally, without the user’s knowledge. This compromises confidentiality and integrity because the cybercriminal can now view or modify the data.
- USB drives – cybercriminals can put malicious software or files on a USB drive and insert it into a device like a laptop. The drive could, for example, run ransomware, meaning the availability of the data has been compromised because it's locked in return for a ransom.
- Always-on home assistant devices – these devices are always listening or watching. A cybercriminal can put malicious software on the app stores for these devices. If a user then installs it, the cybercriminal could, for example, attack the device with spyware to secretly record information, and compromise data confidentiality. They could also move laterally to other home devices, and compromise their data.

#### Device vulnerabilities
A device can become compromised because of poor health, either because it doesn't have the latest security updates, or it has weak authentication. If you connect this type of device to a Wi-Fi hotspot—in an airport, for example, it's an easy target for attackers. They know the common vulnerabilities of devices and applications, and how to gain unauthorized access.

After an attacker gains access, they can run scripts to install malware. In most cases, malware like back doors or botnets can persist on the device even after it's updated. This causes further damage when a user connects the infected device to a work or home network.

Some users want to gain more control of their devices for customization or other purposes, and might resort to jailbreaking. This is where a user finds unofficial ways to get full access to the core systems of a device. The device becomes vulnerable because this action might circumvent security measures. This gives cybercriminals the opportunity to provide false guidance or software that compromises the device.

### Mitigate against device-related threats

#### Device hardening
Device hardening is how you minimize the possibility of having device vulnerabilities that can be exploited. You can use the following methods:

Make sure devices have the latest security updates.
Turn off any unused devices.
Enable security features supported through the device operating system.
Require PIN or biometrics, such as facial recognition, to access devices.
Many modern operating systems have capabilities that support device hardening. For example, users can enable automatic operating system updates to help protect against known vulnerabilities and ensure continued availability of the device. Updates also support security features such as virus and threat protection, and firewall functionality.

These features are easily enabled and can help keep your connected device secure to maintain the confidentiality and integrity of accessible data.

#### Encryption
Encryption is a process that turns information on the device into unintelligible data. The only way to make this information useful is to reverse the encryption. This requires a specific password or key that's only available to the authorized user. When the information is encrypted, it becomes useless without the correct key or password. This way, data confidentiality is maintained. The contents of a device can be encrypted in many different ways. For example, some operating systems come with built-in tools that enable you to encrypt your computer’s hard drive or any storage device you connect to it.

#### Limit application device access
So far, we've looked at the different ways in which applications and devices might be compromised, and the steps you can take to mitigate threats. However, one of the more overlooked attack vectors is when someone directly uses your apps on the physical device.

Suppose you've left your smartphone on the desk and hurried off for an urgent meeting. A bad actor could use your phone to access any of your apps. They could send messages, access bank accounts, and make purchases—all by using apps from your device. If they're smart, they'd leave the device where they found it, so you would never know.

This threat also applies to your work computer. Suppose you're busy working on important and sensitive data, and step away from your computer to get a coffee. A criminal could now use the unsecured computer to look up secret or sensitive data, or download it to a USB drive.

In these two cases, everything the bad actor does will be logged and tracked in your name. There's little chance that the bad actor's actions will be traced back to them, and you'll have to deal with the fallout and clean-up.

The best way to limit access to your applications is to ensure that they're closed or secured when you aren't using them. You do this by locking a device when you step away from it. If the device is small enough, keep it with you.