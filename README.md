# Iterations
- Version 1: First I tried to have the game be multiplayer where I could send someone the link and play them and it be in real time, but I soon realized I was too ambitious, and asked it to revert the changes.
- Version 2: Added localStorage persistence and replay system. Game state auto-saves after every action, allows continuing interrupted games, stores up to 20 past games in history, and includes a full replay viewer with scrubber, play/pause, step controls, and variable speed (0.25x-4x). Refactored to use Tailwind CSS to reduce code size.

# Known Limitations

- AI is random: Enemy just fires at random untried cells with no hunt/target strategy after hits
- No sound effects: Explosions, splashes, and shots are visual only
- Mobile support limited: Designed for mouse interaction; touch controls not optimized
- Replay particles don't show on scrub: Jumping via scrubber shows markers but skips particle animations (only step-by-step replay shows them)
- No undo during placement: Must use "Random" to reset ship positions
- localStorage only: No cloud sync; data is browser-specific and can be cleared
- Single difficulty: No AI difficulty settings
