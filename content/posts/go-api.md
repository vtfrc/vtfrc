---
title: "Health tracking API in Go"
date: 2023-09-17T11:29:00+02:00
draft: false
---

Several people have been talking about [Go](https://go.dev) for a while. I've never felt the need to learn it, but today [one video](https://www.youtube.com/watch?v=iCVkuWgtJlg) caught my attention. A sudden wave of FOMO caught me, and I decided to try and learn it via a quick project.

Considering how much the health world inspires me — and yes, I'll still be working on [Healti](/healti) in the future — I thought it would be nice to build a health-related API to just get my hands dirty with this technology.

Go is praised as an easy-to-read language, with strong concurrency support, and of course static typing. Its syntax looks a bit different compared to the other popular languages I know, but I agree with its readability. Not being used to dealing with memory, I didn't find the pointer notations and operators that straightforward, but still kind of easy to catch up on.

That said, I had the pleasure to use some of the integrated modules from the (rich) standard library, [GORM](https://gorm.io) to interact with the database, [Gin](https://gin-gonic.com/) as the backend framework, [Gorilla](https://gorilla.github.io/) for the WebSocket implementation, and [GoDotEnv](https://github.com/joho/godotenv) for environment variables management.

As of now, these are the features the project has:

- user registration and authentication
- health-related journaling
- exercise and nutrition logging (_to be added_)
- WebSocket-based reminders (_to be completed_)

While, since it is a backend project, these are the available endpoints:

- `/register`, `/login` (for registration and authentication)
- `/journal`, `/journal/entries`, `journal/:id` (for journaling operations)
- `/exercise/entries`, `/exercise/:id` (for exercise logging, _to be added_)
- `/nutrition/entries`, `/nutrition/:id` (for nutrition logging, _to be added_)
- `/reminders`, `/reminder/:id` (for reminders, _to be added_)

You can check out the complete code at [github.com/vtfrc/go-health](https://github.com/vtfrc/go-health).

While this is just a quick experiment, I'll add the remaining pieces. I tend to lean towards batteries-included frameworks, but I like Go and I'm definitely going to keep learning it.
