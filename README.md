# Agility

**Pet Agility Course** — Physics obstacle course that scores a pet's speed, jump, and stamina traits.

Part of the [ComputerPets](https://github.com/RicheyWorks/computerpets) universe. Map: [computerpets-ecosystem](https://github.com/RicheyWorks/computerpets-ecosystem).

> Status: **design scaffold**. Gameplay contract is frozen. Engine choice is the one in the brief. Implementation comes next.

## Loop

The overlay already has walk and carry. Agility is the stopwatch: same body, timed gates, no combat. Reed the frog and Rui do not share a jump arc.

## Genre & engine

- Genre: **Physics runner**
- Engine: **Godot 4**
- Stack: Godot 4.3 · GDScript · rigid-body course · speed/jump traits from overlay
- Default surface: `Godot editor`

## How you play

1. Pick one owned pet.
2. Run a seeded daily course (same seed worldwide).
3. Missed gate = time penalty, not death.
4. Ghost of your best run + friends via Visitation ids.

## Talks to

- computerpets (traits)
- computerpets-motion (clips)
- computerpets-quests (daily course)
- computerpets-telemetry

## Failure doctrine

Physics explode → reset to last gate, never T-pose. Trait missing → species default, never another animal's numbers.

Canon rules that never yield:

- 210 living kinds. No illegal hybrids.
- Overlay pets can get tired, sick, or hide. Tokens are not burned by a minigame.
- Desktop walk stays the main quest. Closing Agility must leave Rui walking.

## Layout

```
computerpets-agility/
  README.md
  LICENSE
  docs/DESIGN.md
  src/                implementation lands here
```

## Run (Windows)

```powershell
godot --path . --import; F5 in editor. Export Windows exe for overlay-adjacent play.
```

Meet Rui first via the [flagship start-here](https://github.com/RicheyWorks/computerpets/blob/main/docs/START-HERE.md). This game is optional.

## License

MIT. See [LICENSE](LICENSE).

---

*Two hundred ten living kinds. Keep them so a line does not go quiet.*
