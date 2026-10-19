# Timed Video Prompts

## Keep the units distinct

A shot is a continuous camera view. It can contain several action or camera phases without a cut. A generation request is one model invocation; it may contain one shot or a supported multi-shot sequence. A take is an actual generated candidate. Editing can use only part of a take.

Choose whether the user needs a continuous shot, separate shot prompts, or a multi-shot prompt. Do not turn every timestamp into a cut. For prompt-writing, honor the requested packaging: a model-neutral timed multi-shot prompt is a valid direct deliverable even before a provider is selected. Verify multi-shot support before actual submission; do not split the requested prompt or block its delivery merely because no model was named. Produce separate prompts when requested or required by a verified target interface.

## Allocate time from the material

Start with the required duration or propose a clearly labeled duration when none is supplied. Estimate the time needed for speech, physical action, overlapping action, and reactions. Dialogue language, delivery, pauses, and speaker changes affect runtime. Treat timing as direction, not a promise of frame-exact model control.

Break time at meaningful events: a trigger, movement phase, contact, response, reveal, cut, or settle. Use a few intervals rather than filling one row per second. Second-by-second direction is useful for a precise synchronization request or a brief complex interaction; it is not a universal quality criterion. Avoid arbitrary decimal precision unless synchronization needs it.

For each interval, make the participants, action, camera behavior, and destination understandable. Actions that must happen in sequence need distinct time; compatible performance, camera movement, and ambience can overlap. Do not cut dialogue midway unintentionally or fit a long line into an implausibly short slot. If the content will not fit, propose fewer beats, more time, or an authorized dialogue reduction.

Check that intervals progress in order, adjacent shot boundaries meet, and the planned sequence reaches the stated duration. Explain intentional ellipses, overlaps, and sound bridges. Distinguish global sequence time from local time in separately submitted clips.

## Build the copyable prompt

Include the following as applicable, in readable production language rather than empty fields:

1. The actual reference inputs and their roles, or a compact subject/setting description if no references exist.
2. Relevant stable appearance, setting, visual direction, and opening state.
3. Timed shot blocks. Each names the visible characters, camera start, framing, spatial relationship, acting/action, camera path or hold, and endpoint. Sound can be integrated with its event or collected into a clearly timed sound line.
4. Critical continuity limits and exclusions, only where they prevent a likely consequential error.
5. Requested output settings outside prompt prose when the tool has dedicated fields.

Use exact readable labels such as '0–4s — Shot 1, ...' for a generic timed prompt; use provider tags only when verified. For a phase inside one continuous take, label it as a phase, not another shot. For independent clips, repeat enough setup that each prompt can stand alone. Never rely on 'same as above' or on the model remembering another request.

Do not paste narrative analysis, internal IDs as visible text, unresolved alternatives, empty placeholders, or instructions to the user into the generation block. If a required reference is missing, provide a clearly marked preparation draft and dependency note, not a falsely executable reference-based prompt. A user may explicitly choose a text-only reinterpretation.

## Illustrative continuous take

This is a model-neutral example of direction, not a claim that any provider accepts its formatting. It uses no reference files.

```text
One continuous 8-second take, no cuts. A quiet kitchen at dusk. A woman in a dark blue shirt stands on the far side of a wooden table, a brass key already held by its bow in her right hand above the table. A man in a grey sweater sits opposite, facing her, both hands resting on the near edge. A window behind the woman supplies soft dusk light, with room bounce keeping both faces readable; no music or dialogue.

0–2s: Medium two-shot from the table's short end at seated eye level, showing both faces and hands in profile. She looks at his empty left hand, then places the key on the table between them. He keeps his eyes on her. The camera holds.
2–5s: He looks down and slides the key toward himself with his left index finger, then closes his left hand around it. She draws her right hand back to her side. The camera tracks a short distance toward his side of the table without crossing the line between them, keeping his hand and face visible.
5–8s: He lifts his gaze to her, his mouth tightening before he gives a small nod. End in a medium close-up of him, his closed left hand still visible at the bottom of frame. The camera settles. A faint scrape of metal on wood follows the key's slide; quiet room tone continues.
```

The phases describe successive states inside one shot. The key changes ownership once, and the endpoint remains available for the next shot.

## Illustrative sequence plan

For a 12-second scene, a possible plan is:

| Sequence time | Shot | Camera and performance | Endpoint |
|---|---|---|---|
| 0–4s | 1 | Medium two-shot from the counter side; the visitor places a sealed envelope on the counter while the clerk watches | Envelope rests between them; visitor's hand has withdrawn |
| 4–7s | 2 | Cut to a close view along the clerk's side of the counter; clerk turns the envelope once with the right hand, revealing its established mark | Mark visible; clerk's hand stops |
| 7–12s | 3 | Cut to the visitor's eye-line on the clerk; a restrained push starts as the clerk recognizes the mark, stops on the clerk's face; the clerk looks back at the visitor without speaking | Recognition held, envelope remains on counter |

The actual mark, appearances, setting, and visual direction must come from the user's material or an identified design proposal. A combined model prompt must spell out those facts and each cut, not submit this abbreviated table as the complete prompt. For separate generation, reset each clip's time to zero and restate its opening, references, and continuity. Do not repeat the envelope placement or turn in a later shot.

## Final timing pass

Read the scene as a performance. Verify the cut points, speech length, object state, eye-lines, who remains off screen, camera phases, and endpoint. A timestamp alone does not make an impossible action feasible. If a model's limits require different packaging, preserve the dramatic shot design and explain the production adjustment rather than silently changing the story.
