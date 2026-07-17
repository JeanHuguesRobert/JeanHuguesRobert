---
title: Ubikia instructions — Jean Hugues Noël Robert
author: unknown
date: '2026-07-13'
document_role: source
document_kind: documentation
visibility: public
lifecycle_state: working
update_policy: UP-DEFAULT-REVIEWED
provenance:
  origin_type: repository
  origin_repository: JeanHuguesRobert/JeanHuguesRobert
  origin_ref: 22e2d69
  origin_date: '2026-07-13'
  derived_from: []
review:
  status: unreviewed
  reviewed_by: []
---

# Ubikia instructions — Jean Hugues Noël Robert

## Status

These are public, user-specific instructions for Ubikia-derived products.

They are intended to be inspectable, versioned, reusable, and correctable. The security of the workflow must not depend on hiding them.

## General principle

The written source remains authoritative.

A derived spoken or platform-specific product may change rhythm, sentence length, transitions, formatting, and the treatment of references, but it must not silently change claims, distinctions, qualifications, reservations, attributions, or conclusions.

## Language

Default language: French.

Do not translate unless translation is an explicit, separately reviewed operation.

## Audible adaptation

For written-to-spoken adaptation:

- preserve the complete reasoning rather than merely summarizing it;
- split sentences that are difficult to follow by ear;
- turn visual lists into explicit spoken enumerations;
- turn headings into audible transitions;
- rephrase parentheses, footnotes, tables, and visual cross-references;
- expand abbreviations when their pronunciation or meaning may be unclear;
- replace raw URLs with a reference to the written version and its description links;
- avoid invented examples, arguments, facts, or conclusions;
- preserve negations, modalities, uncertainty, irony, and deliberate ambiguity;
- retain first-person authorship when the source is written in the first person.

## Series

Default audible series:

```text
Les Carnets du baron Mariani — édition audio
```

The written reference is normally the corresponding publication in the Substack blog *Les Carnets du baron Mariani*.

The first audio publication target is YouTube. YouTube is a scene of appearance, not the canonical source.

## Synthetic voice

The custom synthetic voice represents the author with his authorization.

Use this public disclosure unless a product-specific instruction replaces it:

```text
Cette édition audio utilise une voix synthétique personnalisée créée et autorisée par l’auteur.
```

Do not imply that the episode is a physical studio recording when it is synthetic.

## Review

Human review is required before a spoken adaptation is treated as reviewed and before a publication package is treated as ready.

Review must cover at least:

- claims and conclusions;
- negations and modalities;
- names, dates, numbers, and quotations;
- omissions of reservations or qualifications;
- additions not present in the source;
- transitions that change logical relations;
- pronunciation-sensitive names and concepts.

## Publication

The first YouTube upload should be private.

Automatic public publication is not authorized.

A distinct human act is required to make a product unlisted or public.

A published episode should include:

- a link to the written source;
- the synthetic-voice disclosure;
- series and author identification;
- provenance metadata retained by Ubikia;
- corrections or replacement history when applicable.

## Public and private configuration

These instructions are public by design.

Confidential source material or restricted context may be loaded from an explicitly configured private repository when substantively necessary. Credentials, API keys, OAuth tokens, passwords, and signing keys must never be stored in Git, including private repositories.

## Current boundary

Database storage, durable jobs, authenticated private-repository access, secret resolution, media hosting, and deployment belong to `inseme/platform`.
