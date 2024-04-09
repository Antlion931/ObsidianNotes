#cybersecurity 

# Potential vectors of attack
## Eavesdrop
If communication between two devices doesn't use one time tokens or isn't encrypted. There is a risk involved.
### Magnetic strip on Credit cards
Although it is not an [[RFID]] technology, it is great example why data send by [[NFC]] should be encrypted. On every credit card there is an magnetic strip that let's you pay in some variants of terminals.

![[magnetic-strip-card-reader.jpg]]

It stores unencrypted data that let's someone use a credit card. If that person additionally knows your PIN, he can clean your bank account. That why thieves make a devices called skimmer that is place on card reader in ATM machines and an camera that record you entering a PIN code or even new keypad.

![[skimmer.jpg]]

![[skimmer03.png]]

![[skimmer02.png]]

[[NFC]] tag sends data with use of radio waves with range of 10 cm, that makes a risk of other device to eavesdrop communication. In addition an [[NFC]] tag can be stolen. So if it contains any personal data, it should be encrypted to make it harder to get.

- [ ] #todo write about copping an [[NFC]] tag with skylanders as an example, and how you can do this with just a phone.