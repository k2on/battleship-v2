# Iterations
- Version 1: Built the core 3D Battleship game with Three.js featuring animated ocean waves (custom shader), 3D ship models with hulls/decks/turrets, ship placement phase, battle phase with AI opponent, particle effects for explosions and splashes, and ship sinking animations. Used extensive custom CSS for the naval command aesthetic.
- Version 2: Added localStorage persistence and replay system. Game state auto-saves after every action, allows continuing interrupted games, stores up to 20 past games in history, and includes a full replay viewer with scrubber, play/pause, step controls, and variable speed (0.25x-4x). Refactored to use Tailwind CSS to reduce code size.

# Known Limitations

- AI is random: Enemy just fires at random untried cells with no hunt/target strategy after hits
- No sound effects: Explosions, splashes, and shots are visual only
- Mobile support limited: Designed for mouse interaction; touch controls not optimized
- Replay particles don't show on scrub: Jumping via scrubber shows markers but skips particle animations (only step-by-step replay shows them)
- No undo during placement: Must use "Random" to reset ship positions
- localStorage only: No cloud sync; data is browser-specific and can be cleared
- Single difficulty: No AI difficulty settings
