# Color Range review screenshots

Review evidence for the Color Range preview follow-up to storytold/photocraft#1239.
This orphan branch is separate from all application source branches and is not included
in the pull request diff. Images use synthetic red/blue/black/white fixtures, not personal
photographs or project documents.

- Native eyedropper / blue selection: actual native X11 Linux capture (600 × 360 palette).
- Other images: deterministic offscreen egui/wgpu renderings from the Color Range fixture.
- White marks selected pixels; black marks unselected pixels; Quick Mask covers unselected
  pixels. Image switches the dialog thumbnail to the display-managed composite.

Recorded before the performance fix for the offscreen fixture, and after it for the native
blue selection. The performance fix changes cache-key work, not their visual appearance.

The source changes and their validation are documented in the linked pull request.
