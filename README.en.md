# Postcard Memory Poster Skill

[简体中文](README.md)

A reusable image-generation Skill that turns photographs into 3:4 editorial travel postcard-memory posters.

## Core structure

- Top half: faithfully preserve the original photograph.
- Bottom half: extract the place or human gesture into an airy watercolor memory.
- Middle: a clear 50/50 horizontal split without a heavy frame.
- Information layer: a restrained title and short divider by default; add a location or year only when requested, and use a year only when provided or confirmed.

## Two series

- Scene series: cities, rivers, nature, architecture, roads, and sunsets. Keep only 1–3 place-recognition clues; the watercolor should be medium-small, with more negative space than detail.
- People series — Watercolor Motion: movement, travel, family, and human gestures. Strictly preserve the action skeleton, center of gravity, limb directions, pose, trajectory, and relationships.

In the people series, start at 60%–75% of the normal readable figure scale. If the lower half still feels crowded, reduce below 60%. The person is a memory anchor; negative space and atmosphere are the main subject.

## How to use

1. Install this folder as the `postcard-memory-poster` Skill in your Skill directory.
2. Invoke `$postcard-memory-poster` in a Codex environment that supports Skills.
3. Attach one photograph; select the scene series or People / Watercolor Motion series, or let the Skill decide.
4. Optionally provide the title, location, year, no-text preference, or other information-layer requirements.

Example:

```text
$postcard-memory-poster
Create a Watercolor Motion people-series poster from this photo.
Make the person smaller with generous negative space; keep only one short English title and one thin divider.
```

## Public repository policy

This repository publishes only Skill rules, visual references, and usage documentation. It does not publish user-provided photographs or generated photo posters. Use images as local inputs or local outputs; do not commit them to GitHub.

See [`SKILL.md`](SKILL.md), [`references/art-direction.md`](references/art-direction.md), and [`references/art-direction-en.md`](references/art-direction-en.md) for the complete rules.
