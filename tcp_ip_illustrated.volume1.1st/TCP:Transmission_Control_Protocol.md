# Chapter 17 TCP: Transmission Control Protocol

## 17.1 Introduction

We look at the fields in the TCP header. In the chapters that follow we examine all of these header fields in more detail, as we see how TCP operates.

**chapter 18: TCP connection, including connection establish and terminate**

**chapter 19-20: normal transfer of data, both for interactive use (remote login) and bulk data (file transfer)**

**chapter 21: TCP timeout and retransmission**

**chapter 22-23: TCP timer**

**chapter 24: newer TCP features and TCP performance**

## 17.2 TCP Services

TCP provides a **connection-oriented, reliable, byte stream** service.

The term *connection-oriented* means the two application s using TCP (normally considered a client and a server) must establish a TCP connection with each other before they exchange data.

There are **exactly two end points** communicating with each other on a TCP connection. Concepts that we talked about in Chapter 12, **broadcasting and multicasting, aren't applicable to TCP**.

**TCP provides reliability by doing the following**:

- The application data is broken into what TCP considers the best sized chunks to send.