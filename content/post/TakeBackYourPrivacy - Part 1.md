---
title: "Take Back Your Privacy and Security - Part 1 - Secure your online life"
date: 2017-10-25
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
- 2FA
keywords:
- disqus
- google
- gravatar

autoThumbnailImage: false
thumbnailImagePosition: "top"
metaAlignment: center
draft: true
---
Does privacy matters? You may thing that you have nothing to hide. Like most of us, you are not engaging in criminal activities online. But how would you feel if someone followed you around, everyday, taking notes about what you buy, what you read, what you tell your friends about that weird new colleague, etc. ? In this guide, we'll review how you are tracked online and what you can do about it.
<!--more-->

But first, let cite Glenn Greenwald, a journalist that worked with Edward Snowden, from a [TED Talk](https://www.ted.com/talks/glenn_greenwald_why_privacy_matters) he gave in October 2014: *"Over the last 16 months, as I've debated this issue around the world, every single time somebody has said to me, "I don't really worry about invasions of privacy because I don't have anything to hide." I always say the same thing to them. I get out a pen, I write down my email address. I say, "Here's my email address. What I want you to do when you get home is email me the passwords to all of your email accounts, not just the nice, respectable work one in your name, but all of them, because I want to be able to just troll through what it is you're doing online, read what I want to read and publish whatever I find interesting. After all, if you're not a bad person, if you're doing nothing wrong, you should have nothing to hide." Not a single person has taken me up on that offer."*

Since the Snowden revelations, a lot of sites appeared, advocating tools to take back your privacy. The best of them is [Privacy Tools](https://www.privacytools.io/) : the site gives you a lot of information about the best tools available to protect you privacy against global mass surveillance. While you might not be worried about a government snooping on you, using these tools also protects your privacy from your Internet Service Provider, services like Google and Facebook, Ad networks, Hackers ...

In this series of post, I'll try to give you a sense of why you should care about what you do online and how to better protect yourself from hacking, tracking and surveillance.

The first thing to do in order to enforce your privacy is to secure your online life.

## Secure your accounts
### Step 1: Use a Password Manager
You probably have dozens, if not hundreds, of accounts on multiple websites. Unfortunately, remembering a different and secure password for each website is impossible. Reusing passwords is a bad idea : one day or another, one of the websites you use is going to be hack and your password might find itself freely available on the Internet.

Had a LinkedIn account in 2012? 164 millions email addresses and password were exposed in a breach.

Adobe account? In October 2013, 153 million Adobe accounts were breached with each containing a username, email, encrypted password and a password hint in plain text. The password were poorly encrypted and many were resolved back to plain text.

A lot of others services have been hacked : Yahoo, MySpace, Badoo, Dailymotion, Dropbox, Tumblr, Last.fm, Kickstarter, Forbes, Domino's, Comcast, Sony... Even websites like YouPorn, Ashley Madison (dating site for married people), Fur Affinity, ... All of these have been breached and if you reused the same password on one of those sites, it would be trivial for an attacker to get on your other accounts.

That's why you need a password manager. A password manager helps in generating different and complex passwords and remembers them for you. All you have to remember yourself is your master password, used to decrypt your other passwords. Some Password Managers offer a browser extension (so you don't have to copy/paste the password), a mobile application and some of them hosts your encrypted passwords on their servers to let you access them from anywhere.

When talking about online security, there's usually a trade off between convenience and the level of security achieved. Password Managers are not different.

Arguably, using open-source software and hosting your password database on a device you control (your PC, a USB key, ...) offers the most security but is less convenient. Using closed source password managers, on the other hand, means that you trust the developer to not lie and effectively encrypt your passwords and store them safely.

#### Free and open-source : KeePass
[Keepass](https://keepass.info/) is an open source password manager. The advantage of open source security tools is that they're open to review by the public. You could look at the code to make sure that the software does what it says. KeePass is available on Windows, Linux and Mac. The databases are encrypted using good encryption algorithms (AES and Twofish). Some developers have ported KeePass on [iOS](http://simpleanywhere.com/syncpass/index.html), [Android](http://www.keepassdroid.com/), [Windows Phone](https://www.microsoft.com/en-us/store/p/winpass/9nblggh5z10k), and there's even a [Chrome extension](https://perfectapi.github.io/CKP/). Other ports exists but I've selected those that are open source and relatively up-to-date.

TODO :
- Secure Your Accounts (Password Manager, 2FA, ...)
