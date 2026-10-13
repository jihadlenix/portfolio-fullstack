# Jihad Maasarani, Portfolio · Full-Stack

A single-page, scroll-driven portfolio aimed at full-stack and fintech roles. No
framework and no build step: hand-written HTML, CSS and vanilla JavaScript with
GSAP, ScrollTrigger and Lenis from a CDN.

This is a sibling of the automation portfolio and shares its design. The two are
deployed separately on purpose, so each can be pointed at a different kind of
role without one overwriting the other.

**Live:** _(added after deploy)_

## Running locally

```bash
python .claude/devserver.py 5180
```

The dev server sends `no-store` and implements HTTP Range, which the stdlib
handler does not.

## Notes

- Everything degrades: readable with JavaScript disabled, usable under
  `prefers-reduced-motion`, presentable with every video file removed.
- Animations touch only `transform`, `opacity`, `filter` and `clip-path`.
- Scenes play only while on screen and the preloader gates on real assets
  rather than a timer.

## Licence

Code is free to learn from. The photography, video, copy and CV are not.
