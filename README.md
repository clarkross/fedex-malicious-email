# Analyzing FedEx Malicious Email

> This is not a lab, this is a real sample and should be treated as such. I have obfuscated some information within in order to protect viewers of this project.

![sampleimage1](https://github.com/clarkross/fedex-malicious-email/assets/123221191/fd1d43a4-8acd-4df1-9694-eac5ce6bbfcd)

> I forwarded the email and header information to my personal workstation.

### Hints of Malicious Activity

* **From:** Fedex Shipment ```support[AT]trampolines[.]com``` -- FedEx capitalization is represented differently officially.
* ```trampolines.com``` doesn't seem like a domain name utilized by FedEx. You can even look up the domain and it resolves to something completely different.
* Images as content.
* Sense of reward (Claim Your Package).
* Included order number -- although nothing was ordered.

##### Other Observations

* Unsubscribe included to make it look authentic.
* The physical address included in the footer has no correlation with FedEX.

![sampleimage2](https://github.com/clarkross/fedex-malicious-email/assets/123221191/e4433be7-1154-488f-8966-3446f92fb41c)

* The email source IP is: ```51.159.82.94``` -- This sources from Paris, France
### Conclusion

The email should be moved to junk and no links should be clicked. The email demonstrates suspicious intents.

I decided to do some further sandbox investigation of the link within the email, however, it does not resolve to anything. Being an older email, it was most likely reported already.

I've noted some similar URL strings via other malicious analysis, and most of these reports result in phishing attempts. Further investigation of the email headers isn't really need and this should be concluded as malicious.
