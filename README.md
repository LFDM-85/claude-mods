# claude-mods

Two Claude Code mods, forked from MIT-licensed originals:

- **glowup-plus** — [glowup](https://github.com/NovusEdge/glowup) by Aliasgar Khimani, plus two pane tabs:
  - **Tokens**: every model request with its cache reads, cache writes, uncached input and output, newest first, and the session's cache hit rate.
  - **Flow**: the last turn as a diagram — your prompt, each request with its context bar, the tools it ran, the answer.
- **clean-view-plus** — Clean View by schmas, plus sub-steps: `plan_steps` takes optional `substeps`, `report_progress` an optional `substep`, and the active step unfolds its sub-steps and the last actions actually done.

The tabs add no model calls. The sub-step schema and instruction add about 130 tokens to the cached prompt prefix.

## Install

```
/plugin install glowup-plus --marketplace LFDM-85/claude-mods
/plugin install clean-view-plus --marketplace LFDM-85/claude-mods
```

Answer `y` to add the marketplace, then pick a scope. Disable the original glowup / clean-view if you have them: both register the same commands and pane.

## License

MIT, as the originals; each mod keeps its upstream `LICENSE`/author.
