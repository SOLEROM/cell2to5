# rnd

## emergency

* solution to be able to locally switch to specific optionally supported Profiles, i.e. for testing/certification or for emergency cases
* An Operational Profile with a Profile Attribute allocated,indicating that this Profile is an Emergency Profile.

* Local Enable
```
A function of the interface between a Device and an
eUICC that provides the capability for a Device to locally
enable the Emergency Profile on the eUICC without
involvement of an SM-SR and/or SM-DP.
```

## os update

* eUICC OS Update
* Mechanism to correct existing features on an eUICC by the original OS Manufacturer when the eUICC is in the field

## sms
* The eUICC SHALL support the sending of secure packet over SMS as defined in 3GPP TS 31.115 
* make use of a special SMS for triggering the opening of an HTTPS session to the eUICC.

