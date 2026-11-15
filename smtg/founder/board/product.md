# Product lens
Score: 4 | Vote: FUND IF

## What is strong

The core transaction is simple enough to describe in one sentence: borrow
something nearby from someone who owns it, return it, pay per day. That
simplicity is the product's best asset — there is no explanation problem
for either side.

The escrow-held payment model is the right structural choice. It removes the
awkward moment where a renter hands cash to a stranger, and it gives the
platform a natural hold point to handle disputes before money moves. That
is a real product decision, not an afterthought.

The in-person handoff, often cited as a liability, is also a feature:
it is the moment the product owns from end to end, requires no logistics
infrastructure, and is the natural place for item inspection that protects
both sides. If designed well — with a lightweight checklist, photo capture,
or a condition-confirmation tap — it becomes a trust touchpoint rather than
a seam.

## What would kill it (top 3, most dangerous first)

**1. Damage, disputes, and no-shows have no stated resolution.**
The brief names this openly as unknown. This is not a backlog item — it is
the product. The first time a pressure washer comes back broken and both
sides tell a different story, the platform is the arbiter. Without a
documented damage policy, a deposit or insurance mechanism, and a claims
flow, the product cannot ship to real users. Every design decision that
follows (listing flow, pricing guidance, the handoff screen) depends on
knowing what the platform promises when things go wrong. This is the most
dangerous gap because it is invisible to users until the worst moment.

**2. The experience is handed between at least four parties and three
systems — and every seam is undesigned.**
The Product lens starts from the customer's first five minutes. Walk it:
a renter finds a listing, sends a request, waits for an owner to accept,
arranges a pickup time and place, meets a stranger, hands over money (or
doesn't — escrow), gets an item, uses it, returns it, waits for the owner
to confirm return, waits for the platform to release funds. That is eight
to ten discrete moments. The brief describes the transaction flow in six
steps but names no design for any of them. Seams are where it breaks: the
"owner accepts" step alone introduces an indeterminate wait that kills
conversion for time-sensitive needs ("I need a drill this afternoon").
No stated answer to: how fast must an owner respond before the request
expires? What does the renter do if no one accepts?

**3. There is nothing yet that makes this feel like one product rather
than a utility.**
The Product lens asks what you would cut until what is left is the one
thing the business must do brilliantly. Right now the answer is "a
commission on peer-to-peer rentals" — which is a revenue model, not a
product vision. Without a clear point of view on what the best possible
rental experience feels like (instant, frictionless, trusted, local,
something else?), every feature decision will be made by committee or by
default. This kills craft before the first line of code. The competitor
set includes Fat Llama, ShareTribe-powered clones, Facebook Marketplace,
and local Buy Nothing groups. None of them is excellent. That gap is real,
but only a product with a point of view can fill it.

## The questions I would ask the founder

1. Walk me through the moment an item comes back damaged. What does the
   renter see? What does the owner see? Who decides what happens, and in
   what timeframe? This is the product's hardest problem — what is your
   current thinking, even at the sketch stage?

2. What is the one experience you are optimising for in the first version:
   the owner listing something, or the renter finding something? They have
   different needs and you cannot do both brilliantly with no team and no
   budget. Which half do you believe is the bottleneck?

3. Have you done the in-person handoff yourself — borrowed something from
   a stranger, returned it, paid them? What felt broken? The Product lens
   demands you start from that experience and work back. If you have not
   done it, that is the first thing to do before writing a line of code.

4. What is the one item category you are launching with, in the one
   neighbourhood? "Tools and equipment" is still twenty subcategories.
   What do you cut?

5. If the platform took zero commission and charged a flat fee per listing
   instead, would the product work better for owners? What does that
   question tell you about where the value actually sits?

   (The right financial model question belongs to `founder-cfo`, which also
   answers unit economics and CAC — open questions this lens cannot fill.)

## If FUND IF: the conditions

**1. A damage and dispute policy must exist before any user-facing design
begins.** Not a legal document — a product decision. At minimum: who is
liable for damage, what evidence is required, what the platform covers,
what it does not, and what the resolution timeline is. This decision
shapes every other screen.

**2. The founder must name the one item category and one geography for
launch, and defend the choice.** Not "tools in a city." One type of item
(e.g. power tools) in one specific area (e.g. a single dense neighbourhood)
where supply and demand can both be seeded manually. The Product lens
requires starting small enough to own completely.

**3. A prototype of the handoff experience — the moment of physical
exchange — must be tested with real people before any backend is built.**
This is the seam most likely to fail silently. A paper prototype or a
Wizard of Oz test with five real exchanges counts. The finding from those
tests, not a deck, is what the next conversation should open with.
