# Road to 1.0

0.2.3-preview remains a preview. A polished interface does not replace validation
of exported mods and the game compatibility profile.

## Release gates

1. **Verify a complete mod in Beat Banger build 25730471.** Create a two-level
   pack with three difficulties, original spritesheets, scene/audio events and
   pre/post cutscenes. Export, install and play every part in the real game.
   Reimport the result without losing unknown fields or native value types.
2. **Validate gameplay parity.** Compare both scroll layouts and deterministic
   test charts with the game: exact judgment boundaries, simultaneous notes,
   all seven modifiers, early/late hold releases, miss forgiveness, health,
   combo, score and final grades. Record differences before changing the profile.
3. **Finish preview fidelity.** Validate animation variants, background modes,
   pulse, shutter artwork, camera and all cutscene transitions. Implement the
   preserved transitions beyond fade. Check video/audio sync over complete long
   levels, after seeking and during their endings.
4. **Make long operations reliable.** Add incremental progress and cancellation
   for pack import/export. Confirm cancellation leaves complete old outputs
   intact. Exercise disk-full failures, locked files and termination at several
   save/autosave stages; verify recovery on restart.
5. **Accept the Windows release.** Test real 1366×768 and 1920×1080 desktops at
   100%, 125% and 150% scaling, keyboard focus, every tool and multi-window/full
   screen operation. Profile cold image/video transitions on modest hardware.
   Package with official matching Godot Windows export templates and verify the
   portable build on a clean machine without a Godot installation.

## Useful improvements before release

- Give uncertain menu beat detection a user-controlled BPM/phase override while
  retaining automatic analysis as the default.
- Add clearer contextual help for native event fields and error locations.
- Offer an editable export checklist tied to actual project diagnostics.

These improvements follow the core release gates; they do not expand 1.0 into
MIDI, automatic chart generation or physical device connectivity. Keep the
project format compatible and game references local. Publish the application
only after final release authorization.
