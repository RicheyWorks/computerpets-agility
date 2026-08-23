# Agility design

Implement against this file, not folklore.

## Identity

- Product: **Agility**
- Repo: `computerpets-agility`
- Idea: Pet Agility Course
- Genre: Physics runner
- Engine: Godot 4
- Surface: `Godot editor`

## Loop

The overlay already has walk and carry. Agility is the stopwatch: same body, timed gates, no combat. Reed the frog and Rui do not share a jump arc.

## Play beats

- Pick one owned pet.
- Run a seeded daily course (same seed worldwide).
- Missed gate = time penalty, not death.
- Ghost of your best run + friends via Visitation ids.

## Neighbors

- computerpets (traits)
- computerpets-motion (clips)
- computerpets-quests (daily course)
- computerpets-telemetry

## Failure doctrine

Physics explode → reset to last gate, never T-pose. Trait missing → species default, never another animal's numbers.

## Hard rules

1. Minigames cannot mint or burn NFTs by themselves (Minter is the write path).
2. Stats come from lived overlay care + Dojo caps, not cash shop.
3. Species kits stay inside Lore. Illegal hybrids never spawn.
4. Fail soft: the desktop overlay process is not this process.
