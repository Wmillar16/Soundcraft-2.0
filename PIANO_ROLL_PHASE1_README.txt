# SoundCraft custom Piano Roll — Phase 1 source patch

This archive is the uploaded SoundCraft source tree with one modified source file:

`crates/ui-egui/src/panels/midi_editor.rs`

Phase 1 changes:
- Independent X zoom (Ctrl + mouse wheel) and Y zoom (Alt + mouse wheel), anchored at the pointer.
- Horizontal scrolling using horizontal wheel/trackpad delta; ordinary wheel scrolling remains vertical.
- Double-click empty piano-roll space to add a snapped MIDI note.
- Double-click an existing note to delete it.
- Piano-roll playhead drawn from SoundCraft's existing transport position and tempo map.
- Existing drag, resize, selection, velocity editing and MIDI engine commands are retained.

Important:
- This is a SOURCE archive, not a compiled Windows installer or executable.
- The changes have not been compiled or run in this environment because Rust/Cargo are not installed here.
- Do not copy this `.rs` file into the installed application directory. It belongs in the source tree at the path above.
- Building the application requires the Rust toolchain described in the repository README (Rust 1.95+).
- Scale highlighting / scale-aware snapping and custom workspace design are not included in this first patch.
