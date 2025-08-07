# Css Notes

things i could forget so i will note them

## Polygon (is the way to controll the notes)

```css
/* Rectangle or square */
clip-path: polygon(
    0% 0%,     /* top-left (shifted down) */
    100% 0%,    /* top-right (at top) */
    100% 100%,  /* bottom-right */
    0% 100%     /* bottom-left */
);

/* Piramid */
clip-path: polygon(
    50% 0%,     /* top-left (shifted down) */
    50% 0%,     /* top-right (at top) */
    100% 100%,  /* bottom-right */
    0% 100%     /* bottom-left */
);
```