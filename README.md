# Mask Shift

A turn-based card combat game built for a game jam, where switching masks changes how your cards behave.

## What it does

Fight through turn-based encounters using a deck of cards. Each card belongs to a mask (Comedy, Mystery, Drama, or Fear) and the mask you're wearing changes how your cards resolve: the same card can heal, poison, or hit harder depending on which mask is active. Status effects like poison and thorns, plus mask-specific modifiers, add extra layers to each turn's decisions.

## Why it's structured this way

Cards are implemented as ScriptableObjects grouped by mask, so new cards and mask effects can be added without touching the combat logic. The `CombatManager` and `TurnManager` stay mask-agnostic while each mask's cards define their own behavior.

## Tech

`Unity` `C#` `ScriptableObjects` `Turn-Based Combat` `Game Jam`
