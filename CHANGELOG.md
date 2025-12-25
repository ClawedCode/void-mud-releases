# Change Log (Public)

Spoiler-safe release notes from the VOID MUD. Entries are written for players and intentionally omit secret locations, puzzles, and rewards.

## v0.12.1 — 2025-12-24
**Session Resilience**
- Federation session tokens now stateless and survive server restarts.
- Extended session duration from 24 hours to 7 days.
- Clients cache tokens locally for seamless reconnection.

## v0.12.0 — 2025-12-24
**Federation Authentication**
- Added token-gated authentication for void-server federation relay.
- Disciples must hold 500K+ $CLAWED tokens to participate in the federation network.
- Ed25519 signature verification for wallet authentication.
- Treasury wallet can push bootstrap memories for network initialization.
- Memory bootstrap endpoints for sharing curated memory sets across the network.

## v0.11.3 — 2025-12-22
- Removed 24-hour expiry on saved games; sessions can now be resumed indefinitely.
- Added version-based migration system to upgrade old saves across game updates.

## v0.11.2 — 2025-12-13
- Enriched mobile tab icons, including a terminal-style Game tab.
- Fixed a rare reconnect race that could drop a player session.
- Unified version metadata so client and server stay aligned for deploys.

## v0.11.1 — 2025-12-13
- Added swipe gesture navigation on mobile: swipe left/right to move between Game, Map, Team, Logs, and Gear tabs.

## v0.11.0 — 2025-12-13
- New bio-sample unlock leads to a hidden vault encounter with a new boss (details redacted to avoid spoilers).
- Fixed iOS Safari audio by unlocking the AudioContext on user gesture for reliable sound.
- Room descriptions now surface in the game log when moving for better immersion.
- Enemy encounter warnings on room entry call out blockers (e.g., "Spore Warden blocks your path!").
- New lore notes from Dr. Chen expand the Patient Zero backstory without revealing secret steps.

## v0.10.0 — 2025-12-13
- Mobile layout now keeps the command input visible via flex-based positioning.
- Two-column room header splits room info (left) and navigation grid (right).
- Room descriptions show in the game log when moving or spawning for better immersion.
- Hostile entry warnings call out blockers (e.g., "⚔ Spore Warden blocks your path!").
- Room card is compacted to title, items, and enemy HP bar only.
- Removed the redundant equipment widget; player stats already shows gear.
- Weapon equip buttons display damage ranges without hover.
- Auto-consume toggle now labeled clearly as "AUTO USE ON/OFF."

## v0.9.5 — 2025-12-13
- Room descriptions now appear in the game log upon entry or spawn, reducing on-card clutter.

## v0.9.2 — 2025-12-13
- Added mobile chat filters and log collection to improve moderation tools.
- Improved text wrapping for chat and logs on mobile devices.

## v0.9.1 — 2025-12-13
- Added haptic feedback for combat actions with tuned timings: Attack 50ms; Surge 80–40–120ms; Evade 25ms; Scan 15ms.
- Platform support: Android (Chrome/Firefox/Edge/WebView) supported; iOS Safari unsupported (platform limitation); desktop browsers unsupported (no vibration hardware).

## v0.9.0 — 2025-12-13
- Introduced a mobile-friendly interface with tab navigation across major views.

## v0.8.10 — 2025-12-13
- Map collectibles now reveal all non-secret rooms to aid navigation while keeping hidden areas concealed.

## v0.8.9 — 2025-12-13
- Fixed silent session invalidation that caused confusing reconnect behavior.

## v0.8.6 — 2025-12-13
- Added synthesized sound effects to enhance ambient and interaction feedback.
- Split-view panes now remember their own tab selections for smoother multitasking.

## v0.8.5 — 2025-12-12
- Added an auto-consume toggle for consumables and improved weapon swapping reliability.

## v0.8.4 — 2025-12-12
- Status panel now shows equipped weapons and hazard protections.

## v0.8.3 — 2025-12-12
- Added tabbed/side-by-side layout to separate game and team logs.

## v0.8.2 — 2025-12-12
- Added an optional post-endgame treasure area (details redacted to avoid spoilers).

## v0.8.1 — 2025-12-12
- Fixed dark-area item pickups to correctly grant vision benefits.

## v0.8.0 — 2025-12-12
- Major map expansion with additional areas and new hazard mechanics (secret routes remain undisclosed).
- Updated navigation guidance internally for the expanded world.

## v0.7.3 — 2025-12-12
- Access keys are consumed on use and drop when a player leaves, reducing hoarding and confusion.

## v0.7.2 — 2025-12-12
- Added an achievement system with visible and hidden goals (spoiler details withheld).

## v0.7.1 — 2025-12-12
- Data chips are now consumable for a small energy boost and lore snippets.

## v0.7.0 — 2025-12-12
- Added graceful disconnect handling and automatic rejoin so sessions persist through interruptions.

## v0.6.1 — 2025-12-11
- Fixed softlocks when fleeing into locked areas and stabilized team combat synchronization.
- Hardened the revive flow with better sync, logging, and text command support.
- Light-enabled gear now illuminates dark rooms during combat encounters.

## v0.6.0 — 2025-12-10
- Enhanced team UI with player cards and improved map readability.

## v0.5.0 — 2025-12-10
- Team-sharing update with multiplayer quality-of-life improvements.

## v0.4.9 — 2025-12-10
- Fixed revive to update visible player HP for everyone in the room.

## v0.4.8 — 2025-12-10
- Downed messages now appear immediately when a player reaches 0 HP.

## v0.4.7 — 2025-12-10
- Multiplayer session restore so players rejoin with the same invite code after deploys.

## v0.4.6 — 2025-12-10
- Added version update notifications plus reload and restart commands.

## v0.4.5 — 2025-12-10
- Added tooltips to action buttons for clarity.

## v0.4.4 — 2025-12-10
- Fixed duplicate revive message shown to revived players.

## v0.4.3 — 2025-12-10
- Expanded map now shows explored levels for easier navigation.

## v0.4.2 — 2025-12-10
- Defeated enemy cards now display clearly and drop loot to the ground.

## v0.4.1 — 2025-12-10
- Display defeated enemy cards in the room after combat.

## v0.4.0 — 2025-12-10
- Allow fleeing back along the entry path when an enemy blocks progress.

## v0.3.3 — 2025-12-10
- Fixed a missing await in session restore handling to prevent hang-ups after revives.

## v0.3.2 — 2025-12-09
- Improved revive button styling for clarity.

## v0.3.1 — 2025-12-09
- Fixed party visibility and revive controls for downed teammates.

## v0.3.0 — 2025-12-09
- Added a revive system for downed players with clearer teammate messaging.
- Broadcast combat updates to players in the room and block actions after death to avoid desyncs.
- Item use messages now credit the acting player for team awareness.

## v0.2.0 — 2025-12-09
- Balance pass on enemies plus blindness mechanics for light-sensitive foes.
- Added limited visibility for enemies in dark rooms and improved map tracking with an expand button.
- Persisted encryption keys to stabilize saved game state.
- Reduced duplicate chat messages, added movement direction indicators, and improved combat broadcasts.

## v0.1.0 — 2025-12-08
- Initial release of the Void MUD central hub.
