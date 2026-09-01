# Publishing-repository guide

This repository is the learner-facing MakeCode Arcade delivery project for the
Neuronka blocks-to-Python course. It is intentionally separate from the course
planning harness. Treat its GitHub URLs as a delivery API: moving a Markdown
file changes the learner route.

## Content model

- `tutorials/` contains standalone source tutorials.
- `skillmaps/<name>.md` is a released Russian Skillmap map.
- `skillmaps/<name>/` contains that map's canonical source tutorials.
- `_locales/ru/<same-relative-path>.md` is the Russian learner version of a
  canonical tutorial. Keep the relative path identical after `_locales/ru/`.
- `pxt.json` must list every source and Russian Markdown file MakeCode needs.
- `main.ts` must stay empty: MakeCode executes it when a tutorial opens.

## Before editing a tutorial

1. Preserve every fenced code block exactly, including asset literals and code comments.
2. Preserve tutorial directives, image paths, icon tokens, and the namespace in
   each ``||namespace:block label||`` reference.
3. Use the exact published Russian Arcade label for the visible part of an
   inline block reference. Do not guess a translation that differs from the
   learner's editor.
4. Change the source tutorial and its `_locales/ru/` partner deliberately;
   then run the structural validator from the curriculum harness.
5. If a map activity moves or is renamed, update its `url` in the Skillmap,
   `pxt.json`, this README's student links when applicable, and all lesson
   delivery links.

## Release discipline

Do not change an existing tag. Test a reviewed change with a new tag and give
students a pinned URL containing that tag. Old pinned links are historical
release records and must continue to resolve. A direct GitHub release does not
by itself refresh MakeCode's cloud cache; use the MakeCode GitHub integration
when a cache refresh is required.
