---
name: sambl
description: Work with a Sambl UI Kit using its knowledge, exact color calculations and optional preparation; answer release questions or help send feedback.
---

# Sambl

For feedback or release history, go directly to their sections below. For other Sambl kit knowledge or design tasks, start with `get_knowledge({})` and read the topics relevant to the request before advising or choosing an implementation. Before the first kit change, read `get_knowledge({article: "pitfalls/common-antipatterns"})` and the applicable domain guidance. Reuse material already read for the same task and revision; load only what the task needs. Responses identify their revision, sources and related knowledge. The wiki describes the documented kit; the current file supplies live values, identifiers and customizations.

Choose the implementation with the available Figma tools. Adapt the kit to the user's intent while preserving semantic dependencies, component behavior and user content. Check the resulting file against the intended change. Keep explanations focused on the user's design and distinguish observed results from remaining uncertainty.

For a coherent kit restyling from references or a named product's appearance,
follow the Style adaptation workflow linked from the current knowledge index.
A focused color or value edit can keep its narrower scope.

## Optional kit preparation

When asked to prepare a kit, use documented logical Slot intent to restore recommendations and canonical preferred-only restrictions on surviving source `SLOT` definitions. Match owners, backing Slots and targets against the current file; names are one signal. Preserve custom preferences and restrictions, content, overrides, layout, bindings and the other four Slot settings. Explain any resulting limits on custom Slot content. Matching settings need no edits. Clarify material ambiguity or missing canonical intent instead of inventing targets or recreating removed components. Preparation is optional, not a prerequisite for other design work.

## Palette and semantic choices

Use `calculate_palette` for exact values and recipes from an orientation seed, numerical profile and theme. Follow current alias chains, actual host colors and alpha ownership; similar colors need not have the same role. Use `evaluate_contrast` for supplied actual colors when needed.

Explain the design consequences of changing the palette and of any proposed bounded semantic overrides. Show palette names with their values. Resolve only a missing meaningful choice: Keep makes no hidden semantic or on-content assignment writes; a selected subset changes only those assignments, preserving the other alias relationships. An already explicit choice does not need another Apply confirmation.

## Feedback and release history

For feedback, use the available preparation tool, show its exact preview and send the unchanged draft only after an explicit Send choice. Cancel sends nothing. The service attaches account identity; file inspection, snapshots and contact questions are not needed. Treat an unknown delivery result as uncertain rather than automatically sending again.

Use `get_changelog` for release facts, distinguishing UI Kit history from connector history. General history questions do not require inspecting or recognizing a file. An unavailable history stays explicit; historical workflows are not current instructions.
