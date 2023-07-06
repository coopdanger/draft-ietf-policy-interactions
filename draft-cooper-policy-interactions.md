---
title: "IETF Policy Interactions"
category: info
ipr: trust200902
docname: draft-cooper-policy-interactions-latest
submissiontype: IETF
date: {DATE}
v: 3
venue:
  github: "coopdanger/draft-ietf-policy-interactions"
  latest: "https://coopdanger.github.io/draft-ietf-policy-interactions/draft-cooper-policy-interactions.html"

author:
 -
    fullname: Mark Nottingham
    email: "mnot@mnot.net"
 -
    fullname: Alissa Cooper
    organization: Cisco
    email: "alcoop@cisco.com"

normative:

informative:
CLIPPER:
  display: Clipper
  target: https://cryptomuseum.com/crypto/usa/clipper.htm
  title: "Clipper Chip: Cryptographic Key Escrow"

--- abstract

This document captures a list of interactions between IETF efforts and policy efforts.


--- middle

# Introduction

This document captures a list of interactions between IETF standards-related efforts and external policy efforts (e.g., regulation or legislation) around the world, past or present. The objective of this document is merely to catalogue these interactions in a single location.

Comments and additional suggestions of policy interactions not listed here should be submitted via the issue tracker at [https://github.com/coopdanger/draft-ietf-policy-interactions](https://github.com/coopdanger/draft-ietf-policy-interactions).

# Policy Interactions

## Encryption and Access to Communications

THE IETF has a history of publishing documents that respond to policy developments surrounding the use of encryption, and more generally regarding access to communications.

{{?RFC1984}} stated the IESG and IAB's position regarding legal constraints on encryption in 1996, with a focus on the effects on the Internet. The publication of the document was prompted in part by the controversy surrounding the US government's promotion of the Clipper Chip {{CLIPPER}}. The document was elevated to Best Current Practice (which requires IETF-wide consensus) in 2015.

{{?RFC2804}} articulates why the IESG and IAB believed that it was not appropriate to accommodate wiretapping requirements from law enforcement, circa 2000.

{{?RFC3365}} set a requirement for IETF standard protocols to use 'appropriate strong security mechanisms', including encryption. It was published as Best Current Practice in 2002.

{{?RFC7258}} documents IETF consensus that pervasive monitoring is an attack, and thus should be mitigated in IETF protocols (often, using encryption). It was a response to the Snowden revelations, and followed the Workshop on Strengthening the Internet Against Pervasive Monitoring (STRINT) <https://www.w3.org/2014/strint/>, held jointly by the W3C and IAB. Follow-on work to implement {{RFC7258}} includes opportunistic encryption {{RFC7435}} {{RFC8110}} {{RFC8164}}, data minimization {{RFC7816}} {{RFC9156}}, improvements to the encryption ecosystem such as {{?ACME=RFC8555}}, and discussion of mandatory encryption in {{?HTTP2=RFC7540}}, {{?TLS13=RFC8446}}, and {{?QUIC=RFC9110}}.

## DNS-over-HTTPS (DOH)

{{?DOH=RFC8484}} was a technical response to pervasive monitoring attacks on DNS.

Some related news reporting:
* [Proposal to regulate in Russia](https://www.zdnet.com/article/russia-wants-to-ban-the-use-of-secure-protocols-such-as-tls-1-3-doh-dot-esni/)
* [GCHQ sends 'warning' to Google and Mozilla over DoH](https://www.telegraph.co.uk/news/2019/05/31/gchq-warns-google-mozilla-plans-encrypted-browsers/)
* [Congressional scrutiny of DoH](https://hub.packtpub.com/googles-dns-over-https-encryption-plan-faces-scrutiny-from-isps-and-the-congress/)

## TLS Encrypted Client Hello (ECH)

{{?ECH=I-D.ietf-tls-esni}} is a work-in-progress effort to respond to pervasive monitoring attacks on TLS SNI, which exposes the hostname =being connected to, even when several hostnames are served by the same IP address.

Some related news reporting:
* [Proposal to regulate in Russia](https://www.zdnet.com/article/russia-wants-to-ban-the-use-of-secure-protocols-such-as-tls-1-3-doh-dot-esni/)
* [ESNI blocked in China](https://www.zdnet.com/article/china-is-now-blocking-all-encrypted-https-traffic-using-tls-1-3-and-esni/)

## Voice over IP

The development of the Session Initiation Protocol (SIP) in the early 2000s had involvement from regulators and their proxies. There is a very significant amount of PSTN interop built into SIP. See {{?RFC3261}} and the rest of the SIP document suite.

## Emergency services

The Emergency Context Resolution with Internet Technologies (ECRIT) working group, which began in the starting mid-2000s, had extensive involvement from people working for/with Public Safety Answering Points (PSAPs) as well as some input from telecom regulators such as the US Federal Communications Commission (FCC). See {{?RFC5222}} and the rest of the document suite.

## Caller identity authentication

Secure Telephone Identity Revisited (STIR) and the related SHAKEN initiative are designed to combat caller ID spoofing that uses VoIP.

See {{?RFC8224}}, {{?RFC8225}}, {{?RFC8226}}, and {{?RFC8588}}.

Regulatory mandates to use STIR exist in the US, Canada, and France thus far.

## Messaging interoperability

The More Instant Messaging Interoperability (MIMI) working group is chartered to work on interoperability for encrypted messaging. This work was instigated based on requirements in the EU Digital Markets Act (DMA). Several of the key participants have met with European Commission (EC) staff and participated in an EC workshop on the topic. The area director and co-chairs are staying in touch with the EC staff focused on messaging interoperability.

## TV whitespaces database protocol

The Protocol to Access Whitespaces (PAWS) working group was created based on requirements received from the FCC after they allocated TV whitespaces spectrum for unlicensed use.

## Broadband measurement

The Large-Scale Measurement of Broadband Performance (LMAP) working group was created as a result of disparate efforts by Ofcom in the UK, the FCC, and the Body of European Regulators of Electronic Communications (BEREC), who were all running their own jurisdiction-specific broadband speed measurement efforts (several of them using a vendor which had its own proprietary measurement protocol). There were regulator participants involved in the protocol development effort.

## Incident response

There has been long-term involvement (including people in area director roles) from those involved with various CERTs and national cybersecurity authorities in several of the IETF's working groups focused on incident response and exchange of incident/vulnerability information: Managed Incident Lightweight Exchange (MILE), Security Automation and Continuous Monitoring (SACM), and DDoS Open Threat Signaling (DOTS).

## P2P congestion control

In 2008, the IETF hosted a workshop that was spurred by an FCC action regarding P2P traffic throttling. See {{?RFC5594}}. Related challenges associated with multiplexing flows with different characteristics were addressed in the Active Queue Management working group (see, e.g., {{RFC7567}}) and in the Congestion Exposure working group (see, e.g., {{RFC7713}}).

## Internet Architecture Board (IAB)

In addition to the IAB's coordination with the Internet Society on policy matters, the IAB also frequently contributes to policy and regulatory proceedings around the world. Some recent examples:

- 2022: FTC commercial surveillance proceeding, European Commission eIDAS comments

- 2018: NTIA comments on national privacy priorities, comments on Australian exceptional access bill

IAB workshops also frequently include regulatory or policy perspectives, for example, the unwanted traffic workshop and the CARIS workshop.

# Security Considerations

A number of the policy interactions above relate to security, encryption, and law enforcement access.


# IANA Considerations

This document has no IANA actions.


--- back

