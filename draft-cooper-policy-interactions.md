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

informative: RFC8224: RFC8225: RFC8226: RFC8588: RFC8484: RFC1984: RFC2804: RFC3365: RFC7258: RFC3261: RFC5222: RFC5594:


--- abstract

This document captures a list of interactions between IETF efforts and policy efforts.


--- middle

# Introduction

This document captures a list of interactions between IETF efforts and policy efforts (e.g., regulation or legislation) around the world, past or present, successful or not. The objective of this docment is merely to catalogue these interactions in a single location.

Comments and additional suggestions of policy interactions not listed here should be submitted via the issue tracker at [https://github.com/coopdanger/draft-ietf-policy-interactions](https://github.com/coopdanger/draft-ietf-policy-interactions).

# Policy Interactions

## STIR/SHAKEN

Combatting caller ID spoofing using VoIP.

RFCs 8224-6, 8588.

* FCC-mandated, expanded to Canada.

## MIMI

Interoperability for encrypted messaging.

* Instigated by requirements in the EU DMA. Several of the key participants have met with EC staff and participated in the EC workshop on the topic. The AD and co-chairs are staying in touch with the EC staff focused on messaging interop.

## DoH

DNS-over-HTTPS.

[RFC8484](https://www.rfc-editor.org/rfc/rfc8484.html).

* [Proposal to regulate in Russia](https://www.zdnet.com/article/russia-wants-to-ban-the-use-of-secure-protocols-such-as-tls-1-3-doh-dot-esni/)
* [GCHQ sends 'warning' to Google and Mozilla over DoH](https://www.telegraph.co.uk/news/2019/05/31/gchq-warns-google-mozilla-plans-encrypted-browsers/)
* [Congressional scrutiny of DoH](https://hub.packtpub.com/googles-dns-over-https-encryption-plan-faces-scrutiny-from-isps-and-the-congress/)

## ECH

TLS Encrypted Client Hello.

Ongoing [draft in the TLS WG](https://datatracker.ietf.org/doc/draft-ietf-tls-esni/).

* [Proposal to regulate in Russia](https://www.zdnet.com/article/russia-wants-to-ban-the-use-of-secure-protocols-such-as-tls-1-3-doh-dot-esni/)
* [ESNI blocked in China](https://www.zdnet.com/article/china-is-now-blocking-all-encrypted-https-traffic-using-tls-1-3-and-esni/); ECH?

## Encryption BCPs

- RFC 1984 and all the discussions that led up to it
- RFC 2804 and all the discussions that led up to it
- RFC 3365
- RFC 7258 and all the post-Snowden follow-on activity related to encryption; data minimization in DNS, DHCP, and elsewhere; opportunistic encryption (however impotent that proved to be); ACME; HTTP/2 discussions, TLS 1.3, and QUIC --> I think all of these efforts trace some roots back to post-Snowden.

## VoIP

Early years of SIP (early 2000s) had involvement from regulators and their proxies -- obviously there is a ton of PSTN interop built into SIP. RFC 3261 and the rest of the document suite.
.

## Emergency services

ECRIT (starting mid-2000s) had extensive involvement from people working for/with Public Safety Answering Points (PSAPs) as well as some input from telecom regulators like the FCC. RFC 5222 and the rest of the document suite.

## TV whitespaces database protocol

PAWS (2014-15) -- this whole WG was created based on requirements received from the FCC after they freed up the TV whitespaces spectrum for unlicensed use.

## Broadband measurement

LMAP (2013-2018) -- WG was created as a result of disparate efforts by Ofcom, FCC, and BEREC who were all running their own jurisdiction-specific broadband speed measurement efforts (several of them using SamKnows which had its own proprietary measurement protocol). There were a few regulator people who stayed involved in the protocol development effort, although the protocol itself did not get used much.

## Incident response

There has been long-term involvement (including people in AD roles) from those involved with various CERTs and national cybersecurity authorities in several of the IETF's working groups focused on incident response and exchange of incident/vulnerability information: MILE, SACM, DOTS.

## P2P congestion control

In 2008, the IETF hosted an entire workshop that was spurred by an FCC action against Comcast regarding P2P traffic throttling. See RFC 5594.

## IAB

In addition to the IAB's coordination with ISOC on policy matters, the IAB also frequently contributes to policy and regulatory proceedings around the world. Some recent examples:

- 2022: FTC commercial surveillance proceeding, EC eIDAS comments

- 2018: NTIA comments on national privacy priorities, comments on Australian exceptional access bill

IAB workshops also frequently include regulatory or policy perspectives. E.g., the unwanted traffic workshop, the CARIS workshop

# Security Considerations

A number of the policy interactions above relate to security, encryption, and law enforcement access.


# IANA Considerations

This document has no IANA actions.


--- back

# Acknowledgments
{:numbered="false"}

TODO acknowledge.
