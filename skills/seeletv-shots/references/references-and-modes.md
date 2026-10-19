# References, Keyframes, and Generation Modes

## Reference authority

Use only supplied or accessible material. Inspect actual images before describing their visual contents. A filename or thumbnail cannot establish fine facial features, text, or a complete spatial layout. If media cannot be opened, state which facts are user-reported or unverified. Do not infer canvas connections or hidden upstream assets.

Distinguish a candidate from a user-approved reference. Honor existing approval without requiring a special word. Current selection, upload, and technical completion alone are not creator approval. When the user explicitly designates an image as the reference for this task, use that stated role without demanding a separate ceremony.

Give each reference a precise role and preservation scope:

| Role | What to carry | What not to import by default |
|---|---|---|
| Character identity | Face, stable proportions, distinguishing features | Incidental pose, background, another costume state |
| Costume or story state | Agreed clothing, injury, age, wetness, damage | A different identity or later story event |
| Location | Entrances, fixed anchors, scale and directional relationships | Incidental people or transient objects |
| Composition | Framing, subject placement, eye-line layout, depth | Reference person's identity or unrelated design |
| Visual treatment | Palette, texture, contrast, material language | Source plot, logos, identities, geography |
| Start/end frame | The specified boundary's visible arrangement and state | Actions that belong outside that boundary |
| Source video | Observed movement or continuity relevant to the task | Every incidental event, identity, or sound layer |

A reference can serve more than one stated role if supported; do not split it into duplicate uploads merely to fill a schema. If references conflict, identify the conflict and preserve the user's priorities. Reference roles express intent, not a guarantee that a model can isolate those influences perfectly.

## Keyframes

A reusable character or prop sheet establishes an asset; a shot keyframe establishes a particular view and state. Do not treat them as interchangeable. A start-frame prompt depicts the opening instant, without placing a completed transfer, injury, reveal, or exit there prematurely. A proposed end frame depicts the agreed endpoint.

A still prompt describes visible composition, participants, posture, gaze, object state, light, and relevant reference roles. Camera travel and successive actions belong in the video prompt. A new angle can expose unapproved back-side or spatial details; label them as proposed design, not facts recovered from a single reference.

## Choose a mode by the needed control

- Text-only generation is suitable when precise reference continuity is not required or the user chooses it.
- A first-frame workflow anchors an opening arrangement when the tool supports it.
- First/last-frame generation can guide a known transition if supported, but does not guarantee a valid path between incompatible states.
- Reference-based generation can preserve designated identity, setting, appearance, or motion, subject to the tool's actual roles and combinations.
- Editing or extension requires the real source media and verified controls. Do not describe a new independent shot as a seamless extension.

Use the exact model and interface when checking capabilities. Different services exposing the same model name may offer different durations, media roles, reference counts, audio behavior, or edit controls. Read current official documentation or the host's verified capability catalogue when necessary. Record an important unsupported or unknown control; do not invent tags, limits, prices, or hardcode one vendor's syntax as universal.

Keep settings separate from prose where the interface provides them. Map readable reference names to actual attachments and their verified order or slots. Missing images do not silently convert a reference-based request into text-only generation. Prompt preparation can proceed with clearly identified missing dependencies when the user wants a plan.

## Connected clips

For continuous action, inspect the accepted previous clip or actual final frame. A still confirms visible position and state but cannot by itself confirm movement direction, velocity, camera phase, or audio timing. Preserve that uncertainty.

Begin from the observed state, not the hoped-for endpoint. Keep rejected takes out of continuity. An accepted visual deviation does not authorize a changed plot: reconcile it with the user or repair it before continuing. Use a new intentional cut or canonical reference to recover identity and geography when chaining output introduces drift; do not rely on a universal maximum extension count.
