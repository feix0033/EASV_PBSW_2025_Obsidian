---
title: Week 05 - Introduction to System Integration
create_date: 30-01-2025 15:08
last_modify_date: 30-01-2025 15:08
aliases: 
tags: 
references:
---
## Slices
- [[01-introduction.pdf]]
- [[02-microservices.pdf]]
- [[03-project.pdf]]
- [[04-workshops.pdf]]
- [[05-microservices-design.pdf]]
## Project
### Bizcord
- We only think the Backend
	- UI will be given
- Monorepo
	- class work
	- each group take one microservice
	- trade as a real project.
		- should be have PR
		- should have code review.

### Exam


## Work shop
- Identify core domains

- message service

- because the message database can only be containing the message context with the time stamp and post/receive info.
- **One database for each** (database ownership)
- **single responsibility**
- **Loose coupling**

- auth service

- only authenticate the user access and the permission for user actions.
- **One database for each** (database ownership)

- auth database

- userid
- token
- password

- **single responsibility**

- login/logout/register

- **Loose coupling**

- profile service

- user profile
- **One database for each** (database ownership)
- **single responsibility**
- **Loose coupling**

- streaming service

- handle the video audio stream for
- **One database for each** (database ownership)
- **single responsibility**
- **Loose coupling**

