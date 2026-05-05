# PICC Studio Public Overview

PICC Studio is a creative operations tool for generating co-branded product and event assets from structured inputs, uploaded references, and controlled AI-generated backgrounds.

This public overview uses redacted or synthetic material only. It does not include production source code, credentials, private brand assets, customer data, live uploads, or internal business records.

## Product Problem

Field and brand teams need fast, consistent creative assets for events, product spotlights, and partner promotions. The hard part is not only generating an image; it is turning messy event details, brand constraints, product context, and export requirements into repeatable final assets.

## What The System Does

- Creates event flyer and product spotlight projects.
- Accepts structured inputs for event, partner, product, and message context.
- Uses AI-generated background art as one controlled layer in the workflow.
- Composes deterministic final layouts after generation.
- Exports square, story, and print-ready assets.
- Supports shareable review links without exposing editing access.

## Architecture Notes

- Web app shell for project creation, asset upload, review, and export.
- Server-side AI generation path so private keys are not shipped to browser code.
- Deterministic composition layer for final outputs.
- Optional object storage for uploaded references and rendered assets.
- Future-ready persistence layer for saved projects and version history.

## Data And Privacy Boundary

Public materials should use synthetic events, synthetic products, and placeholder partner names.

Do not publish:

- Real dispensary names unless explicitly approved.
- Private uploaded images.
- Product or pricing records not already cleared for public use.
- API keys, storage tokens, database URLs, or deployment metadata.
- Internal approval notes or operational instructions.

## AI Use Boundary

AI is used for creative background generation and visual exploration. Final output quality depends on product constraints, prompt design, layout composition, export rules, and review workflow, not raw generation alone.

Public demos must avoid direct client-side Gemini/API key exposure and should use rate limiting or a fixed sample mode.

## Public Materials To Add

- Redacted architecture diagram.
- Synthetic before/after asset flow.
- Screenshots with placeholder products and partners.
- Example generated background with deterministic final layout.
- Short explanation of why generation and final composition are separate.

## Suggested Public Copy

> A redacted technical overview of a creative asset workflow that combines structured product/event data, server-side AI image generation, deterministic layout composition, and reviewable exports.

