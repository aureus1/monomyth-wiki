---
name: 🌐 Location inaccuracy
about: A pinned item or point is in the wrong place on a level map
title: "[Location] "
labels: ["data", "location"]
assignees: []
---

> **How to report a location error**
>
> Map pin positions are projected from extracted game data and then
> hand-calibrated. Calibration isn't perfect, so pins can be off. To fix a pin
> we need to know **exactly** where it should be — as a calibration JSON
> snippet, not a screenshot.
>
> **Please do the following before filling out the rest of this issue:**
>
> 1. Open the level map page on the wiki that has the wrong pin.
> 2. Click the **✏️ Edit pin positions** button above the map.
> 3. **Drag the wrong pin(s)** to their correct location(s) on the map.
> 4. Below the map, a **Calibration JSON** snippet appears. Click **Copy**.
> 5. **Paste the JSON snippet** into the "Calibration JSON snippet" section of
>    this issue (paste it as text inside a code block).
>

## Level / map page

Which level map is affected? Give the page name and URL, e.g.
`Level_Tutorial01` — `https://monomyth.aureus.me/docs/.../level-tutorial01`

## Which item / pin is wrong?

Name the item, label, or pin that's misplaced (e.g. "the Echo Stone pin",
"Broadsword", "the second chest").

## What's wrong with it?

- [ ] Pin is in the wrong room / area
- [ ] Pin is in the right room but wrong position within it
- [ ] Pin is missing entirely (item exists in-game but isn't on the map)
- [ ] Pin exists but the item doesn't (phantom pin)
- [ ] Other (describe below)

## Calibration JSON snippet

**Paste the Calibration JSON snippet from the wiki's edit mode here.** Put it
inside a code block (three backticks). It should look something like:

```json
{
  "Level_Tier01C": [
    {
      "worldX": -74164.67,
      "worldY": -6602.948,
      "mapXPercent": 75.30,
      "mapYPercent": 9.20,
      "note": "Armor_MinersShirt — drag-calibrated"
    }
  ]
}
```

> If the map's edit mode produced no snippet (e.g. no `levelId` on the overlay),
> say so here and attach a marked-up screenshot as a fallback.

## Further details

Any extra context: the item's in-game coordinates if you know them, which door
or landmark the correct spot is near, whether the whole map looks shifted, etc.
