# Modulation website: build plan (for Claude Code in VS Code)

Repo: hrishi16/Modulation (GitHub Pages, vanilla HTML/CSS/JS, content in `content/*.json`, edited by Asmita through Decap CMS at `/admin/`).
Rule from the exhibition note: the paintings catch the *experience* of pain; they never illustrate the science. Art and science sit side by side.

Work only inside this folder. Originals (TIF/JPG/GIF) are in the image subfolders here: use them in place of the low-res screenshot crops in `images/lab/`.

## Phase 0: one branch (do first)
1. Merge `v2-preview` into `main` (fast-forward; main is behind by one commit). Delete `v2-preview` afterwards.
2. Hrishi sets Settings → Pages → Branch = `main`, `/ (root)`.
3. From here on: work on `main`, preview locally (`python3 -m http.server`), push when Hrishi approves.

## Phase 1: felt ↔ measured dial (top priority)
Rule: **felt = an artwork, measured = a lab image. Always.** No science-only pairs.

1. Remove the current pair 3 (`oxali_art` ↔ `minis_raw`). The stylised calcium still can go into panel 01 instead.
2. Fix the text overlap under the slider: when the caption wraps to two lines it runs into the hint and credit lines. Captions must take their own height (no absolute stacking that ignores line count). Check at 360 px and 1200 px widths.
3. Add these pairs to `content/home.json → pairs` as placeholders (captions drafted, marked for Asmita's approval):

Only Asmita's paintings (no workshop images). Each lab dataset is used once.

| # | Felt (artwork) | Measured (lab) | Link |
|---|---|---|---|
| 1 | Pain in the Brain | **to replace:** the spinal cord RFP is too dim (see option below) | — |
| 2 | Artist-reworked micrograph | Grpr+ PBN (keep) | existing |
| 3 | Rewired | ACC D1R neurons (d1r_1) | painted filaments ↔ real dendrites |
| 4 | Rewiring | Microglia IBA1 (hippocampus) | touch rewired into pain |
| 5 | Chronic | PBN c-Fos (pbn_0) | bruise-spots ↔ LPBN lights up in chronic pain |
| 6 | Sweet Sorrow | MHb tdTomato fibres (mhb_6) | wire + poppy ↔ pain fibres in an opioid-rich region |
| 7 | That Sinking Feeling | central thalamus c-Fos (cfos_3) | pain-related anxiety |
| 8 | Towards Heaven | thalamus calcium still (minis_raw) | temperature turning into pain |
| 9 | Pushing Through | lateral hypothalamus (lh_1) | needs/stress competing with pain |

Dropped: In Blue (it would repeat the central-thalamus dataset) and all workshop pairs.
Pair 1 option, decided by Hrishi: see the chat.

4. Image prep: from the originals, export WebP of about 1500 px on the long edge and under about 500 kB. Never commit raw TIFs.
5. Test on a phone (Android), then push.

## Phase 2: science images in each theme
1. Replace every `images/lab/*.webp` screenshot crop with a version made from the original, keeping the same filenames.
2. Check the placements: 01 thalamus calcium, 02 PBN c-Fos + LH, 03 MHb set, 04 ACC D1R, 05 central-thalamus c-Fos, 06 microglia (caption says hippocampus).
3. Captions and credits: drafts, then lab approval. Fix "nociplactic" to "nociplastic". Rename the astrocytes file to microglia.

## Phase 3: Take part (three versions to compare)
Keep the Take part page as one nav item, with three tabs inside it (the nav already wraps to two lines):
- **Take part 1:** the existing body map, unchanged.
- **Take part 2: "Felt or measured?"** An unlabelled close-up (from a painting or a micrograph) is shown and the visitor guesses which it is. Zooming out reveals the whole image, its title and a short science text. Crops come from a JSON list Asmita can edit (image, crop position, answer, text).
- **Take part 3: "Bruise bloom."** One of Asmita's body paintings (Touching or Towards Heaven) is the surface. Pressing and holding grows a bruise in her colours (dark centre, purple ring, orange halo), and its size follows how long you hold. On release, the nearest painting and the science under it appear. Respect prefers-reduced-motion. Nothing is stored.
Build 2 first, then 3.

## Handover (the laptop goes away next week)
- Commit every converted web image to the repo, so the site never depends on this laptop.
- Hrishi copies the originals folder to the project Google Drive.
- Later work can be done from claude.ai (it can clone the repo and push), and Asmita edits through /admin/.

## Open items
- Asmita approves or swaps the pairings and captions.
- The lab's channel legends and credit lines for each image set.
