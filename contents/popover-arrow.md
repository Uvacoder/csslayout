---
layout: layouts/post.njk
title: Popover arrow
description: Create a popover arrow with CSS
keywords: css arrow, css popover
---

## HTML

```html
<div class="popover-arrow">
    <!-- The content -->
    ...

    <!-- Top left arrow -->
    <div class="popover-arrow__arrow popover-arrow__arrow--tl"></div>

    <!-- Top center arrow -->
    <div class="popover-arrow__arrow popover-arrow__arrow--tc"></div>

    <!-- Top right arrow -->
    <div class="popover-arrow__arrow popover-arrow__arrow--tr"></div>

    <!-- Right top arrow -->
    <div class="popover-arrow__arrow popover-arrow__arrow--rt"></div>

    <!-- Right center arrow -->
    <div class="popover-arrow__arrow popover-arrow__arrow--rc"></div>

    <!-- Right bottom arrow -->
    <div class="popover-arrow__arrow popover-arrow__arrow--rb"></div>

    <!-- Bottom left arrow -->
    <div class="popover-arrow__arrow popover-arrow__arrow--bl"></div>

    <!-- Bottom center arrow -->
    <div class="popover-arrow__arrow popover-arrow__arrow--bc"></div>

    <!-- Bottom right arrow -->
    <div class="popover-arrow__arrow popover-arrow__arrow--br"></div>

    <!-- Left top arrow -->
    <div class="popover-arrow__arrow popover-arrow__arrow--lt"></div>

    <!-- Left center arrow -->
    <div class="popover-arrow__arrow popover-arrow__arrow--lc"></div>

    <!-- Left bottom arrow -->
    <div class="popover-arrow__arrow popover-arrow__arrow--lb"></div>
</div>
```

## CSS

```css
.popover-arrow {
    /* Border */
    border: 1px solid #d1d5db;

    /* Used to position the arrow */
    position: relative;
}

.popover-arrow__arrow {
    /* Size */
    height: 0.5rem;
    width: 0.5rem;

    background-color: #fff;
    position: absolute;
}

.popover-arrow__arrow--tl {
    /* Position at the top left corner */
    left: 1rem;
    top: 0;

    /* Border */
    border-left: 1px solid #d1d5db;
    border-top: 1px solid #d1d5db;
    transform: translate(50%, -50%) rotate(45deg);
}

.popover-arrow__arrow--tc {
    /* Position at the top center */
    left: 50%;
    top: 0;

    /* Border */
    border-left: 1px solid #d1d5db;
    border-top: 1px solid #d1d5db;
    transform: translate(-50%, -50%) rotate(45deg);
}

.popover-arrow__arrow--tr {
    /* Position at the top right corner */
    right: 1rem;
    top: 0;

    /* Border */
    border-left: 1px solid #d1d5db;
    border-top: 1px solid #d1d5db;
    transform: translate(-50%, -50%) rotate(45deg);
}

.popover-arrow__arrow--rt {
    /* Position at the right top corner */
    right: 0;
    top: 1rem;

    /* Border */
    border-right: 1px solid #d1d5db;
    border-top: 1px solid #d1d5db;
    transform: translate(50%, 50%) rotate(45deg);
}

.popover-arrow__arrow--rc {
    /* Position at the right center */
    right: 0;
    top: 50%;

    /* Border */
    border-right: 1px solid #d1d5db;
    border-top: 1px solid #d1d5db;
    transform: translate(50%, -50%) rotate(45deg);
}

.popover-arrow__arrow--rb {
    /* Position at the right bottom corner */
    bottom: 1rem;
    right: 0;

    /* Border */
    border-right: 1px solid #d1d5db;
    border-top: 1px solid #d1d5db;
    transform: translate(50%, -50%) rotate(45deg);
}

.popover-arrow__arrow--bl {
    /* Position at the bottom left corner */
    bottom: -0.5rem;
    left: 1rem;

    /* Border */
    border-bottom: 1px solid #d1d5db;
    border-right: 1px solid #d1d5db;
    transform: translate(50%, -50%) rotate(45deg);
}

.popover-arrow__arrow--bc {
    /* Position at the bottom center */
    bottom: -0.5rem;
    left: 50%;

    /* Border */
    border-bottom: 1px solid #d1d5db;
    border-right: 1px solid #d1d5db;
    transform: translate(-50%, -50%) rotate(45deg);
}

.popover-arrow__arrow--br {
    /* Position at the bottom right corner */
    bottom: -0.5rem;
    right: 1rem;

    /* Border */
    border-bottom: 1px solid #d1d5db;
    border-right: 1px solid #d1d5db;
    transform: translate(-50%, -50%) rotate(45deg);
}

.popover-arrow__arrow--lt {
    /* Position at the left top corner */
    left: 0;
    top: 1rem;

    /* Border */
    border-bottom: 1px solid #d1d5db;
    border-left: 1px solid #d1d5db;
    transform: translate(-50%, 50%) rotate(45deg);
}

.popover-arrow__arrow--lc {
    /* Position at the left center */
    left: 0;
    top: 50%;

    /* Border */
    border-bottom: 1px solid #d1d5db;
    border-left: 1px solid #d1d5db;
    transform: translate(-50%, -50%) rotate(45deg);
}

.popover-arrow__arrow--lb {
    /* Position at the left bottom corner */
    bottom: 1rem;
    left: 0;

    /* Border */
    border-bottom: 1px solid #d1d5db;
    border-left: 1px solid #d1d5db;
    transform: translate(-50%, -50%) rotate(45deg);
}
```

{% demo %}
{% include "covers/popover-arrow.njk" %}
{% enddemo %}
