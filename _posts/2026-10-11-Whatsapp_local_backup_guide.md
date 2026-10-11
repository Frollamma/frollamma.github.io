---
published: true
layout: post
title: Whatsapp Local Backup Guide
description: A guide on how to Backup your backup chats and browse them offline on your computer (or any device)
date: 2026-10-11 13:20:00 +0200
categories: ["hacking"]
tags: [hacking, android, tools]
authors: [frollo]
---

This guide was born because I didn't find any complete guide online on how to backup Whatsapp chats on PC, so I built my own. I used multiple open source tools along the way.

> **Disclaimer** This guide is not an endorsement to use Whatsapp, actually you should escape it, boycott it and use alternative, ethical and free apps (so far my favourite is [DeltaChat](https://delta.chat/)) and share them with your friends. So, quite the opposite, this guide is meant as way to take your data **off** Whatsapp and, if you need to keep using it, be independent from their backup infrastructure and pay no subscriptions.

## Scope

What you will be able to do following this guy:

- Backup your Whatsapp chats from your phone to your computer
- Restore your Whatsapp chats without using any cloud service
- Visualize your chats offline on your computer
- Automate this process

This guide will focus on Whatsapp running on an Android phone, if you're on iOS, you should make slight variations that I try to mention, similarly, the backup is stored/visualized on a computer, but you could also keep it on your phone or any other device.

## Setting up

To follow this guide you need to have set up an End-to-End encrypted Whatsapp backup with a 64 hex chars (32 bytes) key, if you have already, great, skip to the next section, otherwise keep following here.

Go to chat backup Whatsapp settings (should be Settings -> Chats -> Chat Backup), there is an option for End-to-End encrypted backups, if you never used it, just set the 64 chars key, if you instead have an existing E2EE backup that doesn't use a 64 chars key, select "Turn off" and set it up again.
Since Meta and Google are despicable companies, on Android, if you set up a backup using Google Drive, and you don't have enough storage for an online backup, the button "Back Up" will fail, leaving you to wonder if the local backup worked anyway.
I didn't test it, I just used the free trial of Google One to get more storage for a month, but you can (contact me if you do), you simply need to run the backup anyway and when it fails you keep following this guide, when you will decrypt the database you can look for recent chats, if they are there, then it means that locally it worked.

Whatsapp will show you the 64 chars code **only once**, so copy it and save it somewhere safe, you can also take a screenshot, but it's better to copy it.

## Backing up

To have a fully independent Whatsapp backup
