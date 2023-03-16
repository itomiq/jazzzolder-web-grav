---
title: Kalender
process:
  markdown: true
  twig: true
twig_first: true
never_cache_twig: true
next:
  items: "@self.children"
  dateRange:
    start: "-1day"
  order:
    by: date
    dir: asc
  limit: 1
  pagination: false
upcoming:
  items: "@self.children"
  dateRange:
    start: "-1day"
  order:
    by: date
    dir: asc
  limit: 25
  pagination: true
past:
  items: "@self.children"
  dateRange:
    start: "-5month"
    end: "-1day"
  order:
    by: date
    dir: desc
  limit: 6
  pagination: false
---

## Kalender

Hier vind je het overzicht van de aankomende en bevestigde optredens.

Standaard werken we met 2 sets per optreden. De eerste set start om {{ site.events.starttime|e }} (deuren om {{ site.events.doors }}), de tweede start op {{ site.events.starttime_set2 }} (deuren om {{ site.events.doors_set2 }}). Als je zeker wil zijn van een plaatsje, koop dan uw ticket vooraf en online via onze ticketshop. We hebben **geen** genummerde plaatsen, dus kom ook zeker op tijd.

<a class="btn-primary my-4 inline-block text-center mx-auto" href="{{ site.ticketshop.url }}">Naar de ticketshop</a>

![51052452841_d70e324de7_h](51052452841_d70e324de7_h.jpg "51052452841_d70e324de7_h")
