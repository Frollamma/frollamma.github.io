---
published: true
layout: post
title: XRP 2024 Hackathon in Rome
date:   2024-11-24 00:00:00 +0200
embedded_pdf_filename: "Hackathon 2024 - Group F.pdf"
categories: [competitions]
tags: [hackathon, crypto, XRP]
---

On the 22th of November 2024, the _IXH24 Hackathon_ was held in Rome. It was a 24 hours hackathon with two tracks were available:

1. Develop a cryptographic protocol to vote for a new president, where the voters hand over the vote to the president and the president must declare the results. The protocol must be such that the president can't cheat.
2. Develop an application using XRPL (XRP Ledger)

I had the fortune of being the leader of a team made up of great individuals with different skills, we competed for the second track.

## Diaden

Diaden is a (fictitious) company offering a SaaS for manufacturers that allows them to avoid counterfeiting and to make each product unique.
In our example the manufacturer company produces shoes and it's called Mike:

- Mike produces its shoe
- Mike calls the Diaden SaaS and generates a unique code that represents the shoe
- Diaden created a code that represents an NFT on the XRPL, that contains all the production information (fingerprint) that make that shoe unique (product name, product series, time of creation, factory name, random seed, etc)
- From the fingerprint Diaden can generate an unique digital content attached to the shoe (for example ecoding the fingerprint as seed to generate an image using a genAI model). This is optional.
- Mike integrates the code the way they prefer (as an example as QR code on the shoe)
- The consumer can use the Diaden app and verify that the shoe is genuine, they can access to the unique digital content as well

This is what we produced:

- [Diaden presentation]()
- [Diaden frontend](https://github.com/roodeeex/diaden.git) with [demo](https://diadenn.vercel.app)
- [Diaden backend](https://github.com/Frollamma/IXH24-Hackathon)
