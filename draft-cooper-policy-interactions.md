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

--- abstract

This document captures a list of interactions between IETF efforts and policy efforts.


--- middle

# Introduction

This document captures a list of interactions between IETF efforts and policy efforts (e.g., regulation or legislation) around the world, past or present. The objective of this docment is merely to catalogue these interactions in a single location.

Comments and additional suggestions of policy interactions not listed here should be submitted via the issue tracker at [https://github.com/coopdanger/draft-ietf-policy-interactions](https://github.com/coopdanger/draft-ietf-policy-interactions).

# Policy Interactions

## Encryption BCPs

- See {{?RFC1984}} and all the discussions that led up to it.
- See {{?RFC2804}} and all the discussions that led up to it.
- See {{?RFC3365}}.
- See {{?RFC7258}} and all the post-Snowden follow-on activity related to encryption: data minimization in DNS, DHCP, and elsewhere; opportunistic encryption; ACME; HTTP/2 discussions, TLS 1.3, and QUIC. All of these efforts trace some roots back to post-Snowden.

## DNS-over-HTTPS (DOH)

See {{?RFC8484}}.

* [Proposal to regulate in Russia](https://www.zdnet.com/article/russia-wants-to-ban-the-use-of-secure-protocols-such-as-tls-1-3-doh-dot-esni/)
* [GCHQ sends 'warning' to Google and Mozilla over DoH](https://www.telegraph.co.uk/news/2019/05/31/gchq-warns-google-mozilla-plans-encrypted-browsers/)
* [Congressional scrutiny of DoH](https://hub.packtpub.com/googles-dns-over-https-encryption-plan-faces-scrutiny-from-isps-and-the-congress/)

## TLS Encrypted Client Hello (ECH)

See {{?I-D.ietf-tls-esni}}.

* [Proposal to regulate in Russia](https://www.zdnet.com/article/russia-wants-to-ban-the-use-of-secure-protocols-such-as-tls-1-3-doh-dot-esni/)
* [ESNI blocked in China](https://www.zdnet.com/article/china-is-now-blocking-all-encrypted-https-traffic-using-tls-1-3-and-esni/); ECH?

## VoIP

The early years of SIP (early 2000s) had involvement from regulators and their proxies. There is a very significant amount of PSTN interop built into SIP. See {{?RFC3261}} and the rest of the document suite.

## Emergency services

ECRIT (starting mid-2000s) had extensive involvement from people working for/with Public Safety Answering Points (PSAPs) as well as some input from telecom regulators such as the FCC. See {{?RFC5222}} and the rest of the document suite.

## Caller identity authentication

STIR (and the related SHAKEN initiative) are designed to combat caller ID spoofing that uses VoIP.

See {{?RFC8224}}, {{?RFC8225}}, {{?RFC8226}}, {{?RFC8588}}.

* Regulatory mandates exist in the US, Canada, and France thus far.

## Messaging interoperability

The MIMI working group is chartered to work on interoperability for encrypted messaging.

* Instigated by requirements in the EU Digital Markets Act (DMA). Several of the key participants have met with EC staff and participated in the EC workshop on the topic. The AD and co-chairs are staying in touch with the EC staff focused on messaging interop.

## TV whitespaces database protocol

The Protocol to Access Whitespaces (PAWS) working group was created based on requirements received from the FCC after they freed up TV whitespaces spectrum for unlicensed use.

## Broadband measurement

The Large-Scale Measurement of Broadband Performance (LMAP) working group was created as a result of disparate efforts by Ofcom, the FCC, and BEREC, who were all running their own jurisdiction-specific broadband speed measurement efforts (several of them using a vendor which had its own proprietary measurement protocol). There were a few regulator participants involved in the protocol development effort.

## Incident response

There has been long-term involvement (including people in AD roles) from those involved with various CERTs and national cybersecurity authorities in several of the IETF's working groups focused on incident response and exchange of incident/vulnerability information: MILE, SACM, and DOTS.

## P2P congestion control

In 2008, the IETF hosted a workshop that was spurred by an FCC action regarding P2P traffic throttling. See {{?RFC5594}}.

## IAB

In addition to the IAB's coordination with ISOC on policy matters, the IAB also frequently contributes to policy and regulatory proceedings around the world. Some recent examples:

- 2022: FTC commercial surveillance proceeding, European Commission eIDAS comments

- 2018: NTIA comments on national privacy priorities, comments on Australian exceptional access bill

IAB workshops also frequently include regulatory or policy perspectives, for example, the unwanted traffic workshop and the CARIS workshop.

# Security Considerations

A number of the policy interactions above relate to security, encryption, and law enforcement access.


# IANA Considerations

This document has no IANA actions.


--- back

