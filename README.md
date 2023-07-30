# bookmark-search

This is the chrome extention to search the bookmark

# Creating a Chrome Extension for Bookmarks

## Introduction:

Today, I found myself unable to sleep, so I decided to utilize the time by coding something. After some thought, I came up with an idea – why not create a Chrome extension for managing bookmarks? It seemed like a fun project to work on, so I decided to give it a try.

## What is a Chrome Extension?

A Chrome extension is a tool designed to enhance your browsing experience in the Chrome browser. There are various types of Chrome extensions available, each catering to different needs. It's possible that the extension I plan to build already exists, but I am unaware of it. Nevertheless, I'll create my own and see how it turns out.

## Let's Get Started!

Although I have never developed a Chrome extension before, I'm excited to take on this challenge. My first step is to figure out how to create a Chrome extension. After some searching, I found the official Google link that provides guidance on this topic.[**Getting started guide for extention**](https://developer.chrome.com/docs/extensions/mv3/getstarted/)

## Extension files

Extensions contain different files, depending on the functionality provided. The following are some of the most frequently used files:

### **The manifest**

The extension's [manifest](https://developer.chrome.com/docs/extensions/mv3/manifest/) is the only required file that **must** have a specific file name: `manifest.json` . It also has to be located in the extension's root directory. The manifest records important metadata, defines resources, declares permissions, and identifies which files to run in the background and on the page.

### **The service worker**

The extension [service worker](https://developer.chrome.com/docs/extensions/mv3/service_workers/) handles and listens for browser events. There are many types of events, such as navigating to a new page, removing a bookmark, or closing a tab. It can use all the [Chrome APIs](https://developer.chrome.com/docs/extensions/reference/), but it cannot interact directly with the content of web pages; that’s the job of content scripts.

### **Content scripts**

[Content scripts](https://developer.chrome.com/docs/extensions/mv3/content_scripts/) execute Javascript in the context of a web page. They can also read and modify the [DOM](https://developer.mozilla.org/docs/Web/API/Document_Object_Model) of the pages they're injected into. Content Scripts can only use a subset of the [Chrome APIs](https://developer.chrome.com/docs/extensions/reference/) but can indirectly access the rest by exchanging messages with the extension service worker.

### **The popup and other pages**

An extension can include various HTML files, such as a [popup](https://developer.chrome.com/docs/extensions/mv3/user_interface/#popup), an [options page](https://developer.chrome.com/docs/extensions/mv3/options/), and [other HTML pages](https://developer.chrome.com/docs/extensions/mv3/architecture-overview/#html-files). All these pages have access to [Chrome APIs](https://developer.chrome.com/docs/extensions/reference/).

## What should be the folder structure?

!https://wd.imgix.net/image/BhuKGJaIeLNPW9ehns59NfwqKxF2/hjccQNanPjTDpIajkhPU.png?auto=format&w=1400

## How to run locally

This link gave me clear idea on how can i run the extension locally: **[Run locally](https://developer.chrome.com/docs/extensions/mv3/getstarted/development-basics/#load-unpacked)**
