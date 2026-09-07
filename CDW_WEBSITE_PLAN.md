# Callaway Data Watch Website — Plan & Reference

This document explains what this website is, how it's built, and what's
planned next. Written so anyone (a developer picking this up later, a
volunteer, a board member) can understand the whole picture without
needing to already know web development.

---

## WHAT THIS WEBSITE IS

This is the main public website for Callaway Data Watch (CDW), separate
from the Sunshine Archive project (that's a different site, aka a subdomain, a document
search tool, living in its own separate repository). This site is the
organization's front door: who we are, what we're doing, and how to
get involved or reach us.

**Planned final structure: three pages, built one at a time.**

| Page | Purpose | Status |
|---|---|---|
| Home | Who we are, mission, contact, links | Built |
| Take Action | How someone can take action and what we need help with now | Built |
| Videos | Embedded TikTok/YouTube content | In Construction |

---

## WHERE THIS LIVES

Same approach as the Sunshine Archive: a GitHub repository, hosted for
free through GitHub Pages, connected to our own domain.

- **Repository:** a new, separate GitHub repo from the Sunshine Archive
  (repo name: `callawaydatawatch-site`), inside the
  CallawayDataWatch GitHub page
- **Domain:** the bare root domain, `callawaydatawatch.org` (no
  subdomain prefix), which is different from the archive's
  `archive.callawaydatawatch.org`
- **Hosting:** GitHub Pages, exactly like the archive, free, no hosting
  costs

**Why a separate repository instead of adding this to the Sunshine
Archive repo:** these are two different tools serving two different
purposes. The archive is a searchable document database. This site is
an organizational homepage. Keeping them separate means a change to
one can never accidentally break the other, and each can eventually
have different people working on it without stepping on each other's
work.

---

## FILE STRUCTURE (same pattern as the archive, kept simple)

```
callawaydatawatch-site/
├── README.md
├── index.html          <- Home page (Phase 1, building now)
├── our-work.html        <- Get Involved / Our Work page (Phase 2)
├── videos.html          <- Videos page (Phase 3)
├── style.css            <- Shared styling for all pages
└── assets/
    └── CDW_Logo-04.png          <- CDW logo (reuse the one from the archive project)
```

Every page uses the same `style.css` file, so the whole site looks
consistent, and updating a color or font once updates it everywhere.

---

## PHASE 1: HOME PAGE (building today)

**What it includes:**

1. **Logo** at the top
2. **About section** — a short paragraph explaining who Callaway Data
   Watch is
3. **Mission statement** — a distinct, short statement of purpose
4. **Contact information** — email address and a link to our public
   Facebook group
5. **Navigation** — simple links at the top to the other two pages
   (even before they're built, we can show them as "coming soon" or
   just build placeholder pages)

**Content used (as provided):**

> Callaway Data Watch is a community organization focused on
> transparency and accountability in local government. We track what's
> happening in our county, give people a safe place to bring
> information forward, and help connect residents to the meetings and
> decisions that affect them. We then push for outcomes that reflect
> what this community actually wants.

Mission statement (written to match the tone and content of the above):

> Our mission is to make local government open, honest, and answerable
> to the people it serves, by tracking public decisions, protecting
> the people who come forward with information, and turning community
> concern into real, organized action.

**Contact info:**
- Email: callawaydatawatch@gmail.com
- Facebook: the CDW public Facebook group

---

## PHASE 2: TAKE ACTION PAGE (built)

**What it includes:**

1. A bold, full-width banner at the top calling people to act now
2. A short summary of what Callaway Data Watch is actively working on
3. Six numbered action cards laying out specific ways to get involved:
   organizing, showing up to sit-ins, going door to door, raising a
   banner, joining the No More Dirty Data Centers coalition, and
   helping fund legal counsel through Preserve Callaway County
   Missouri LLC
4. A closing call-to-action box with contact info and the Facebook
   group link

**Design note:** this page is intentionally more visually bold than
the Home page, meant to stand out and drive real action, not just
inform.

---

## PHASE 3: VIDEOS PAGE (In Construction)

Will display embedded TikTok and/or YouTube videos. Both platforms
provide a simple "embed code" (a small snippet of HTML) for any public
video, which can be pasted directly into this page without needing any
video hosting of our own. When you're ready to build this page, gather
the links to the specific videos you want featured and we'll generate
the embed codes for each one.

---

## HOW TO ADD OR UPDATE CONTENT LATER

Since this site follows the exact same GitHub workflow as the Sunshine
Archive:

1. Make changes to the relevant `.html` file
2. Never edit directly on the live `main` branch — create a new branch,
   commit your change, push it, then open a pull request and merge it
   (see the Sunshine Archive's branch/PR workflow, which applies here
   identically)
3. Changes go live at callawaydatawatch.org within a couple of minutes
   of merging

---

## THINGS TO DECIDE LATER (not blocking today's build)

- Additional pages can be added later as needed
- Pull request rules should be applied to this new repo the same way they are on the Sunshine
  Archive. This means not pushing new data to the main branch. (*reach out to Danielle Lawson or IT dept. if you have any questions on how to accomplish this)
