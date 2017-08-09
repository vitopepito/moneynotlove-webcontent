---
title: 'Round Table'
menu: 'Round Table'
content:
    items: '@self.children'
    order:
        by: date
        dir: desc
    dateRange:
        end: today
        field: header.date
upcoming:
    items: '@self.children'
    order:
        by: date
        dir: asc
    dateRange:
        start: today
---

<header class="banner horizontal-center" markdown="1">

## The Creative's Round Table

Events über die grössere Relevanz kreativer Arbeit in der Gesellschaft.

<br />

</header>
