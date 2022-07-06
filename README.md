# spec-vclinks

Specification for the rules and semantics that govern the verification of linked-chains of Verifiable Credentials (trust graphs).

# Status

Raw - work has not yet started.

# Goal

Many VC use cases include a “trust-graph” that shows the relationships between VC types and actors (identified by DIDs).  A key assumption in the trust architecture is that verifiers will follow linked credentials to reach the “trust anchors” that add integrity to the system.  However, there is not yet strong consensus in the VC implementer ecosystem on how best to express the links and how verifiers should interpret them. This presents several risks to the trust architecture

* Issuers may link their VCs to a trust anchor, but verifiers may not be able to follow the links.
* Malicious issuers may define links to genuine trust anchors that are not relevant to the use case which verifiers may mis-interpret. 
* Some trust graphs may require verifiers to check additional business rules - for example that the species listed in a CITES permit must be included in the species list in the linked operations permit.

The verification of a linked set of credentials therefore depends on consistent technical implementation of links and the correct evaluation of a number of credential specific business rules by verifiers. 

This repository provides guidance for implementers on the use of linked credentials and the verification of trust graphs.


