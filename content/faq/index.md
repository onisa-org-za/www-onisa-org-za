---
title: "Frequently Asked Questions"
---

- [What is LoRa and what is TTN?](#what-is-lora-and-what-is-ttn)
- [Which band is used in South Africa?](#which-band-is-used-in-south-africa)
- [How do I start?](#how-do-i-start)
- [How many transactions does the infrastructure support?](#how-many-transactions-does-the-infrastructure-support)


## What is LoRa and what is TTN?

The features and differences can be best explained with these two simple introductory videos:

- [ESP32 with LoRa using Arduino IDE – Getting Started (5:31)](https://www.youtube.com/watch?v=w6ygDCTSQug) 
- [The Things Network (1:31)](https://www.youtube.com/watch?v=U4UrXl-SGEo)

## Which band is used in South Africa?

We use the 868MHz band, as does Europe. Radio regulations differ worldwide and are split into regions. This is significant when ordering components where you would usually have to distinguish between 868MHz and 915MHz (North America).

## How do I start? 

There are plenty of options, here possible approaches: 

- Find a project that you are really interested in from your favorite maker site (e.g. [hackster.io](https://www.hackster.io/the-things-network), [TTN Labs](https://www.thethingsnetwork.org/labs/stories/), [TTN Mapper](https://github.com/ttnmapper/gps-node-examples)). Copy the build and modify it to your liking.

- Use a [LoRa Shield](http://wiki.dragino.com/index.php?title=Lora_Shield) instead of soldering seperate components, or a [LoPy](https://www.thethingsnetwork.org/docs/devices/lopy/), or even only a [The Things Node](https://www.thethingsnetwork.org/docs/devices/node/). 

##  How many transactions does the infrastructure support? 

The Things network has a fair use policy

- An average of 30 seconds uplink time on air, per day, per device.
- At most 10 downlink messages per day, including the ACKs for confirmed uplinks.

Which [boils down to](https://www.thethingsnetwork.org/forum/t/limitations-data-rate-packet-size-30-seconds-uplink-and-10-messages-downlink-per-day-fair-access-policy/1300) 

- 30 seconds air-time per device per day
- For 10 bytes of payload, this translates to approx.:
- 20 messages per day at SF12
- 500 messages per day at SF7
- This allows for >1000 nodes per gateway

*It is worthwhile noting that regulatory bodies commonly set the [Maximum Duty Cycle](https://www.thethingsnetwork.org/docs/lorawan/duty-cycle.html#maximum-duty-cycle) to 1% for LoRaWAN*


<small>This article is licensed under CC BY-SA 3.0. Improve by submitting a pull request or filing an issue in our [GitHub repo](https://github.com/onisa-org-za/www-onisa-org-za)</small>
