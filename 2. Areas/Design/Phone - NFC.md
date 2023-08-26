## Mobile

**How**
Use P2P for active TAQ
Use card emulation? for passive
Flutter NFC Package  → https://github.com/nfcim/flutter_nfc_kit/tree/master
or 
Web NFC JSON → **https://w3c.github.io/web-nfc/#write-and-read-json-serialized-and-deserialized**

**What**

**Security**
	Two attacks that are important to focus on:
	- Man in the Middle
		How to pre-encrypt or ensure data is untampered during NFC
		- Certificates from PORTOL and TAQ 
			or
		- Can wallet pub/priv key act as a certificate
	- Side Channel 
		- secure key storage and hashes inside device's TEE
		- private key is unknown to all, even NFQ

Ideas: 
Use TCP and maybe SSH to connect a phone to TAQ through WIFI?
	pros: standardized tooling, secure (hard to MITM) 
	cons: where does NFC fit in? can it securely start an auth? do businesses need a separate WIFI?
No transfer of value over NFC
	easier to secure


