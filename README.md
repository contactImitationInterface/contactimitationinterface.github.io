# CIMI project website

Local clone of https://github.com/contactimitationinterface/contactimitationinterface.github.io.

## Preview

Run `python3 scripts/serve.py` from this directory, then open http://127.0.0.1:8000.
The site is static and needs no build step or external dependencies. The preview server supports byte-range requests so videos can seek correctly.

## v33 update

The supplementary video is the final `CIMI_ICRA_Supplementary_v33_Josh.mp4` from the CIMI workspace. Its SHA-256 is `ce9c43bdb4d86fa79b4f705d93ca5b4de0c359b2d83f2313f15cc4907d4902ac`.

- Full narrated video with English captions. Demonstration and comparison videos require the native play control. The silent retargeting animation autoplays and loops when visible, and pauses when hidden.
- Four silent task clips extracted from that final video, preserving camera geometry and playback-speed labels, including the corrected bulb panel on slide 9.
- Four evaluation observations aligned with slides 10–13, including the caption corrections on slides 11–12 in the full video.
- Captions use the existing narration text and measured audio timings from the v33 build.
- Collection efficiency and the static rollout figure were removed. The supplementary PDF and anonymous submission details remain from the source website.

`assets/videos/manifest.json` records source clip timings. Demonstration and comparison videos load on request; the retargeting animation loads metadata and plays when visible. Without JavaScript, all stage content and comparison clips remain accessible.

## Page structure

- Overview and full supplementary video.
- Method: Collection, Preprocessing, Policy training, and Inference, with numbered buttons and Previous/Next navigation. Each stage starts with its inputs and outputs.
- Human demonstrations paired with robot policy rollouts for four tasks.
- Observations: four selectable inline comparisons, using the same navigation as Method.
- Abstract and supplementary PDF.

The Method section includes the human collection video, side-by-side retargeting and reprojection, and planner/controller architecture diagrams from the supplement. Figures use SVG exports from the original PDFs. The site retains the Amarna font and CIMI blue, green, and orange colors.
