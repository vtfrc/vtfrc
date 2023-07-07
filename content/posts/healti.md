---
title: "My new open source experiment"
date: 2023-07-07T11:31:36+02:00
draft: true
---

I explored a lot of technologies recently. Inspired by [Fireship](https://fireship.io)'s [FKIT](https://fireship.io/courses/sveltekit) stack, and by [shadcn](https://shadcn.com)'s [Taxonomy](https://tx.shadcn.com) project, I decided to learn a couple of new tools while open sourcing everything and building in public.

The app I'm going to work on is a health monitoring service: since 2-3 years I'm really fascinated by the idea of building something related to health, and this seemed like the perfect opportunity. I'd like to build a comprehensive service that lets you check in by collecting your health-related data, gives you an overview on your condition over time, offers custom recommendations to improve it, connects with external systems to integrate adjacent areas' resources, and more.

This is just the initial idea, and I'm sure a lot of cool features will come to mind while building. In terms of tech, I'm currently playing with 2 main tools: [Nuxt3](https://nuxt.com) and [Supabase](https://supabase.com). As I said, the FKIT stack (Firebase + SvelteKit) seems like a pretty good combo, so looking into frontend meta-frameworks (that basically offer a more complete option compared to the main frameworks) and BaaS, I stumbled into what looks like another interesting combo: Nuxt - Vue's meta-framework - and Supabase - the Firebase alternative.

Why them though? Well, I tried working with Next.js and React before, and I didn't fall in love with them. As basically everyone is aware of, the main advantage of using React today (and Next since it's becoming te de facto standard for working with React) is its ecosystem. This, and some opinions I've heard about it, made me consider Vue instead of, for example, Svelte, even though Svelte as well is becoming a widely used and supported framework.

Recently, Nuxt has seen more stable updates and releases being published, so it seemed logical to try and play with it, especially for a personal project like this, and especially because I have no particular interest in mastering React since I don't plan on taking corporate frontend jobs.

Now Supabase: here I mainly went for what inspired me, and Supabase certainly did with no vendor lock-in (not a hard contraint though), with its underlying use of Postgres granting robustness and scalability, with its nice auth solution, with its cloud and self hosted options, and with its stupidly easy Nuxt integration module built on top of its supabase-js.

And just like this I have a minimum, base product ready to build on. I already deployed this project on Vercel at [healti.net](https://healti.net), and I plan on adding cool features soon. Expect more posts covering their development.

P.s.: with the potential huge number of features this app can host in the future, I'm still deciding whether it would be better to already build a more solid backend with something like FastAPI - because I'm still inclined towards the use of Supabase for the db and auth parts. Write me on one of my profiles/contacts on the homepage if you want to give me your opinion on this.
