# lettershoot

> A feed of the cool things companies ship, without the newsletters.

**Status:** idea only. No code yet. This repo exists so I don't lose the thought.

## Where this came from

On 2026-10-29 I unsubscribed from Resend and Tailscale marketing emails. Most of what
those emails contain isn't for me, but Resend in particular *does* ship features I
genuinely like. Unsubscribing meant losing that signal too.

The ratio was the problem: dig through 100% of the emails to find the ~20% that's
interesting.

## The idea

Flip it around. Instead of companies pushing everything into my inbox, I have a
**feed I pull from** that only shows the good part: **cool new features companies
are shipping**.

- **Pull, not push.** No notifications, no emails, no badges. It only does anything
  when I open it and browse.
- **Features, not marketing.** Pull out the "here's a new thing you can do" bits.
  Skip the webinars, case studies, discounts, and "we're hiring".
- **Focused on what I like.** Companies and kinds of features I care about, not
  everything.

Think **a personal Hacker News meets an RSS reader**.

### How it works (rough shape)

1. **The emails still arrive**, just not where I have to read them.
2. **An agent reads them** and looks for the specific things I care about.
3. **It writes "posts"**, one per topic that would interest me. Each post is a short
   write-up that **links back to the source emails** and the relevant links inside
   them (changelog entries, docs, blog posts).
4. **I browse the posts** like a front page. If something looks good, I click through.

Several emails about the same thing (an announcement, then a follow-up, then a
"now GA") can become a single post.

## Deliberately undecided

I'm not making these calls yet:

- **Email intake:** a dedicated inbox to resubscribe with, forwarding rules from my
  main inbox, a Gmail label, etc.
- **Other sources later?** Changelogs, blogs, RSS, GitHub releases could feed the same
  agent, but emails come first.
- **The agent:** which model or framework, how it decides what's interesting, and how
  it groups emails into posts.
- **Taste:** how it learns what I like (a list of companies, thumbs up/down, tags...).
- **Shape:** web app, CLI, TUI, a static page rebuilt on visit...
- **Freshness:** fetch on browse vs. a background crawl that just stays quiet.
- **Audience:** just me, or something other people could use too.

## Seed list

Companies whose updates prompted this:

- Resend
- Tailscale
