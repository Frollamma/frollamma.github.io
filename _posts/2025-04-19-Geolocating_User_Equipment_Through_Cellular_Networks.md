---
layout: post
title: Geolocating User Equipment Through Cellular Networks
date: 2025-04-19 17:04 +0200
categories: [notes]
tag: [math, cybersecurity]
embedded_pdf_filename: "Geolocating_User_Equipment_Through_Cellular_Networks.pdf"
authors: [frollo, lorella]
---

In this paper we provide a mathematical model of the cellular network (the specific technology used is not relevant for our model), we describe a possible attack that allows an unprivileged attacker to locate a victim, without their interaction and their knowledge, in any area that has been previously "scanned" by (ab)using SMSs. We believe that this attack could be used by a motivated attacker, with limited economic resources, to perform a targeted attack. We've built tools to perform a PoC attack, unfortunately we didn't have the time to test the attack in the wild, but we made promising simulations.

This paper and all the tools were initially developed in 11 days as a project for the exam of "Mathematical Methods for Datamining".

## Possible improvements

- Use something much better than TDoA
- We suggested some methods for the attacker to reduce complexity of calculating the weights of the graph, we didn't consider that the attacker could simply fix a tower and make all the calculations from there, this also implies that the attacker is confined to a single location for the attack, but it's not a strong assumption.
