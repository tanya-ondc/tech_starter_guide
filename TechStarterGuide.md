# Tech_Starter_Guide

# Table of contents
1. Introduction
2. Onboarding
3. Reference Apps
4. Signing and Verification
5. Endoints and Environments
6. Registry
7. Domain API specifications
8. Testing
9. Servicability
10. Error Codes
11. FAQs


# 1. Introduction
This guide will walk through the end to end technical flow on getting onboarded to ONDC network.

As a first step, understand ONDC ecosystem and the participants involved in making the digital commerce transactions happen in an open unbundled network. Please go through the [guide](https://docs.google.com/presentation/d/1FJ8D_2pG9Ta4Siu3q84S4eGXZq1XyTED/edit#slide=id.g1151f945cbc_1_115) and [recording](https://drive.google.com/file/d/1c1f5FS4aOTmhIHogHs-kTyal31p7kD9N/view) here. We also have a weekly business briefing call every Tuesday at 3:00 - 4:00 PM - [Meeting Link](http://meet.google.com/wuh-hwji-qdn)


Having understood the business context of ONDC network, here is the [guide](https://docs.google.com/presentation/d/17mJ_zPjEYPagc5PZuw7FS3Ftcc-Gop4U6536wStRSag/edit#slide=id.g1204a6ff419_0_56) that will walk you through the technical overview of ONDC network. Refer to the recorded session [here](https://drive.google.com/file/d/1WuHCc59C45LClpbiIPomPMuTeClRZw7h/view?usp=sharing). We have a weekly technical briefing call every Friday at 11:00 - 12:00 PM - [Meeting link](http://meet.google.com/woj-rfzf-aqg)
 

To have more deeper insights on building trust within the open network and what are potential measures taken to build the trust. Kindly go through the consultation paper [here](http://resources.ondc.org/consultationpaper).

# 2. Onboarding

What role will your organisation play on ONDC?

You can use the following documents to help you determine your role on the network:

- [Network Participant Agreement](https://drive.google.com/file/d/1O4BoIc6TS66rA3VCyLyER53FlZBbM4Qk/view?usp=sharing)
- [Regulatory Requirements for NPs](https://docs.google.com/document/d/1QidUsNWEetURl9Yx0-JPpzzZbNkhj-cd/edit?rtpof=true)
- [Taxable Obligations for NPs](https://docs.google.com/presentation/d/1rVb9XHsxG5aCp0Vsl9IsJ-lo4xAnXTBg/edit?usp=sharing&ouid=106369910452286389453&rtpof=true&sd=true)

Once you have decided on the role to play on ONDC, they must fill the NP profile form.

- [NP Profile form](https://forms.gle/fwqvBCecRwTx5txS9)

# 3. Reference Apps

Need assistance in building the buyer or seller apps. Go through our reference buyer and seller apps source code. 

ONDC reference Buyer [WebApp](https://github.com/ONDC-Official/biap-client-node-js) and [MobileApp](https://github.com/ONDC-Official/ONDC-Mobile-Buyer-App-Private)

ONDC reference [Seller App](https://github.com/ONDC-Official/seller-app-sdk)

# 4. Signing and Verification

Below resources will help you understand the Auth Header Signing and Verification process and utilities available for the same.

[Auth Header - Signing and Verification](https://docs.google.com/document/d/1-xECuAHxzpfF8FEZw9iN3vT7D3i6yDDB1u2dEApAjPA/edit)

Signing and Verification Utilities: This utility will help you generate key pairs, create/verify authorization headers.

- [Python](https://github.com/ONDC-Official/reference-implementations/tree/main/utilities/signing_and_verification)
- [Java](https://github.com/ONDC-Official/reference-implementations/tree/main/utilities/ondc-crypto-utility-master)


# 5. Endoints and Environments

**Staging** - Staging refers to the Sandbox environment available for potential Network Participants to carry out their tech development and testing

**Pre-Production** - It is the environment where Network Participants carry out end-to-end testing before going live on the network

**Production** - It is the live environment where ONDC transactions are carried out

## ONDC Staging Endpoints

a. Registry end point
```
https://pilot-gateway-1.beckn.nsdl.co.in/lookup
```

b. Gateway end point

```
https://pilot-gateway-1.beckn.nsdl.co.in/search

https://pilot-gateway-1.beckn.nsdl.co.in/on_search
```

## ONDC Pre-Production Endpoints

a. Registry end point

```
https://preprod.registry.ondc.org/ondc/lookup

https://preprod.registry.ondc.org/ondc/vlookup
```

b. Gateway end point

```
https://preprod.gateway.ondc.org/search

https://preprod.gateway.ondc.org/on_search
```

## ONDC Production (Live) Endpoints

a. Registry end point

```
https://prod.registry.ondc.org/lookup

https://prod.registry.ondc.org/vlookup
```

b. Gateway end point

```
https://prod.gateway.ondc.org/search

https://prod.gateway.ondc.org/on_search
```

# 6. Registry

The process for entry to staging to different environments can be found in the following document:

- [Manual Entry to Staging](https://docs.google.com/document/d/1HnOeTBWvYXO8kjAEHSrR6W8XICsPfKGIT6B_IhmvVV0/edit)

- [Onboarding to Pre-Prod and Prod](https://github.com/ONDC-Official/developer-docs/blob/main/registry/Onboarding%20of%20Participants.md)

# 7. Domain API specifications

ONDC API contracts map business requirements for various use case scenarios to a set of attribute keys in different APIs and ensures interoperability, between a buyer app & seller app, as follows:
- by defining the set of attribute keys that need to be exchanged to establish a handshake
between the buyer app & seller app;
- clearly defining the single source of truth for each attribute key and thereby establishing mutability & immutability of these keys on behalf of the participants at each end of the transaction;

## Retail

- [Retail MVP](https://docs.google.com/document/d/1UZtSwLjEz8j6BZzjF5_IRGHI4oBsje09/edit?usp=sharing&ouid=103244249656832991961&rtpof=true&sd=true)
- [Retail API contract](https://drive.google.com/file/d/1Z0eT1PZ8_tthEyxli8bLs-B9oCYAZIS0/view?usp=sharing)
- [Retail Transactions contract](https://drive.google.com/file/d/1Z0eT1PZ8_tthEyxli8bLs-B9oCYAZIS0/view?usp=sharing)
- [Retail v1.2 working doc](https://docs.google.com/document/d/1LpRon1jTS__Aeg2aDzVpxdB-wB9H8vGbGnrlMLVdCpY/edit?usp=sharing)

## Logistics

- [Logistics MVP](https://docs.google.com/document/d/11mFbIIeINI2IVgKP30Md54IfuU0i5Jg-/edit?usp=sharing&ouid=103244249656832991961&rtpof=true&sd=true)
- [Logistics Transactions contract](https://docs.google.com/document/d/1LiKGK3AKwzx5GWAc5g942QKB-TzDn0gGMsvXNJgIrmk/edit?usp=sharing)
- [Logistics API contract](https://drive.google.com/file/d/1IebvnM4ZyGXllsQTFTVRAvUTlkmARnM_/view?usp=sharing)

## IGM (Issue and Grivience management)

- [IGM Process Flow](https://docs.google.com/document/d/135OCfsi5jQ7wh4H_LOoMxb0T0ZrWDYy4LTBvpYS6k_w/edit?usp=sharing)
- [IGM API Contract](https://docs.google.com/document/d/1UYGIo1fSOcA4ypnk5FuaCgUgNnu9dBQt/edit?usp=sharing&ouid=103244249656832991961&rtpof=true&sd=true)

## RSP (Reconciliation and Settlement)

- [RSP API Contract](https://docs.google.com/document/d/1ubUPAWpbbUJ4vG2h5TQ74srZBjYjrO0P/edit?usp=sharing&ouid=103244249656832991961&rtpof=true&sd=true)

## B2B

- [Grocery(B2B) API Contract](https://docs.google.com/document/d/1Zg684Akm8cw9SIVpBPkflogoh6Sh-SN1JtAsWjugzbw/edit?usp=sharing)

# 8. Testing

## Moving from staging to Pre-Prod

Kindly test end-to-end transaction flow with the ONDC ref [buyer](https://buyer-app-preprod.ondc.org/login) and [seller](https://ref-seller-app-preprod.ondc.org/) applications. 
Once tested at NPs end, kindly submit the [form](https://forms.gle/KEEHxWyCUabyY1fc8) for Demo to achieve tech compliance.

## Moving from Pre-Prod to Prod

The [checklist](https://docs.google.com/spreadsheets/d/1G7NFGmhIy5u6H3fqjl1b-Qt8Xz0SPL1Mk8EiVBeSe_o/edit#gid=0) provides the steps under technical, operational and regulatory compliance that must be completed to qualify to move into Production environment. 

## Test Cases for Logs Validation

Kindly go through the below documents based on domain to understand the business test cases required for Production go ahead. NPs need to test the logs based on the test cases using the [log utility](https://github.com/ONDC-Official/reference-implementations/tree/main/utilities/log-validation-utility) and share the final logs with ONDC tech team on [GIT](https://github.com/ONDC-Official/verification-logs).

### Retail

[Test Cases](https://docs.google.com/document/d/1ttixilM-I6dutEdHL10uzqRFd8RcJlEO_9wBUijtdDc/edit?usp=sharing)

### Logistics

[Test Cases](https://docs.google.com/document/d/1ttixilM-I6dutEdHL10uzqRFd8RcJlEO_9wBUijtdDc/edit?usp=sharing)

### IGM

[Test Cases](https://docs.google.com/document/d/1O-11TsUGLLvYgq1Fo-HNIkGIlOelBJH4/edit?usp=sharing&ouid=103244249656832991961&rtpof=true&sd=true)

### B2B

[Test Cases](https://docs.google.com/document/d/1ew9a4AzWgwFHcGqRmnv4XT_oRzHC4Qsl/edit?usp=sharing&ouid=103244249656832991961&rtpof=true&sd=true)

# 9. Servicability

- [City Codes](https://github.com/ONDC-Official/developer-docs/blob/main/City-codes.md)

- [State Codes](https://github.com/ONDC-Official/developer-docs/blob/main/State-codes.md)

- [Servicability Construct](https://docs.google.com/document/d/1f4QbVstY5m-L_-Jut5jvbeiaBKLR1ttJL_am6GG2Fko/edit?usp=sharing)

# 10. Error Codes

[Error Codes](https://github.com/ONDC-Official/developer-docs/blob/main/protocol-network-extension/error-codes.md)

# 11. FAQs

- [Order Cancellations/ Returns/ Replacements](https://docs.google.com/document/d/1M-lZSduYMFKIk1V6d8QLt-j-16-rVzYVdPn0pmbkclk/edit?usp=sharing)
- [Catalogue Mandatory Requirements](https://docs.google.com/spreadsheets/d/1BNPOgcJzKglZzj1bpx-KkjvWBpH-R50AXbdC1AKJm1g/edit?usp=sharing)
- [Payment and Settlement](https://docs.google.com/document/d/1iqLdayk488ekEzKrEs-yn6gVrevbxBkILBe5j4oIxMY/edit?usp=sharing)
- [Checklist for sellers](https://docs.google.com/document/d/1m2V3GR6UIjJK65u4JW1r35cihy7lFmuBe8_cv66mVU8/edit?usp=sharing)
