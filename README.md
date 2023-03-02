# privacy
Onboarding Guide to Privacy, Security, and Digital Soverignty


# Introduction

This is a guide that first goes over why this is important and then I go over my personal setup and strategies I use. The main goal of this write-up is to inform people and discuss ideas on how individuals to acheive privacy and security.

# Why Privacy, Security, Data and Software Sovereignty is Important.

If you do a lot of very important things (media, communication, work, etc) digitally or if you store a of assets (bank account, sensitive info, etc) digitally, you are going to want it to be private and secure. The internet can be a highly adversarial environment and privacy and security is a form of self defense.

I personally would go as far as saying privacy, security and data sovereignty even ultimately ties closely with basic human rights (freedom, democracy, freedom of speech, property rights, etc.)

On more of the note on data and digital sovereignty, I highly recommend reading “WhatsApp and the domestication of users“. The TL;DR of this article is WhatsApp is the perfect example of how mainstream digital services get users locked in to their service to ultimately exploit users and then the importance of “libre software” (if you dont know what that is, watch Richard Stallman’s TED talk to get an idea of it). 

Rather then using a service because of it is convenient, we should consider its privacy, security, governance and how much sovereignty the users have. Often times there is a spectrum and trade off between convenience versus privacy and security. I just think it is a trade off we need to be aware of and willing to accept. It takes a lot of learning and work to opt-out into alternative solutions, therefore I am writing I am sharing my current solution for review and discussion.

This is also a longer discussion so feel free to contact me if you want to discuss further.

# Resources I used

## Websites

+ Anonymous Planet - I highly recommended reading through this guide and it’s foot notes. Read the section “Understanding some basics of how some information can lead back to you and how to mitigate some:” to learn about how identifiable you are on “Clearnet” (internet without TOR/VPN) and the possibilities RFID, WI-FI, IP addresses, etc.  

+ Privacy Guides - Go through the knowledge base, think about your threat model (what you want to protect) and look through all its recommended tools. 

+ The New Oil - fairly good guide for beginners. 

+ https://www.privacytools.io/ -  I do not like all its recommendations but a good source to consider

+ https://privsec.dev/ - still going through this one.

## Books

+ Michael Bazzel - Extreme Privacy: What it Takes to Disappear 4th edition - This is the book that introduced me to privacy. The author worked at the FBI in intelligence previously.

+ Michael Bazzel - OSINT 10th edition - Great book to get into Open Source Intelligence. It is pretty eye opening to see the amount of information you can get from a million different data brokers with an email or phone number. It gets even more interesting when you get into breached data and stealer logs for security research.

## Youtube/Odysee

+ Sun Knudsen - Youtube - Sun is a self proclaimed security and privacy researcher. He previosly worked on an analytics tool (Lickstats), realized the invasiveness in tracking technologies. He does a really good job with his videos in explaining and offering step by step guides along with an updated guide on his website. I really like his transparent and personable personality and how he seeks his work to be peer reviewed.

+ Mental Outlaw - Youtube - Odysee - Kenny is a Linux enthusiast & network engineer. His videos are  commentary around recent tech events, Linux related stuff, digital privacy, and some rants. He does a really good job of explaining stuff.

+ Techlore - Youtube - I have not watched that many Techlore videos but they are good for a less technical audience.

+ Luke Smith - mostly videos on Linux, some on privacy. He is about being independent and sovereign in every sense. He might be a bit radical and even alt right by some standards. I personally think he has a pretty interesting perspective on things and he explains himself pretty well.

+ The Hated One - I mostly watched the ones on TOR

# My Current Set Up and Strategies

## Note on implementing these strategies

Reach out if you need help with anything. I will gladly help. Also, there is no elitism or moral superiority in whatever decision you make.

# Mobile Devices

Consider this video by the Wall Street Journal. If you put you sensitive data and functionality on your phone you are going to want to make it secure.

I have a iPhone and I also use GrapheneOS with a Pixel 6a.  I am slowly transitioning from iPhone to GrapheneOS.

# Computers

Having one computer be both secure/private and usable/convenient is impossible. The key to it is compartmentalization. Maybe something like this. 

## Linux

I recently bought a Thinkpad and I run Ubuntu, Mint and Tails off of it. Still playing around and trying to learn.

## MacOS

+ DrDuh Github Guide - I am still going through this list.

+ Little Snitch as a Application Firewall to control all network calls that are made. (LuLu is a open source alternative) Sun Knudsen has a video about how to use Little Snitch, why it is so important. 

The most general advice I can give is go through all the settings and change it to how you see fit. I do not sign into apple ID and I do not recommend using iCloud and Siri.

# Web Browsers

I mostly use Brave and Firefox. I have not yet found my ideal browser set up. I use Firefox Containers and uBlock Origin to control the network calls. I recommend going through Arkenfox firefox settings. There are a lot of other browsers to consider like Librewolf or an ungoogled Chromium.

# Encrypted Storage & Backups

I currently use Veracrypt containers to store all my sensitive data. That container is encrypted password. You can even have a hidden volume for plausible denability. In a later section, I will list out what I store in there to give you an idea. I backup this container on multiple USB flash drives, SD cards, and Proton Drive. I have given a copy to a few friends and family so in any case of emergency I can have them send me that container.

## Files to put in a USB/SD card backup

