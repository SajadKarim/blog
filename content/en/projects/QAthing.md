---
author:
  name: "Sajad Karim"
date: 2017-10-11
linktitle: QAthing
type:
- post
- posts
title: QAthing
weight: 10
active: true
series:
- Hugo 101
tags:
  - QA Automation
  - C/C++
  - C#
  - WIN API
  - programming
  - full-stack development
  - leadership
  - consulting
---

----
> The QAthing project aims to simplify the automation of Windows applications using an intuitive approach. By leveraging Microsoft® VisualUIVerify for UI Control inspection and a specialized library, QAthing allows users to create keywords for UI Controls, which act as descriptors. These keywords can then be used to build scripts and perform actions on the application's UI Controls. This method enables the design of custom test structures using building blocks. QAthing has proven effective in various operations and scenarios, though there are still features to be implemented. Ultimately, this project facilitates automated testing of Windows applications, streamlining the process and enhancing efficiency for educational purposes and beyond.

----

# Automating Windows Applications with QAthing

Automating any Windows application isn't a big deal; a lot of help is available over the internet. The idea was to achieve automation using a simple and intuitive way. In this regard, a few changes have been made to VisualUIVerify (its code is available). Major changes are made to grab UI Control information of any running application. VisualUIVerify is used as a UI Control inspector. A library has been developed which can run almost all the actions that any Windows UI Control supports.

Automation using this technique is like handling building blocks where you design your own test structure and scripts using individual blocks. In this idea, a keyword is a basic building block that defines any UI Control. A keyword is like a contact card (or descriptor) for any UI Control. At first, you define keywords for the UI Controls that you want to be included in your testing. Once all the keywords have been recorded, you use them in your scripts to perform supported actions.

Many operations and scenarios have been achieved using this idea. Though there are many things still left to be implemented, the work done so far in this regard is more than a POC project.

## 2-Step Automation

1. Create Keywords (UI Controls' contact card) for the application and build its KeywordBook (Phone book) file. This lets the process know about the application and its UI Controls.
2. With the help of the library, QAthing, access UI Control using Keywords, and send desired commands.

A video exhibits how easily any Windows GUI application can be automated with the help of Microsoft® VisualUIVerify + UI Automation and using the QAthing library. For more sample videos, visit the YouTube channel [QAthing Club](https://www.youtube.com/channel/QAthingClub).

The project, QAthing, was started for educational purposes, and only basic or general scenarios have been addressed in the videos. In case of complex scenarios, you may post your queries to support@qathing.com or visit the FAQ page.

## Tools and Resources

- **The Tool**: To download The Tool, click on this [Link](#).
- **The Library**: To download The Library, click on this [Link](#).
- **Sample Project**: To download the Sample Project, click on this [Link](#).
- **Iron Python**: To download Iron Python, follow this [Link](#).
- **VisualUIAVerify**: UIA Verify is a Microsoft® product. It's a test automation framework that features the User Interface Automation Test Library (UIA Test Library) and Visual UI Automation Verify (Visual UIA Verify), the graphical user interface tool. Its source code is available at this [Link](#). It populates all the UI Controls in a tree form and provides in-depth details, including supported patterns.

## Pipeline

The project has evolved tremendously from the first proof of concept (POC). Some features still need to be implemented, such as:


1. **Form-Level Operations**: Designer (in VisualUIAVerify) to define such functionality. Currently, there is no way to perform operations (e.g., form fill) that includes multiple controls (except calling them individually, which results in code/script repetition). A designer is required to provide this feature so that generic/form-level operations can be performed using the available Keywords.
2. **Python Shell Integration**: To VisualUIAVerify to execute/verify form-level operations.

