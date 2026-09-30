# Storyboard — gains.trade "Referrals" recreation

Source: `assets/sssx.io_1790785143556.mp4` — 35.0s, 25fps, 3840×2160.
Project: 30fps, 1920×1080 → 1050 frames. All layout numbers below are 1080p
pixels (top-left origin) measured off the reference frames in `.ref/`.

Shared look: near-black `#060807`, faint grey 170px squares drifting in the
corners, `+` crosshairs at (94,74) (1839,74) (84,555) (1829,555) (84,1010)
(1829,1010), a low green haze along the bottom. Mint `#86f7b0`, teal `#22c3d6`.
HUD labels = text in a box with corner brackets, typed on with a block caret.

| # | File | Source time | Frames | Shot |
|---|------|-------------|--------|------|
| 1 | 01-link.ts | 0.0–4.5s | 135 | URL bar + lock. Camera pushes 0.55×→1.8×. REFERRALS / NOW SELF-SERVE HUD types on. Lock unlocks (1.2s), fills green with pixel burst + green flash (1.4s), squashes into the text caret (2.2s). "alpha" types (2.5–3.0s). HUD glitches out (3.4s). "Copy link" button pops with pixel ring (3.4s), hand cursor arrives, clicks (4.0s), button tilts & flies (4.4s). |
| 2 | 02-share.ts | 4.5–9.4s | 147 | Capsule shrinks to the orb (4.8s). Three spokes to wireframe globes w/ Telegram / X / Discord badges swing into place (5.0–5.8s). SHARE IT ANYWHERE HUD types. Packets travel in (6.0s+). Camera tilts into 3D (6.8–7.4s), counter box "$ 0.00 ↑" counts to 1284.00 (7.0–8.8s). Scene falls into darkness (9.2s). |
| 3 | 03-tree.ts | 9.4–16.4s | 210 | Line draws into "You $0.00" pill (9.4–10.2). Counter ticks up ~270/s to 1621. L1 (green) hangs off You (10.8), L2 (teal) off L1 (11.4); +10% / +5% tags with glowing packets up the connectors. Push to 1.29× (11–12s), punch to 2.6× on the number with pixel glitch (12.4–13.6), pull back to overview (14.0). HUD: "Earn 10% of their fee" / "5% of everyone they bring in" (14.0–15.0). |
| 4 | 04-bound.ts | 16.4–20.3s | 117 | L1/L2 pills multiply into a scrolling wall (16.4–17.6), pull back to a small grid (17.8), slide right and compress into a gradient block against a mint bar (18.2–18.5) with a lock badge. HUD "Bound to you / for life". Dashboard edge sweeps in (20.0). |
| 5 | 05-dashboard.ts | 20.3–28.9s | 258 | 3D-tilted referral dashboard with a mint glow edge. Stats count up, bar chart grows, table rows. Camera: swing in (20.3–21.2), glide down over rewards (21.2–23.4), tilt across the table (23.4–24.6), flat close on header stats (25.0–26.2), rewards (26.2–26.9), table with a type badge flashing mint (26.9–28.6). Fade out. |
| 6 | 06-outro.ts | 28.9–35.0s | 183 | Dark mark fades in (29.2), green bloom + pixel frame (30.4), mark slides left as "gains" wordmark reveals (30.9–31.5), URL types beneath (31.5–33.0). Hold. |

Build order: static key poses for every scene → compare against reference →
animate → compare → swap copy (components/copy.ts) to the sarcastic version.
