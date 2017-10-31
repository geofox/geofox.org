---
title: "Take Back Your Privacy and Security - Part 1 - Secure your Passwords"
date: 2017-10-31
slug: password-manager
categories:
- tech
- encryption
- privacy
- security
tags:
- privacy
- pgp
- gpg
- blog
- encryption
- security
- password
autoThumbnailImage: false
thumbnailImagePosition: "top"
metaAlignment: center
type: post
---
Does privacy matters? You may thing that you have nothing to hide. Like most of us, you are not engaging in criminal activities online. But how would you feel if someone followed you around, everyday, taking notes about what you buy, what you read, what you tell your friends about that weird new colleague, etc. ? In this multi-part guide, we'll review how you are tracked online and what you can do about it.
<!--more-->

But first, let cite Glenn Greenwald, a journalist that worked with Edward Snowden, from a [TED Talk](https://www.ted.com/talks/glenn_greenwald_why_privacy_matters) he gave in October 2014: *"Over the last 16 months, as I've debated this issue around the world, every single time somebody has said to me, "I don't really worry about invasions of privacy because I don't have anything to hide." I always say the same thing to them. I get out a pen, I write down my email address. I say, "Here's my email address. What I want you to do when you get home is email me the passwords to all of your email accounts, not just the nice, respectable work one in your name, but all of them, because I want to be able to just troll through what it is you're doing online, read what I want to read and publish whatever I find interesting. After all, if you're not a bad person, if you're doing nothing wrong, you should have nothing to hide." Not a single person has taken me up on that offer."*

Since the Snowden revelations, a lot of sites appeared, advocating tools to take back your privacy. The best of them is [Privacy Tools](https://www.privacytools.io/) : the site gives you a lot of information about the best tools available to protect you privacy against global mass surveillance. While you might not be worried about a government snooping on you, using these tools also protects your privacy from your Internet Service Provider, services like Google and Facebook, Ad networks, Hackers ...

In this series of post, I'll try to give you a sense of why you should care about what you do online and how to better protect yourself from hacking, tracking and surveillance.

The first thing to do in order to enforce your privacy is to secure your online life.

![Padlocks](/img/locks.jpg)
## Secure your accounts
### Step 1: Use a Password Manager
You probably have dozens, if not hundreds, of accounts on multiple websites. Unfortunately, remembering a different and secure password for each website is impossible. Reusing passwords is a bad idea : one day or another, one of the websites you use is going to be hack and your password might find itself freely available on the Internet.

Had a LinkedIn account in 2012? 164 millions email addresses and password were exposed in a breach.

Adobe account? In October 2013, 153 million Adobe accounts were breached with each containing a username, email, encrypted password and a password hint in plain text. The password were poorly encrypted and many were resolved back to plain text.

A lot of others services have been hacked : Yahoo, MySpace, Badoo, Dailymotion, Dropbox, Tumblr, Last.fm, Kickstarter, Forbes, Domino's, Comcast, Sony... Even websites like YouPorn, Ashley Madison (dating site for married people), Fur Affinity, ... All of these have been breached and if you reused the same password on one of those sites, it would be trivial for an attacker to get on your other accounts. Want to know if one of your account has been breached? Enter your email or username on [Have I Been Pwned](https://haveibeenpwned.com/) and find out. You probably will be surprised of the results!

That's why you need a password manager. A password manager helps you generate different and complex passwords and then remembers them for you. All you have to remember yourself is your master password, used to decrypt your other passwords. Some Password Managers offer a browser extension (so you don't have to copy/paste the password), a mobile application and some of them hosts your encrypted passwords on their servers to let you access them from anywhere.

When talking about online security, there's usually a trade off between convenience and the level of security achieved. Password Managers are not different. It's all about your [threat model](https://en.wikipedia.org/wiki/Threat_model) : are you worried about a State actor that can compel a software provider to give up your data or backdoor the software? Do you trust a software vendor offering a closed source app to have strong crypto and security and not rely on security by obscurity? Ask yourself those questions to choose the solution you're comfortable with.

Arguably, using open-source software and hosting your password database on a device you control (your PC, a USB key, ...) offers the most security but is less convenient. Using closed source password managers, on the other hand, means that you trust the developer to not lie and effectively encrypt your passwords and store them safely.

#### Free and open-source : KeePass
![KeePass](/img/keepass.png)

[Keepass](https://keepass.info/) is an open source password manager. The advantage of open source security tools is that they're open to review by the public. You could look at the code to make sure that the software does what it says. KeePass is available on Windows, Linux and Mac. The databases are encrypted using good encryption algorithms (AES and Twofish). Some developers have ported KeePass on [iOS](http://simpleanywhere.com/syncpass/index.html), [Android](http://www.keepassdroid.com/), [Windows Phone](https://www.microsoft.com/en-us/store/p/winpass/9nblggh5z10k), and there's even a [Chrome extension](https://perfectapi.github.io/CKP/). Other ports exists but I've selected those that are open source and relatively up-to-date.

KeePass is, in my opinion, the only viable open-source Password Manager out there. It's a great choice if free and open-source is a requierement for you. It's a great cross-platform tool that allows you to be in complete control of your data.

#### Paid and closed-source : 1Password
![1Password](/img/1Password.png)

[1Password](https://1password.com/) by AgilteBits Inc. is a password manager initially created for Mac and iOS. It now supports Android and Windows but those versions are not as polished as their iOs and macOS counterparts (they're functional). 1Password hosts your encrypted passwords on their servers (hosted on Amazon Web Services) so they're accessible everywhere you have internet (it is also cached on your devices for offline access). To encrypt your password database, 1Password  uses a combination of your Master Password and a Secret Key. AgileBits claims that, combined with a strong Master Password, the Secret Key gives you more than 128 bits of entropy. It uses AES-256 encryption with PBKDF2 key derivation. They've publish a [White Paper](https://1password.com/files/1Password%20for%20Teams%20White%20Paper.pdf) explaining their security design.

1Password doesn't have a free plan. It will cost you 2.99$ a month, billed annually. They also offer family and team plans.

Compared to KeePass, 1Password is more convenient. It offers features like Watchtower that tells you password breaches and other security problems on the websites you have saved in 1Password, integrations with 3rd-party apps so you can fill your password quickly, Secure Documents, Backups, ... Again, with 1Password, you have to trust AgileBits because it's closed source. You have to bet that they won't backdoor the software (if they did, that would probably tank their business, but they may be compelled to do so).

#### Paid and closed-source : Alternatives
There's now a lot of Password Managers on the market. [Dashlane](https://www.dashlane.com/) is worth mentioning. It's a strong competitor to 1Password. Dashlane also has a [White Paper](https://www.dashlane.com/download/Dashlane_SecurityWhitepaper_v2.8.8.pdf) explaining their security design. From a user’s Master Password, Dashlane derives a ciphering key using 10000 PBKDF2 iterations, and uses AES-256 to cipher a user’s passwords. Dashlane offers a free plan but if you want to sync passwords across devices, you need to subscribe to their Premium Offering ($3.33 per month, billed annually). If you want more features than KeePass and if you don't own a Mac or an iPhone, it's a better alternative than 1Password as it achieves features parity on almost every platform.

There's also [LassPass](https://www.lastpass.com/) (bought by LogMeIn Inc.) who has a nice free plan offering sync (you have to pay to sync with 1Password and Dashlane). For $24 a year, you can sign up for LastPass Premium with features including priority customer support, 1GB of encrypted file storage, Windows fingerprint reader support, and two-factor authentication either with a Yubikey or a thumb drive with Sesame. LastPass is probably the king of Password Managers in terms of users.

It's worth noting that [LastPass suffered from a “major architectural problem”](https://www.theguardian.com/technology/2017/mar/30/lastpass-warns-users-to-exercise-caution-while-it-fixes-major-vulnerability), which could allow an attacker to steal passwords or execute code, in March 2017. To be fair, bugs are a threat for every app, even open-source ones. In February, security researchers from The Fraunhofer Institute for Secure Information Technologie (TeamSIK) [found vulnerabilities](https://www.theregister.co.uk/2017/02/28/flaws_in_password_management_apps/) in a **lot** of Password Managers.

So there you have it. Use a Password Manager to generate strong and unique passwords for every sites you have an account on. In the next post, we will learn how to secure even more your accounts with Two Factor Authentication (2FA). Stay tuned!
