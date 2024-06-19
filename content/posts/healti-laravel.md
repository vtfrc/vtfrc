---
title: "Healti migrates to Laravel"
date: 2023-11-04
draft: false
---

I chose [Laravel](https://laravel.com).

I'm pretty sure I have some kind of problem that makes me want to try all sorts of alternatives for frameworks, languages, themes, apps... yeah everything.

[Healti](https://healti.net) was written in Typescript with [Nuxt and Supabase](/healti), and I like these technologies. There were a few problems though:

- I kept trying new stuff
- I don't like JavaScript and TypeScript
- I don't like frontend frameworks in general
- I rewrote (easily, but still) basic functionality like authentication, which I'd prefer to be battle-tested
- I wanted something more backend-centric

So, I considered:

- Go with Gin, Fiber, or even just the standard library
- Ruby with Rails
- Python with Django or FastAPI
- PHP with Laravel

Go's solution is way too minimal, Rails is interesting, FastAPI is too minimal as well, and I didn't try any demo with Django (for some reason I tried to stay away from Python).

I would've used [HTMX](https://htmx.org) with Go/Python, [Hotwire](https://hotwired.dev) with Rails, and [Livewire](https://livewire.laravel.com) or HTMX with Laravel.

Well, since I had already worked with Laravel once, and I love how fast you can get an app running with it (not just development but even deployment with Forge), I went with it.

I don't get the hate for PHP, plus I heard the newest versions got rid of all the problems that probably caused the hate.

Some modules from the Laravel ecosystems I love and I'm working a lot with: Blade for templating, Eloquent as the ORM, the authentication system, Forge with a provider (I use Hetzner but I also recommend Vultr) for deployment and server management, Breeze as a starter.

I already rebuilt the current core feature of the app: the OCR-powered automatic health data manager. I have to add complementary features but I have no doubts about how smooth the experience will be with Laravel.

More on this soon.

