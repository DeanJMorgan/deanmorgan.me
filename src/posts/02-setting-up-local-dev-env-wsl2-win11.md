---
title: Setting up a local dev environment on Windows 11
description: An in-depth guide to how I've set up my local development environment on Windows 11.
date: 2021-11-01
tags:
  - Windows 11
  - WSL2
  - Node / NPM
layout: post
templateClass: u-padding-small
---

## Precursor

Time for a quick bit of background... I am predominatly a Windows user and have been since my Dad bought our first PC which was running Windows 3.1 (Around 1993). I've used almost every version of Windows since but I am familar with and regularly use Linux (Ubuntu) and MacOS as well.

If I'm being really truthful, I really like working on Linux but I'd always given MacOS a hard time. It wasn't until joining Pinpoint (where I didn't really have much choice but to use a Mac) that I actually started to use it for development. Once I realised the similarities with Linux I actually found it quite enjoyable and realised I may have been a little overly judegemental as there are some really nice benefits to doing web development on MacOS.

I think Windows had been somewhat left behind by developers as most of the modern tools seemed to be getting built for Linux/Mac with Windows versions often being community driven, which is a bit of a shame. However, in most cases it seems as though there are now viable alternatives on Windows. This has led me to explore just how much of the development experienc

## Main Objective

Create a development environment on Windows that is similar to what I'm currently running on MacOS. The core of my current setup is as follows;

- LEMP Stack (Nginx, PHP, MySql)
- NodeJS / NPM
- Elasticsearch (Required for Magento 2.4)
- Mkcert

On MacOS most of the above is managed using Homebrew, and although that option is available (thanks to being able to run Linux via WSL), I would prefer to try and set this using the native `apt` method on Linux.

## Steps

1. Install WSL2 on Windows 11
1. Configure VSCode to work with WSL2
1. Install LEMP stack software (inc. Elasticsearch)
1. Install NVM
1. Adding SSL/HTTPS support
1. Configure nginx


## Install WSL2 on Windows 11

It's actually very simple, head to the Windows store, search for 