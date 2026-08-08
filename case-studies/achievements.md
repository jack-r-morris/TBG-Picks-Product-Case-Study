# Achievements

**Using status, identity, and progression to reinforce valuable behavior**

## Signal

TBG originally had a limited **Tipster** badge for selected users who shared picks and helped bring other users into the product.

As the Discord community grew, regular users began directly asking for badges they could earn themselves.

That request aligned with a broader product goal: make TBG feel like a sports community users developed identity and status within, rather than a utility they visited only to place a ticket.

---

## Product Problem

Simply adding badges to profiles would have had limited value.

Very few users actively visited other users' profile pages.

If achievements were meant to influence social behavior, they needed to appear where users were already making social decisions.

That led to two product principles:

1. Achievements should represent meaningful behaviors worth encouraging.
2. Achievements should be visible outside the profile.

---

## Achievement Design

The system expanded to recognize behaviors including:

- Sharing tickets others wanted to join
- Supporting creators through Team Ups
- Sustained activity
- Tournament participation and wins
- Creating successful tournaments
- Exploring competitions
- Trying multiple pick types
- Winning larger or more complex tickets

Examples included:

| Achievement | Behavior |
| --- | --- |
| Tipster | Consistently attract backers |
| Tycoon | Reach a major coin-winnings milestone |
| Grand | Reach a major credit-winnings milestone |
| Centurion | Complete 100 picks |
| Mainstay | Reach a 30-day activity streak |
| Wingman | Support many different creators |
| Crowd Favorite | Repeatedly create popular Team Ups |
| Champion | Win multiple tournaments |
| Host | Create successful tournaments |
| Explorer | Participate across different competitions |
| Perfect Parlay | Complete a successful multi-leg ticket |
| Invincible | Build an extended win streak |
| All-Rounder | Participate across multiple pick types |

The exact achievement catalog evolved during implementation.

---

## Status & Scarcity

Achievements were divided into visual difficulty tiers:

**Bronze → Silver → Gold → Mythic → Legendary**

The goal was to ensure that status retained meaning.

If achievements were too easy or too common, they would stop communicating anything useful.

Users could also showcase only a limited number beside their username, forcing them to choose which accomplishments best represented their identity.

<p align="center">
  <img src="../assets/product/TBG-profile.PNG" width="38%" />
</p>

---

## Moving Status Into the Social Experience

One of the most important UX decisions was making achievement showcases visible in **Team Ups and tournaments**.

<p align="center">
  <img src="../assets/product/TBG-teamups.PNG" width="38%" />
</p>

This changed achievements from hidden profile decoration into social proof.

When a user encountered someone marked as a **Champion** or **Tipster**, the status appeared at the moment they might be deciding whether to follow that user or join their ticket.

---

## Technical Collaboration

The expanded system required more than frontend badge artwork.

I worked with engineering around considerations including:

- Achievement qualification logic
- Locked vs. earned states
- Progress calculations
- User-selected showcase slots
- Achievement data surfaced in multiple product views
- Backfilling existing users
- Maintaining achievement state efficiently
- Avoiding expensive historical calculations on every profile request
- Migration and rollout sequencing

The implementation ultimately used precomputed achievement state for efficient reads while maintaining progress as relevant user events occurred.

---

## Results

Within the analyzed user base, **5.4% unlocked and displayed achievements**.

Users with badges represented an unusually high-value cohort:

<p align="center">
  <img src="../assets/analytics/achievements-cohort.png" width="78%" />
</p>

The cohort showed substantially higher:

- Deposit rate
- Deposits per user
- Average active days
- Recent activity

---

## Analytical Limitation

This is a highly selected cohort.

Several achievements are themselves earned through behaviors associated with engagement—for example sustained streaks or high activity.

Therefore:

> **The data should not be interpreted as achievements causing the entire engagement difference.**

Instead, the analysis demonstrated that the system successfully identified and surfaced many of TBG's highest-engagement users.

A stronger test of the motivational effect would compare users' behavior before and after earning their first achievement or examine behavior around achievement thresholds.

---

## What I Learned

Gamification is most useful when it reinforces behaviors the product already values.

The goal was not simply to give users decorative icons.

It was to create an identity system where:

**valuable behavior → recognition → visible status → more social context → stronger product attachment.**