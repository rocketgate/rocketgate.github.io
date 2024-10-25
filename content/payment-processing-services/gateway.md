---
title: Gateway

params:
  tagline: Easy to use APIs have you up and running transactions in minutes.

  right_content1:
    title: Use Multiple Merchant Accounts
    content: Sophisticated and highly configurable load balancing and cascading across multiple banks, merchant accounts, platforms, processors, card issuers, currencies, websites and more.

  right_content2:
    title:  Multiple Currency Support
    content: Support for more than 60 different currencies, so you can expand your business worldwide.  Supports multiple US-based and offshore banks.
---

# Gateway

RocketGate’s sophisticated and easy to use APIs (application programming interface) in multiple languages (PHP, Java, Ruby, Python, .NET etc) enable sample code-to-processing in minutes. [See the Lifecycle of a Gateway Transactions.](/images/files/gateway-init.png)

<br />
 
## Features include:

* Support for all major credit cards including Visa, MasterCard, American Express, Discover, JCB, ChinaUnionPay, BC Card, Diners Club, Maestro and Solo.  
* Multiple currency support (see Multiple Currency page for complete list of supported currencies) 
* Support for merchants based in the United States and across the globe
* Tokenized processing (link to anchor tokenized processing for details)
* Simple per transaction pricing (no %-based fees)
* Configurable for multiple merchant accounts in order to support business continuity for acquirer and processor failures – 
  * including load balancing and cascading across multiple banks, merchant accounts and processor
  * load balancing by card issuer, currency, volume and website

<br />
 
## A few examples of load balancing, routing and cascading scenarios:

1. load balance and cascade across 2 accounts - 50% to account #1 and 50% to account #2
1. 100% to a single account with a cascade to a 2nd account
1. route to 3 accounts:  Maestro/Solo to account #1, Visa/Mastercard to account #2, JCB to account #3, EURO to account #3
1. Site based load balancing for merchants with multiple websites

<br />
 
## Tokenized Payment Processing

This can be used whether you are connected to RocketGate via Gateway or Hosted Page or Hosted Form methods. RocketGate returns a unique token after the initial transaction that allows you to process subsequent transactions, such as recurring billing or repeat purchases, without storing credit card data. This feature is supported by both our Gateway and Hosted Page solutions. See the lifecycle of [Gateway Tokenized Transactions](/images/files/gateway-token.png) and the lifecycle of [Hosted Page Tokenized Transactions](/images/files/hosted-page-token.png).
