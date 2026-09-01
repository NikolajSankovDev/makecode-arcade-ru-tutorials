# MakeCode Arcade tutorials in Russian

Russian learner-facing MakeCode Arcade material for Neuronka. This repository
is the separate publishing project used by the Arcade course; it is not the
course-planning repository.

## Student links

Students only open the assigned link. There is nothing to install, clone, or
configure. `lang=ru` selects Russian tutorial text, and `lockedEditor=1` keeps
the learner in the lesson flow.

| Material | What it contains | Pinned learner link |
|---|---|---|
| Full of Stories | Four short creative activities in one Skillmap | [Open Skillmap](https://arcade.makecode.com/--skillmap?lang=ru&lockedEditor=1#github:NikolajSankovDev/makecode-arcade-ru-tutorials/skillmaps/full-of-stories#v0.1.1) |
| Chase the Pizza | Standalone guided game tutorial | [Open tutorial](https://arcade.makecode.com/?lang=ru&lockedEditor=1#tutorial:https://github.com/NikolajSankovDev/makecode-arcade-ru-tutorials/tutorials/chase-the-pizza#v0.1.1) |

## Repository layout

```text
tutorials/                         standalone tutorials
skillmaps/<skillmap>.md            a Skillmap's Russian map
skillmaps/<skillmap>/              that Skillmap's canonical tutorial sources
_locales/ru/<same-relative-path>   matching Russian tutorial views
```

For example, `skillmaps/full-of-stories/greeting-card.md` is the canonical
source and `_locales/ru/skillmaps/full-of-stories/greeting-card.md` is what a
student sees with `lang=ru`. The five Full of Stories files are intentional:
one map and four separate activities, not duplicate versions.

See [AGENTS.md](AGENTS.md) before changing course content or links.

## Source and license

The canonical English tutorials come from Microsoft MakeCode Arcade's
[`pxt-arcade`](https://github.com/microsoft/pxt-arcade) repository under the
MIT licence. This repository retains the upstream MIT licence and contains
modified Russian localizations. MakeCode Arcade and related marks remain the
property of their respective owners.
