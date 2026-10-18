# Visual Asset Production

## Scope and delivery mode

Propose a compact inventory with asset ID, subject/state, narrative purpose, parent reference IDs, necessity, and approval status. Include only assets with a distinct visual or continuity need. Agree on scope before generating images; a concise description is sufficient for a single explicitly requested asset. Independent props need not wait for all characters, or vice versa.

Support prompt-only delivery and image generation with available tools. If the mode is unclear, clarify it before image generation. Inspect actual reference images before relying on their visual contents, identify each reference's role, and adapt notation and output settings to the target tool. Do not invent reference inputs or promise unsupported resolutions.

## Character masters

Use the approved script interpretation and creative brief. Describe observable features that matter to identity: age presentation, face, hair, build, posture, clothing layers, materials, wear, and distinctive details. Do not infer fixed facial anatomy, personality, or appearance from nationality or ethnicity. Use script-specific characterization and approved visual references.

A useful master is a single character in a readable, relaxed pose, with sufficient coverage to show the required costume and footwear. Use a neutral background and lighting that preserve form and intrinsic color. Portrait orientation, often 9:16, is a practical starting point for full bodies; adapt to the subject and tool. A portrait-only request does not require a full-body image.

Translate the brief into visible properties. Avoid vague quality claims and long negative-prompt lists. Include exclusions only for likely, consequential errors.

## Dependencies and variants

Generate independent masters first. A state variant uses the approved revision of the same character as its parent. Preserve identity and stable anatomy; change only the agreed costume, injury, age, or transformation features. Track each narratively distinct state separately to avoid importing a later injury or transformation into an earlier scene.

For relatives, resemblance is a design choice rather than a deterministic biological formula. When likeness is requested, agree on a few shared features while preserving individual identities. Do not create otherwise unnecessary parents just to generate a child. If both approved parents are designated references, wait for both or obtain agreement to relax that dependency.

Clarify transformation degree only when the script and brief leave a consequential ambiguity. Describe visible changes; percentage labels alone do not define a usable design.

If planned dependencies form a cycle, select a shared approved design brief or a base master with the user rather than waiting indefinitely.

## Character sheets

Create sheets only when requested or useful for a stated downstream need. Build them from approved masters. Choose front, back, profile, face detail, or costume detail according to the information still missing; do not force a headless view or a fixed panel layout.

A new angle may introduce details absent from the master. Label these as proposed design decisions for review, not recovered facts. Check panel-to-panel identity, proportions, costume construction, hair, footwear, and left/right details. Read left and right from the character's perspective unless specified otherwise; back views do not swap anatomical sides.

Keep labels minimal. Prefer editable text outside the generated image when exact names or measurements matter. Do not invent a height to fill a sheet.

## Key props

Prioritize objects with distinctive construction, recurring use, meaningful transfer or damage, identity clues, or important handling requirements. Ordinary incidental objects can remain text descriptions.

Describe silhouette, relative or confirmed scale, construction, materials, intrinsic color, wear, functional contact points, asymmetry, and current story state. Do not claim exact dimensions unless supplied or approved.

A single-object neutral-background reference with a clear identifying angle is usually sufficient. Choose aspect ratio to keep the complete object readable; 3:4 is a useful option, not a requirement. Add views or handling context only when the requested use needs them. If grip fit or proportions depend on a character, use that approved character reference or establish the relevant dimensions first. Prop states may depend on an intact parent or earlier state.

Separate reference roles: a layout reference informs framing and lighting; a design reference informs the object's form. Do not transfer unrelated logos, text, ornaments, or materials from a layout example. Preserve story-critical markings; verify legibility rather than assuming a generator rendered them accurately.

## Prompt assembly

Write a self-contained prompt from the current record, covering only applicable elements:

1. Deliverable and subject/state.
2. Actual reference inputs and the features each should preserve.
3. Stable identity or construction details.
4. Agreed changes from parent assets, if any.
5. Pose/view, framing, lighting, background, and relevant style.
6. Critical exclusions and requested output settings supported by the tool.

Do not leave empty fields or template placeholders in delivered prompts. For external tools, map reference names to the actual files the user must attach. If a required reference is missing, provide a dependency note rather than an executable-looking prompt that pretends to use it.

## Review priorities

- **Character:** identity, age presentation, required anatomy, costume, materials, intrinsic colors, distinguishing marks, and correct story state.
- **Sheet:** consistency across views, new design assumptions, orientation, required coverage, and readable labels.
- **Prop:** complete structure, credible construction for the story world, scale, handling points, markings, asymmetry, and damage state.

Repair the failing attributes while preserving approved ones. Distinguish visual review from creator approval. When the tool cannot reliably preserve identity, text, geometry, or resolution, describe the specific limitation and provide a practical handoff rather than promising exactness.


## Review, approval, and bounded repair

Deliver candidates with asset IDs, prompts, actual reference mappings, and review status. Check the relevant priorities above and distinguish observable defects from details that cannot be verified. A generated or uploaded image is not automatically approved; obtain user approval for a clearly identified revision or batch before using it as a downstream authority. Reuse existing approvals.

Repair only the failing attributes while preserving agreed ones. Stop repeated generation after one targeted repair attempt unless the user requested a larger iteration budget. Summarize remaining issues and propose the next action instead of looping indefinitely. Verify actual output dimensions before reporting delivered resolution.

Additional views and sheets should meet a stated need rather than automatically duplicate every master. Finish with an asset index, approved brief, prompts, available output files, and outstanding issues.

## Project record and revisions

For multi-asset or multi-session work, maintain one concise `seeletv-project.md` in the task's output folder. Reuse an existing record. For chat-only delivery or unavailable file writing, provide an equivalent compact handoff. Keep project data outside the installed skill directory.

Record:

- Script revision and coverage, brief revision, confirmed decisions, and unresolved choices.
- Asset ID and revision, subject/state, parent asset revisions, prompt/output locations, and status: `planned`, `candidate`, `approved`, `needs-review`, or `superseded`.
- What the user approved, bound to the specific brief or asset revision.

When a script, brief, or approved parent changes, assess downstream dependencies and mark affected assets `needs-review`. Preserve prior files and approvals as history; explain which attributes may have changed. Unaffected assets retain their status. Never overwrite an approved image as if it were the same revision. Resume from recorded decisions rather than assuming approval from file existence.
