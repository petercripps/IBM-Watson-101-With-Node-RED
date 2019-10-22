# **IBM Watson 101** _with Node-RED_
This tutorial provides a practical introduction to both creating functional application prototypes, and using [IBM Watson](https://www.ibm.com/watson)'s AI capabilities, **even if you have no previous coding experience**.

Using the _flow-based visual programming_ tool [Node-RED](https://nodered.org/), we'll create a series of applications that showcase some of the capabilities of **IBM Watson**, using little or no code.

Node-RED is a flow-based programming tool, originally developed by [IBM’s Emerging Technology Services team](https://emerging-technology.co.uk/) and now a part of the [JS Foundation](https://js.foundation/). Flow-based programming was invented in the 1970s, and is a way of building an application using a network of black-boxes, or “nodes”, where each node has a well-defined purpose: it is given some data, it does transforms the data in some way, and then it passes it on to the next node in the network for further transformation, until the desired result is achieved. Think of a car going down the line of a manufacturing plant - as a car moves down the line, different machines perform different additions or modifications that contribute to the manufacturing process, until at the end the finished product rolls off the end.

The visual, "building block" nature of Node-RED makes it extremely accessible to a wide range of users. If you can use drag-and-drop within a web browser, you can operate Node-RED and build applications by connecting nodes together.

Node-RED is also **open source** and **community-driven** - basically, if there's a service you want to interact with, then the chances are that someone will have already built a set of nodes for it. Want to hook up your smart lightbulbs and change their luminosity levels with the weather? Or when you post a specific message on Twitter? Want to get a text whenever there's a BBC news alert? Or when snow is forecast? Maybe you want to access your Strava cycling performance data and build yourself a reporting dashboard?

Node-RED also integrates brilliantly with **IBM Cloud** and **IBM Watson**, allowing you to build apps that utilise the latest AI technology, all without having to be an experienced coder!

In the course of this tutorial, you will:

- set up your own **Node-RED** environment on the **IBM Cloud**
- create a **"Hello World!"** application
- build an application to **analyse the text from a webpage**
- create a live, publicly available dashboard application that uses IBM Watson to **analyse the sentiment of a news or other internet article**
- setup an AI-based **image recognition** dashboard application that can classify the objects in a given image
- import earthquake data from a third party source, and use it to **automatically map recent seismic activity**
- build an application to recognise languages and perform **translations**

## Prerequisites
- [IBM Cloud](https://cloud.ibm.com) account
- No coding experience is necessary

## Workshop materials
The materials for each part of the tutorial are contained in the subfolders README files:
* [Watson-101 Lab 1: Setting Up Your Environment](./1-Setup)
* [Watson-101 Lab 2: Hello World!](./2-Hello-World)
* [Watson-101 Lab 3: Analysing a Webpage Using Node-RED and IBM Watson](./3-NLU)
* [Watson-101 Lab 4: Building an IBM Watson Text Analytics Dashboard](./4-Dashboard)
* [Watson-101 Lab 5: Creating a Visual Recognition Application](./5-Visual)
* [Watson-101 Lab 6: Building an Earthquake Mapping Application](./6-Earthquake)
* [Watson-101 Lab 7: Constructing a Language Translation App](./7-Translation)
