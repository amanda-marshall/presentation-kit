## Version 0.4

### Features

#### Random Indices `randomIndex(int count)`
- Produces a random index between `1` and `count`
- Is non-repeating

#### Theming `setTheme(string themeId)`
- Introduce basic theming functionality
- Theme can be set via `setTheme` as either `light` or `dark`
- Previously, every trial type just had a default theme

#### Empty Responses
- Empty string variables can now be provided as triggerNames (`""`)

#### Trigger templates `initTriggerTemplates`
- Takes a three-dimensional string array of trigger templates, and flattens it out into a list of permutations separated by an underscore.
  - *Input*: { { {"trial"}, {"repetition", "alternation"}, {"go", "nogo"} } }
  - *Output*: { "trial_repetition_go", "trial_repetition_nogo", "trial_alternation_go", "trial_alternation_nogo" }
