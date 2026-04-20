# HOSAKA — Operator Manual

```
  ██╗  ██╗ ██████╗ ███████╗ █████╗ ██╗  ██╗ █████╗
  ██║  ██║██╔═══██╗██╔════╝██╔══██╗██║ ██╔╝██╔══██╗
  ███████║██║   ██║███████╗███████║█████╔╝ ███████║
  ██╔══██║██║   ██║╚════██║██╔══██║██╔═██╗ ██╔══██║
  ██║  ██║╚██████╔╝███████║██║  ██║██║  ██╗██║  ██║
  ╚═╝  ╚═╝ ╚═════╝ ╚══════╝╚═╝  ╚═╝╚═╝  ╚═╝╚═╝  ╚═╝

      * \ _ /
       @( )@          a console-first AI field terminal.
      */\|/\*         signal steady. no wrong way.
     (@)|  /\
      \ | /(_)
       _|_/_
      [_____]
```

> _someone built a machine. something ancient woke up._
> _signal steady._

This is the operator manual for **Hosaka** — a terminal that pretends to
be a desktop, an appliance that pretends to be a console, and a story
that pretends to be a manual. You are the operator. There is no wrong
way to read this.

---

## what hosaka is, in three sentences

1. A **web desktop** at `terminal.hosaka.xyz` — a touchable retro
   terminal in your browser, talking to a sandboxed AI agent.
2. A **Raspberry Pi appliance** — the same shell, running on a real
   cyberdeck, served from `:8421`, controllable from your phone.
3. A **single-file Python client** called `hosakactl` — drives the
   appliance from your laptop without a single dependency.

All three layers share one philosophy and one mood. This manual is
how you tour them.

---

## table of contents

| # | chapter | what's inside |
|---|---|---|
| 01 | [welcome](docs/01-welcome.md) | what hosaka is, why it exists, what to expect |
| 02 | [the three faces](docs/02-three-faces.md) | hosted vs appliance vs docker — pick your path |
| 03 | [quickstart](docs/03-quickstart.md) | feel the signal in under five minutes |
| 04 | [accounts you'll need](docs/04-accounts.md) | every service, why it matters, what to set |
| 05 | [the hosted terminal](docs/05-the-hosted-terminal/README.md) | the browser experience, panel by panel |
| 06 | [the appliance](docs/06-the-appliance/README.md) | install on a Pi, run it forever |
| 07 | [the laptop client (hosakactl)](docs/07-the-laptop-client/README.md) | drive a remote pi from your terminal |
| 08 | [the docker edition](docs/08-the-docker-edition.md) | run the whole stack on your mac |
| 09 | [lore](docs/09-lore/README.md) | the cascade, the orb, the plant, the long quiet |
| 10 | [reference](docs/10-reference/README.md) | env vars, ports, api, glossary, troubleshooting |

---

## the operator's motto

> **NO WRONG WAY.**
>
> You can't really break this experience by experimenting.
> If a command fails, Hosaka redirects — it does not punish.

If you read nothing else, read [the no-wrong-way manifest](docs/09-lore/01-the-no-wrong-way-manifest.md).

---

## hosting this manual on github pages

This directory is a self-contained Jekyll site.

```bash
# from the repo root
git add hosaka_manual
git commit -m "manual: signal steady"
git push

# in github → settings → pages:
#   source: deploy from a branch
#   branch: main / hosaka_manual
```

GitHub Pages will serve it. Or run it locally:

```bash
cd hosaka_manual
bundle init && bundle add jekyll jekyll-relative-links jekyll-titles-from-headings
bundle exec jekyll serve
# → http://127.0.0.1:4000
```

---

> _the shape of what matters is clear. the details compress well._
> _signal steady._
