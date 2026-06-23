# Google Cloud Pub/Sub: Messaging Service Fundamentals

## Introduction

Google Cloud Pub/Sub is a fully managed messaging service that enables asynchronous communication between independent applications and services. It allows publishers to send messages to topics while subscribers receive those messages through subscriptions. This architecture supports scalable, reliable, and event-driven systems. In this lab, Pub/Sub topics and subscriptions were created, messages were published, and subscribers were used to receive and process those messages.

## Objectives

* Understand the basic concepts of Google Cloud Pub/Sub.
* Create and manage Pub/Sub topics.
* Create and manage Pub/Sub subscriptions.
* Publish messages to a topic.
* Receive messages through a subscriber.
* Gain practical experience with asynchronous messaging systems using Google Cloud.

## Key Steps Performed

### 1. Environment Setup

* Created and activated a Python virtual environment.
* Installed the Google Cloud Pub/Sub client library.
* Cloned the Pub/Sub sample repository from GitHub.
* Navigated to the sample code directory for hands-on exercises.

### 2. Topic Creation

* Examined the publisher sample script.
* Created a Pub/Sub topic named **MyTopic** using Python.
* Verified the topic by listing available topics in the project.

### 3. Subscription Creation

* Examined the subscriber sample script.
* Created a pull subscription named **MySub** for **MyTopic**.
* Verified the subscription by listing project subscriptions.

### 4. Publishing Messages

* Published messages to **MyTopic** using Pub/Sub commands.
* Sent multiple text messages to simulate communication between applications.
* Confirmed successful message delivery to the topic.

### 5. Receiving Messages

* Used the subscriber application to listen for messages.
* Pulled messages from the subscription.
* Verified that all published messages were received successfully.

## Results

The lab was completed successfully by creating a Pub/Sub topic and a corresponding subscription. Multiple messages were published to the topic and retrieved through the subscription. The successful exchange of messages demonstrated the functionality of Google Cloud Pub/Sub as an asynchronous messaging service for application communication.

## Conclusion

This lab provided practical experience with Google Cloud Pub/Sub and its publish-subscribe messaging model. By creating topics, subscriptions, publishing messages, and receiving them through subscribers, the lab demonstrated how distributed applications can communicate efficiently and reliably. The knowledge gained provides a strong foundation for building event-driven and scalable cloud applications.
