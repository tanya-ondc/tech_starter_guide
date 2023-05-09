# tech_starter_guide

# Table of contents
1. Introduction
2. 


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

# 2. Policy Documents

# 3. Ref apps

Need assistance in building the buyer or seller apps. Go through our reference buyer and seller apps source code. 

ONDC reference Buyer [WebApp](https://github.com/ONDC-Official/biap-client-node-js) and [MobileApp](https://github.com/ONDC-Official/ONDC-Mobile-Buyer-App-Private)

ONDC reference Seller App

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

## Configuration settings for ONDC Staging Environment

a. Registry end point

https://pilot-gateway-1.beckn.nsdl.co.in/lookup

b. Gateway end point

```
https://pilot-gateway-1.beckn.nsdl.co.in/search

https://pilot-gateway-1.beckn.nsdl.co.in/on_search
```

## Configuration settings for ONDC Pre-Production Environment

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

## Configuration settings for ONDC Production (Live) Environment (N)

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

The process for entry to staging can be found in the following document:

- [Manual Entry to Staging](https://docs.google.com/document/d/1HnOeTBWvYXO8kjAEHSrR6W8XICsPfKGIT6B_IhmvVV0/edit)

- 


# 7. Domain API specifications

## Retail

## Logistics

## IGM

## RSP

## B2B