+ Bitwarden Password Manager backed up as csv
+ KeePassXC files like one for Recovery Codes, 2FA reset codes.
+ Contacts
+ PGP/SSH keys
+ Identification Document (passport, drivers, birth certificate, health insurance etc.)
+ Personal Docs

## VPNs

There are a lot of ads around VPNs and I think it has created a misconception on how they give you privacy. The only thing VPNs do is shift your trust from your ISP to your VPN provider. VPNs help you achieve privacy by concealing our IP address from websites you visit.

I currently use Proton VPN when browsing the internet. I am thinking about trying out https://njal.la/vpn/ or Mullvad VPN. And then eventually setting up my own VPN server with a privacy conscious web hosting service. (something like this)

## Email with email masking service

I currently use Protonmail. 

For most, if you use the same email address for a lot of things, it is very closely tied to your real identity. With OSINT a lot of information can be uncovered with that email address. This is why you should use a email forwarding service.

I currently use Simple Login. For anything that is not important, I provide an alias email address that gets forwarded to a Inbox Folder.

Here is my email strategy and addresses that I have

+ real.name@pm.me : This is considered a public email address. Provided to anyone that already knows my real identity. These will probably 
numbers@pm.me : This is a generic email without any personal identifying information. I try to keep these addresses as non-public as possible because I use them with important services like financial services. I think there are still some 4 digit domains with @pm.me still available.

I have a lot of other email addresses but feel free to compartmentalize whatever you want. Like maybe one for purchases, alias names, etc.

I have also exported all my emails out of old gmail and set up a forwarding/delete to a masked email.

Password Manager

It is very important to use a Password Managers. Security researchers unanimously agree that you must be using a password manager. It is so suprising to me how many people do not use one. If you do not use one, you are probably reusing passwords. People that claim that are not also claim that they “have their own algorithm“. That is not secure because it is probably not hard to decode or decrypt that “algorithm” once 1 of them gets breached and what makes that password unique depends on the name of the service.

I currently use a Bitwarden Premium ($10/year) for 2FA and trusted emergency access. 

I multiple KeePassXC vaults for more sensitive secrets like recovery codes, 2FA reset codes, backup codes (those 3 are literally the same thing?), SSH keys, PGP keys, a few not all of my BIP 39 seed phrases, etc

Making a good Master Password

Making a good Master password or passphrase is not easy but extremely important. I recommend watching Computerphile video and Sun Knudsen cover how password entropy works. A good master password should be memorable and have more than 40 bits of entropy (maybe more depending on your threat model). Consider writing it down and then destroying that piece of paper when you are confident you memorized it.

Idea of the passwords you actually do need to memorize

"master password" to password manager and veracrypt hidden containers

password to unlock laptop and devices and Metamask other wallets etc. (this is a weak password, less than 8 characters)

4 PIN number for ATM cards, ledger device etc.

very weak password for outer volume vercrypt.

2FA

The order of preference of 2FA is

Hardware key like (Yubikey, Onlykey, Nitrokey, Solokey, etc)

TOTP Authenticators like (Authy, Aegis, etc)

Email

Phone number

It is important to use 2FA because it significantly increases your security and much harder to hack you.

Phone numbers and VOIP numbers

It is likely the phone number you give out is very closely tied to your identity with data brokers like truecaller. Your friends saved your number and then apps will harvest your contacts data when you sync it. I “retired my 10+ year phone number by porting it over to my google voice number.

If you want to text/call with Twilio or Telnyx VOIP numbers. You can host your own version of this VOIP app with the instructions here. Or you can use the hosted one. 

An easier and free option is to use Google Voice. This is what I use when anonymity is not important and a VOIP number is accepted.

If you are price insensitive, this is a solid service for a non-VOIP private number.

Instant Messaging Platforms

Privacy Guides covers this section pretty well. Signal has great E2EE encryption. It has pretty good user adaption.

Matrix is great as a open platform and protocol. I really like the mission they are striving for. I will try to create my own Matrix server when I get a chance.

The thing getting to private text messaging is incredibly difficult because 2 people need to be on the same protocol or platform. Adaption of using something just slightly more difficult is so difficult and network effects are incredibly strong. Probably much stronger than you think. I currently have iMessage with an email but I really want to delete it. Once I delete it, I will be unable to contact some people unless its SMS text and that is actually worse.

Social Media

I deleted all the data on FB, IG. The only thing holding me back from deleting/deactivating them is the friend connection I have. Once I figure out a way to export them, I will probably delete the account. I want to get to a point where I do not need these platforms with closed ecosystems to manage that for me.

In the long run, Social Media usage has been a net negative on me. I also think it is mostly a net negative for most unless you make money on them or you have extreme discipline to only use certain features.

RSS Feed

RSS is a open protocol to subscribe to any media. I really like it because it gives you full control over your news feed. It is important to curate your own information diet. I currently use Fluent Reader but I am still working on building out my feed.

Payment

For transactions and payments I want to more privacy. I use privacy.com. 

More info on Monero XMR will be added later.

AML/CFT (Anti-Money Laundering/Combating the Financing of Terrorism) is a euphemism for warrantless surveillance.  All your banking activity is reported to the government. The 4th amendment is not doing anything anymore.

Digital Assets

I use a Ledger to generate my BIP39 seed phrase. I write it down and put it in a safe place. I then use BIP39 passphrase or “25th word“ memorize it and back it up in a KeePassXC vault.

