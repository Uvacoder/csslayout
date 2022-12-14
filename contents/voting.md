---
layout: layouts/post.njk
title: Voting
description: Create a voting control with CSS flexbox
keywords: css flexbox, css triangle buttons, css voting control
---

## HTML

```html
<div class="voting">
    <!-- Up button -->
    <button class="voting__button">
        <div class="voting__triangle voting__triangle--up"></div>
    </button>

    <!-- Number -->
    <div class="voting__number">...</div>

    <!-- Down button -->
    <button class="voting__button">
        <div class="voting__triangle voting__triangle--down"></div>
    </button>
</div>
```

## CSS

```css
.voting {
    border: 1px solid #d1d5db;
    border-radius: 0.25rem;
    display: flex;
    flex-direction: column;
    height: 8rem;
}

.voting__button {
    /* Reset */
    background: none;
    border: none;
    cursor: pointer;

    /* Center the content */
    align-items: center;
    display: flex;
    justify-content: center;

    /* Size */
    height: 1rem;

    /* Position the triangle */
    position: relative;
}

.voting__triangle {
    border-style: solid;

    /* Size */
    height: 0;
    width: 0;
}

.voting__triangle--up {
    border-color: transparent transparent #d1d5db;
    border-width: 0 0.5rem 0.5rem;
}

.voting__triangle--down {
    border-color: #d1d5db transparent transparent;
    border-width: 0.5rem 0.5rem 0px;
}

.voting__number {
    /* Take the available height */
    flex: 1;

    /* Center the number */
    align-items: center;
    display: flex;
    justify-content: center;

    /* Spacing */
    padding: 0.25rem;
}
```

{% demo %}
{% include "covers/voting.njk" %}
{% enddemo %}
