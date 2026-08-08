# Team Ups

**Turning uncertainty into social participation**

## Problem

During early user research, we repeatedly heard that users who were interested in sports picks did not always feel knowledgeable enough about soccer to confidently create their own tickets.

Users described two common workarounds:

- Leaving TBG to research lines and players elsewhere
- Finding successful users and copying their picks

Both behaviors represented an opportunity.

If users were already looking to other users for guidance, we could bring that behavior inside the product and make it part of TBG's community experience.

---

## Hypothesis

Instead of simply allowing users to copy another person's ticket, I wanted the interaction to feel collaborative.

The hypothesis was:

> If joining another user's ticket creates value for both the creator and the participant, users will be more willing to share, discover other users, and remain inside the TBG ecosystem.

---

## Product Concept

I proposed the feature initially as **Bet Backing**, which eventually became **Team Ups**.

A user could publish or share a ticket. Other users could then join that ticket.

Each additional participant increased the profit multiplier for everyone already participating.

This created two-sided incentives:

**Creator**
- Share successful or interesting tickets
- Attract more backers
- Increase the potential payout for the group
- Build social credibility

**Participant**
- Discover tickets from other users
- Participate without needing to originate every pick
- Benefit from the same growing multiplier
- Find creators worth following

<p align="center">
  <img src="../assets/product/TBG-teamups.PNG" width="38%" />
</p>

---

## Product Design

The original PRD covered:

- A dedicated Team Ups discovery surface
- Ticket sharing from submission and history
- In-app sharing
- External sharing
- Deep links back into the ticket
- Backer counts
- Limited available spots
- Incremental multiplier boosts
- Creator identity and social proof
- Clear loading, failure, and success states

The feature evolved from a sharing mechanic into a broader social layer within the app.

---

## Technical & Implementation Considerations

Although I did not write the production implementation, I worked with engineering through implementation implications including:

- Creating per-user ticket history for participants
- Associating all participants with the same Team Up
- Updating adjusted payouts as new users joined
- Handling wager differences between users
- Locking tickets after relevant events began
- Applying existing void behavior consistently
- Configurable participation caps
- Minimum participation amounts
- Deep-link routing
- Feature flags for rollout and tuning

The goal was to define the product deeply enough that engineering edge cases were addressed before launch rather than discovered only after users encountered them.

---

## Positioning & Launch

I also helped position and market the shipped feature.

<p align="center">
  <img src="../assets/launch/TBG-Ad-teamup.png" width="75%" />
</p>

The language evolved away from "Bet Backing" toward **Team Ups** because the latter better reinforced TBG's positioning as a community of sports fans rather than a purely transactional picks product.

---

## Results

Team Ups reached substantial participation across the user base.

A cohort analysis specifically comparing users who joined another person's ticket against bettors who never joined a Team Up showed:

<p align="center">
  <img src="../assets/analytics/team-ups-cohort.png" width="80%" />
</p>

Key observations included:

- **13.7 average active days vs. 5.0**
- **9.1% deposit rate vs. 7.6%**
- **$12.17 deposited per user vs. $10.56**
- **12.1% active in the most recent 14 days vs. 10.8%**

The largest difference appeared in sustained engagement.

---

## Analytical Limitation

This comparison demonstrates **correlation, not causation**.

Highly engaged users may be more likely to discover and participate in social functionality in the first place.

A stronger causal analysis would compare behavior immediately before and after a user's first Team Up or use an experimental holdout.

Even with that limitation, the results showed that Team Ups became strongly associated with some of TBG's most engaged users and validated continued investment in social features.

---

## What I Learned

The original problem sounded like:

> "Some users don't know enough about soccer."

The higher-leverage opportunity was:

> "Users already want guidance from other users. How do we turn that behavior into a product advantage?"

Team Ups transformed an off-platform workaround into an in-product social mechanic aligned with TBG's broader community strategy.