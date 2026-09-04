# Watercolor Memory Poster

A reusable image-generation Skill for turning uploaded photographs into high-end 3:4 editorial posters with a strict 50/50 split:

- **Top half:** faithful original photograph with subtle editorial grading.
- **Bottom half:** a small, airy watercolor-memory interpretation with strong negative space.
- **Human subjects:** preserve identity, expression, pose, relationships, and movement; use controlled watercolor motion blur to emphasize dynamic gesture.
- **Typography:** exactly one short English title line; no year, subtitle, or extra caption.

## Core concept

> Reality above. Memory below.

The photograph records what happened. The watercolor preserves how the moment felt.

## Structure

```text
watercolor-memory-poster/
├── SKILL.md
├── agents/
│   └── openai.yaml
└── references/
    └── art-direction.md
```

## Usage

Use this Skill when you want to transform a photo into the established watercolor-memory editorial style. It works especially well for:

- travel photography
- sports and movement
- family or candid moments
- portraits with expressive body language
- quiet landscapes and environmental scenes

For multiple uploaded photos, generate **one independent poster per photo**. Never combine them into a collage.

## Visual direction

The lower watercolor should not be a full painted copy of the photo. It should isolate the emotional center of the moment, keep the illustrated subject relatively small, preserve essential gesture and expression, and let unnecessary detail dissolve into paper, pigment, motion, and empty space.

The final result should feel like **a memory that is still moving**.
