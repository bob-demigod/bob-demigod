# esclear

Marketplace payments for a physical-goods handoff. The buyer pays by card, the seller ships, and the seller is paid when the buyer confirms delivery.

This is marketplace transfers, not licensed escrow.

## Problem

Classifieds buyers and sellers do not trust a bank transfer to a stranger. The buyer wants the money held until the item arrives. The seller wants to be paid once delivery is confirmed.

## What I built

- Accounts, a dashboard, and a deal page for buyer and seller
- A status path from created, through funded and shipped, to delivered and released, with cancel and dispute branches
- Card payment by the buyer into the platform account
- Carrier and tracking on the shipment, with an activity log
- Payout to the seller after the buyer confirms delivery
- An admin view for a paused deal: refund the buyer, or release to the seller
- A post-quantum signature on each deal event, and a check that the history still matches

## Stack

React, FastAPI, MongoDB, Stripe Checkout and Connect, Docker.

## Status

Private product. An earlier mobile package used another name. This page does not include hosts, account names, or payment configuration.
