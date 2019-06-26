# TMSI

* The TIMSI (Temporary IMSI) is a pseudo-random number generated from the IMSI (International Mobile Subscriber Identity) number.
* The TIMSI is utilized in order to remove the need to transmit the IMSI over-the-air. This helps to keep the IMSI more secure.
* To track a GSM user via the IMSI/TIMSI, an eavesdropper must intercept the GSM network communication where the TIMSI is initially negotiated. In addition, because the TIMSI is periodically renegotiated, the eavesdropper must intercept each additional TIMSI re-negotiation session.

* used in CS domain allocated by VLR
* timsi has only local significane withing a VLR and the area controlled by a VLR
