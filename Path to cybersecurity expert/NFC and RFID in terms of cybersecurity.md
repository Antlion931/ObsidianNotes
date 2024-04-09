#cybersecurity 

# Potential vectors of attack
## Eavesdrop
If communication between two devices doesn't use one time tokens or isn't encrypted. There is a risk involved.
### Steeling personal data
On every credit card there is an magnetic strip that let's you pay in some variants of terminals.Although it is not an [[RFID]] technology, it is great example why data send by [[NFC]] should be encrypted.

![[magnetic-strip-card-reader.jpg]]

It stores unencrypted data that let's someone use a credit card. If that person additionally knows your PIN, he can clean your bank account. That why thieves make a devices called skimmer that is place on card reader in ATM machines and an camera that record you entering a PIN code or even new keypad.

![[skimmer.jpg]]

![[skimmer03.png]]

![[skimmer02.png]]

[[NFC]] tag sends data with use of radio waves with range of 10 cm, that makes a risk of other device to eavesdrop communication. In addition an [[NFC]] tag can be stolen. So if it contains any personal data, it should be encrypted to make it harder to get.

### Coping an NFC

If [[NFC]] tag doesn't support any tokenization and some way of authentication. Then you can simply copy what that tag send, and you can use that copy as an original. It happens with skylanders.

![[skylanders.jpg]]

Skylanders is a game, where you buy a portal, on which you place you characters. Then they became playable character in game. It used [[NFC]] as a way of detecting which hero is on portal. Some people discover that you can copy them very easily. 

![[copy_of_skylander.png]]

Nowadays it would be even easier cause everyone have at least one [[NFC]] reader/writer, new smart phones can do this with a free application.

# How credit cards deal with it

Credit cards are not simple [[NFC]] tags, but a smart card, firstly authenticate the other part. Then sends encrypted data with additional codding that let's detect errors. Terminal are under regulations, and do not give immediate access to money. Meaning it is safe. But you still need to be careful with you magnetic strip.
