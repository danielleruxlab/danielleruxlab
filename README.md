/index.md
---
layout: default
title: Welcome
---

Welcome to the Rux Lab! We study **synovial joint development and disease**, with a focus on how developmental signaling programs build and maintain articular cartilage—and how their disruption contributes to osteoarthritis.

<div class="grid">
  <div class="card">
    <img src="/assets/img/research1.jpg" alt="Synovial joint development">
    <strong>Joint patterning</strong><br/>
    How cell fates and boundaries form the synovial joint.
  </div>
  <div class="card">
    <img src="/assets/img/research2.jpg" alt="Articular cartilage zones">
    <strong>Cartilage zonation</strong><br/>
    Building postnatal architecture and lifelong tissue integrity.
  </div>
  <div class="card">
    <img src="/assets/img/research3.jpg" alt="Osteoarthritis mechanisms">
    <strong>OA mechanisms</strong><br/>
    Linking developmental pathway dysregulation to degeneration.
  </div>
</div>

/research.md
---
layout: default
title: Research
---

## Current Research Areas

### 1) Synovial joint development
<img src="/assets/img/joint-dev.jpg" alt="Joint development">

We define how signaling gradients and tissue interactions establish joint boundaries, shape the epiphysis, and specify synovial tissues.

### 2) Articular cartilage morphogenesis and maintenance
<img src="/assets/img/ac-zones.jpg" alt="Articular cartilage zones">

We study how developmental pathways build postnatal zonal architecture and how “just-right” pathway activity is required for lifelong cartilage function.

### 3) Osteoarthritis pathogenesis
<img src="/assets/img/oa.jpg" alt="OA model">

We test how perturbations in developmental programs sensitize joints to post-traumatic and age-associated osteoarthritis.

/team.md
---
layout: default
title: Team
---

## Principal Investigator
<div class="card">
  <img src="/assets/img/pi.jpg" alt="PI photo">
  <h3>Danielle Rux, PhD</h3>
  Assistant Professor • UConn Health<br/>
  Synovial joint development • Cartilage biology • Osteoarthritis
</div>

## Lab Members
<div class="grid">
  <div class="card">
    <img src="/assets/img/member1.jpg" alt="Lab member">
    <strong>Member Name</strong><br/>
    Role / Program<br/>
    1–2 sentence bio + project focus.
  </div>
</div>

/publications.md
---
layout: default
title: Publications
---

## Selected Publications
- Paper title. Authors. *Journal* (Year). [PubMed](https://pubmed.ncbi.nlm.nih.gov/...)
- Paper title. Authors. *Journal* (Year). [PubMed](https://pubmed.ncbi.nlm.nih.gov/...)

**Full list:** add a link to your Google Scholar profile.

/news.md
---
layout: default
title: News
---

## Lab News

### Jan 2026 — New preprint posted
Short blurb + optional photo.

### Oct 2025 — Welcome our new rotation student
Short blurb.

/contact.md
---
layout: default
title: Contact
---

### Lab Location
UConn Health, Farmington, CT

### Email
your.email@uchc.edu

### Prospective trainees
We welcome motivated trainees. Please email a CV and a short statement of interests.

/_config.yml
title: Rux Lab
description: Synovial joint development, articular cartilage morphogenesis, and osteoarthritis
theme: minima
markdown: kramdown

/_layouts/default.html
<!doctype html>
<html lang="en">
  <head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width,initial-scale=1" />
    <title>{{ page.title }} | {{ site.title }}</title>
    <link rel="stylesheet" href="{{ '/assets/css/style.css' | relative_url }}">
  </head>
  <body>
    {% include nav.html %}

    <main class="container">
      <h1>{{ page.title }}</h1>
      {{ content }}
    </main>

    <footer class="footer">
      © {{ "now" | date: "%Y" }} {{ site.title }}
    </footer>
  </body>
</html>


/_includes/nav.html
<nav class="nav">
  <div class="nav-inner">
    <a class="brand" href="{{ '/' | relative_url }}">{{ site.title }}</a>
    <div class="links">
      <a href="{{ '/' | relative_url }}">Home</a>
      <a href="{{ '/research' | relative_url }}">Research</a>
      <a href="{{ '/team' | relative_url }}">Team</a>
      <a href="{{ '/publications' | relative_url }}">Publications</a>
      <a href="{{ '/news' | relative_url }}">News</a>
      <a href="{{ '/contact' | relative_url }}">Contact</a>
    </div>
  </div>
</nav>

/assets/css/style.css
:root { --max: 980px; }
body { margin: 0; font-family: system-ui, -apple-system, Segoe UI, Roboto, Arial, sans-serif; line-height: 1.5; }
.container { max-width: var(--max); margin: 0 auto; padding: 24px 16px; }
.nav { border-bottom: 1px solid #e6e6e6; background: #fff; position: sticky; top: 0; }
.nav-inner { max-width: var(--max); margin: 0 auto; padding: 12px 16px; display:flex; align-items:center; justify-content:space-between; gap:16px; }
.brand { font-weight: 700; text-decoration: none; color: #111; }
.links a { margin-left: 12px; text-decoration: none; color: #333; }
.links a:hover { text-decoration: underline; }
.grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(240px,1fr)); gap: 16px; }
.card { border: 1px solid #e6e6e6; border-radius: 12px; padding: 14px; }
.footer { border-top: 1px solid #e6e6e6; padding: 16px; text-align:center; color:#666; }
img { max-width: 100%; border-radius: 12px; }

/assets/img/...

