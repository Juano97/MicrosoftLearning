# Authentication and Authorization in Cybersecurity

## Concepts Learned

### Authentication

#### Authentication methods

Authentication can be divided into three types: something you know, something you have, and something you are.

Something you know includes:
- Passwords
- PIN numbers
- Security questions

Something you have includes:
- Identity cards
- USB keys
- Computers
- Cell phones

Something you are includes:
- A fingerprint
- Facial recognition
- Retinal scan
- Other forms of biometric ID.

### Authentication-Based Attacks

#### Brute force attack
In a brute force attack, a criminal will attempt to gain access simply by trying different usernames and password combinations. Typically, attackers have tools that automate this process by using millions of username and password combinations. Simple passwords, with single-factor authentication, are vulnerable to brute force attacks.

#### Dictionary attack
A dictionary attack is a form of brute force attack, where a dictionary of commonly used words is applied. To prevent dictionary attacks, it’s important to use symbols, numbers, and multiple word combinations in a password.

#### Credential stuffing
Credential stuffing is an attack method that takes advantage of the fact that many people use the same username and password across many sites. Attackers will use stolen credentials, usually obtained after a data breach on one site, to attempt to access other areas. Attackers typically use software tools to automate this process. To prevent credential stuffing, it's important not to reuse passwords, and to change them regularly, particularly after a security breach.

#### Keylogging
Keylogging involves malicious software that logs keystrokes. Using the key logger, an attacker can log (steal) username and password combinations, which can then be used for credential stuffing attacks. This is a common attack at internet cafes or anywhere you use a shared computer for access. To prevent keylogging, don't install untrusted software and use reputable virus-scanning software.

Keylogging isn't limited to just computers. Suppose a bad actor installs a box or device over the card reader and keypad at an ATM. When you insert your card, it passes first through the bad actors card reader - capturing the card details, before feeding it into the ATMs card reader. Now, when you key in your pin using the bad actor's keypad, they get your pin as well.

#### Social engineering
Social engineering involves an attempt to get people to reveal information or complete an action to enable an attack.

Most authentication attacks involve exploitation of computers or an attempt to try many credential combinations. Social engineering attacks are different in that they exploit the vulnerabilities of humans. The attacker tries to gain the trust of a legitimate user. They persuade the user to divulge information or take an action that enables them to cause damage or steal information.

A number of social engineering techniques can be used for authentication theft, including:

> `Phishing` occurs when an attacker sends a seemingly legitimate email with the objective of having a user reveal their authentication credentials. For example, an email might appear to be from the user’s bank. A link opens to what looks like the bank’s sign-in page, but is actually a fake site. When a user logs in at the fake site, their credentials become available to the attacker. There are several variations of phishing, including spear-phishing, which targets specific organizations, businesses, or individuals.

> `Pretexting` is a method where an attacker gains the victim's trust and convinces them to divulge secure information. This can then be used to steal their identity. For example, a hacker might call you, pretending to be from the bank, and ask for your password to verify your identity. Another approach uses social media. You might get asked to complete a survey or a quiz, where they asked seemingly random and innocent questions that get you to reveal personal facts, or you'll get something that looks fun, like making up the name for your fantasy pop-star band by using the name of your first pet and the place you were born.

> `Baiting` is a form of attack where the criminal offers a fake reward or prize to encourage the victim to divulge secure information.