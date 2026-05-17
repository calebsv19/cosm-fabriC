# kit_ui Roadmap

`kit_ui` is currently a shared immediate-mode control layer on top of `kit_render`.

## Implemented Now

- stack layout helpers
- clip-stack helpers
- label, button, checkbox, slider, scrollbar, and segmented control drawing
- simple input evaluation helpers
- theme-scale style sync
- text measurement and text-fit helpers
- validation harness coverage for live Vulkan-backed checks

## Deferred

1. keyboard focus and navigation helpers
2. retained row/list helpers for higher-level inspectors
3. settings/action binding adapters
4. richer text input or editor controls
5. host-specific event-loop, pane, or persistence behavior

## Hardening Notes

- Version `0.8.1` truth-locks the immediate-mode ownership boundary and expands invalid-arg, clip-stack, and text-fit edge coverage.
- Large-file decomposition is still deferred because the current pass only touches existing helper lanes rather than adding a new subsystem.
