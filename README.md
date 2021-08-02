
## Identity Model
1.3.1 The centralized identity model
e.g. Account-based website
![Figure1.1](https://drek4537l1klr.cloudfront.net/preukschat/HighResolutionFigures/figure_1-1.png)


1.3.2 The federated identity model
The basic idea : insert a service provider called an identity provider (IDP) in the middle
Examples :
- SAML
- OAuth
- OpenID Connect
- SSO
![Figure1.2](https://drek4537l1klr.cloudfront.net/preukschat/Figures/CH01_F02_Preukschat.png)

1.3.3 The decentralized identity model
A new model, inspired by blockchain technology since 2015

- DIDs as a new decentralized identity standard.
- Not account-based
- peer-to-peer relationship, neither of you has an 'account'; both share a 'connection'

![Figure1.4](https://drek4537l1klr.cloudfront.net/preukschat/HighResolutionFigures/figure_1-4.png)


- Blockchain for decentralized identity model

```
Public/private key cryptography is a way of securing data
via mathematical algorithms based on cyptographic keys held by each party.

Instead of using blockchain technology for cryptocurrency,
identity management uses it for decentralized public key infrastructure (DPKI).

In essence, blockchain technology and other decentralized network technologies can give us a strong,
decentralized solution for
1. Exchanging public keys directly to form private, secure connections between any two peers
2. Storing some of these public keys on public blockchains to verify the signatures on digital identity credentials (aka verifiable credentials) that peers can exchange to provide proof of real-world identity
```

## The basic building blocks of SSI

SSI is a set of technologies that build on core concepts in identity management, distributed computing, blockchain or distributed ledger technology (DLT), and cryptography.

2.1 Verifiable credentials (aka digital credentials)
2.2 The trust triangle: issuers, holders, and verifiers
2.3 Digital wallets
2.4 Digital agents

2.5 Decentralized identifiers (DIDs)

Knowing the IP address of a machine on the internet doesn’t tell you anything about the identity of
the person, organization, or thing controlling that machine.
To do that, the controller (the identity holder) needs to be able to provide proof
about their identity, attributes, relationships, or entitlements.
And that proof has to be verifiable in some way.

We’ve had technology for creating digital proofs for decades now
: **Public/private key cryptography**
The owner of a private key uses it to sign messages, and anyone else can verify this signature
using the owner’s corresponding public key.
The signature verification shows that the signature was created by the owner of
the private key and the message has not been tampered with since.

However, to rely on this verification, the verifier must know the correct public key for the owner.
So, for decentralized messaging between digital agents and wallets to be secure—
and for agents to be able to send cryptographically verifiable proofs of VCs to each other—
we need a strong, secure, scalable way for identity holders and their agents
to prove ownership of their public keys.
The solution has been public key infrastructure (PKI)
: The system of obtaining public key certificates from a small set of certification authorities (CAs) around the world.
: TOO centralized 
=> DIDs, a new identifier (permanent, resolvable, cryptographically verifiable, decentralized)

An example of a decentralized identifier (DID) and the associated public and private keys.
A DID functions as the address of a public key on a blockchain or other decentralized network.
In most cases, a DID can also be used to locate an agent for the DID subject (the entity identified by the DID).
![Figure2.11](https://drek4537l1klr.cloudfront.net/preukschat/HighResolutionFigures/figure_2-11.png)


2.6 Blockchains and other verifiable data registries

2.7 Governance frameworks (aka trust frameworks)


8 Decentralized Identifiers

A new type of globally unique identifier
![figure8.2](https://drek4537l1klr.cloudfront.net/preukschat/HighResolutionFigures/figure_8-2.png)

A DID is a URI that can be either a URL or a URN and that can be looked up (resolved)
to get a standardized set of information (metadata) about the resource identified by the DID.
If the identified resource has one or more representations on the web, the metadata can include one or more of those URLs.
Four properties of DID:
1. Permanent
2. Resolvable
3. Cryptographically verifiable
4. Decentralized


8.2 The functional level: How DIDs work

8.2.1 DID documents

Give DID to a specialized piece of software (or hardware) called a "DID resolver"
that will use it to retrieve a standardized data structure called a DID document. 

Each DID method is required to have its own technical specification,
which must define the following aspects of the DID method:
- Method-specific identifier (sov,btcr,v1,ethr,jolo,...)
- Four basic operations can be executed on a DID: CRUD
- Security and privacy considerations specific to the DID method

It is difficult to make generic statements about the four DID operations
since DID methods can be designed in very different ways.
For example, some DID methods are based on blockchains or other distributed ledgers.
In this case, creating or updating a DID typically involves writing a transaction to that ledger.
Other DID methods do not use a blockchain; they implement the four DID operations in other ways (see section 8.2.7).


8.2.3 DID resolution
The process of obtaining the DID document associated with a DID


