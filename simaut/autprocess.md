# Authentication process

## general

* When the mobile equipment starts up, it obtains the international mobile subscriber identity (IMSI) from the SIM card, and passes this to the mobile operator, requesting access and authentication. The mobile equipment may have to pass a PIN to the SIM card before the SIM card reveals this information.
* The operator network searches its database for the incoming IMSI and its associated Ki.
* The operator network then generates a random number (RAND, which is a nonce) and signs it with the Ki associated with the IMSI (and stored on the SIM card), computing another number, that is split into the Signed Response 1 (SRES_1, 32 bits) and the encryption key Kc (64 bits).
* The operator network then sends the RAND to the mobile equipment, which passes it to the SIM card.
* The SIM card signs it with its Ki, producing SRES_2 and Kc, which it gives to the mobile equipment. 
* The mobile equipment passes SRES_2 on to the operator network.
* The operator network then compares its computed SRES_1 with the computed SRES_2 that the mobile equipment returned. 
* If the two numbers match, the SIM is authenticated and the mobile equipment is granted access to the operator's network. 
* Kc is used to encrypt all further communications between the mobile equipment and the network.



