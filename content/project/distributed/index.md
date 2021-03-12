---
title: "Distributed Travel Reservation System"
description: "Project for distributed system course"
code: "COMP512-Project"
tags: ["Distributed System", "Middleware", "TCP", "RMI", "java"]
weight: 5
report: true
draft: false
---

## Abstract

The goal of this project is to design and develop a component-based distributed travel reservation system. The concepts of distribution, coordination, scalability, and fault-tolerance are implemented in the system. This project focuses on backend design of the system, with minimal frontend interactive interface.

## System Design

The system architecture is RMI-based with middleware server that supports multiple clients and multiple resource managers. The key components of middleware is the middleware process, a centralized lock manager, and a transaction manager. The middleware process handles RMI calls, provides client user interface, stores a database for client, and maintains resource manager proxy. The centralized lock manager handles lock conversion, response to transaction manager lock requests, and prevent deadlock by timeout mechanism. The transaction manager maintains a database for transactions by hashing, and also a transaction history stack for data recovery. The database shadowing and logging are also implemented to provide crush recovery. Two Phase Commit protocol is applied to maintain the consistency of database and transactions. The concurrency control is achieved by Two Phase Lock in addition to Two Phase Commit. The system is very robust and consistent. In the event of any component disconnection or crush, the system still maintains the integrity and consistency and can be recovered efficiently and effectively. The system also scales well for large amount of clients and load injection. Despite of middleware design, it is not a bottleneck of the system. Here is an overview of the RMI-based distributed system with middleware.

{{< imgresize rmi.png "750x750" "System Design" >}}


