---
sip: <to be assigned>
title: Add DeFi subindex synths
status: WIP
author: Afif Bandak (@ab589)
discussions-to: <Create a new thread on https://research.synthetix.io and drop the link here> 

created: <date created on, in ISO 8601 (yyyy-mm-dd) format>
requires (*optional): <SIP number(s)>
---

<!--You can leave these HTML comments in your merged SIP and delete the visible duplicate text guides, they will not appear and may be helpful to refer to if you edit it again. This is the suggested template for new SIPs. Note that an SIP number will be assigned by an editor. When opening a pull request to submit your SIP, please use an abbreviated title in the filename, `sip-draft_title_abbrev.md`. The title should be 44 characters or less.-->

## Simple Summary
<!--"If you can't explain it simply, you don't understand it well enough." Simply describe the outcome the proposed changes intends to achieve. This should be non-technical and accessible to a casual community member.-->
Add index synths for DeFi verticals 
- DEX protocols (DEX/iDEX)
- Lending protocols (sLEND/iLEND)
- Derivatives (sDERI/iDERI)
- Structured products (sPROD,iPROD)

## Motivation
<!--This is the problem statement. This is the *why* of the SIP. It should clearly explain *why* the current state of the protocol is inadequate.  It is critical that you explain *why* the change is needed, if the SIP proposes changing how something is calculated, you must address *why* the current calculation is innaccurate or wrong. This is not the place to describe how the SIP will address the issue!-->
As DeFi continues to expand, markets for specific services are increasingly crowded. While sDEFI provides exposure to a basket of DeFi tokens, adding subindex synths for various DeFi  verticals can offer more focused diversification.

## Specification
<!--The specification should describe the syntax and semantics of any new feature, there are five sections
1. Overview
2. Rationale
3. Technical Specification
4. Test Cases
5. Configurable Values
-->
These synths will all be indices implemented in the same way as sDEFI/iDEFI synths. Upper and lower thresholds for inverse synths will be added to the SIP before deployment. Each index will be comprised of the following assets:
1. sDEX: UNI, SUSHI, CRV, ZRX, BAL, BNT, KNC 
2. sLEND: AAVE, COMP, MKR, CREAM
3. sDERI: SNX, UMA, MIR, PERP, DDX, INJ
4. sPROD: YFI, ALPHA, BOND, SFI, DHT

### Rationale
<!--This is where you explain the reasoning behind how you propose to solve the problem. Why did you propose to implement the change in this way, what were the considerations and trade-offs. The rationale fleshes out what motivated the design and why particular design decisions were made. It should describe alternate designs that were considered and related work. The rationale may also provide evidence of consensus within the community, and should discuss important objections or concerns raised during discussion.-->
Adding additional DeFi index synths will add further utility to the Synthetix protocol, allowing users to optimize passive investing strategies while also significantly lowering the cost of implementing a diversification strategy. 

### Test Cases
<!--Test cases for an implementation are mandatory for SIPs but can be included with the implementation..-->
This SIP is an extension of the functionality offered by sDEFI/iDEFI, which provide a clear example of how custom synth indicies can function successfully in the Synthetix protocol.

### Implementation
<!--Please list all values configurable via SCCP under this implementation.-->
Weightings TBD pending discussion

## Copyright
Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0/).
