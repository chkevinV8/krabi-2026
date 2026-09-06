# Krabi 2026

A personal mobile-friendly travel field guide for a 10-day trip to Krabi, Thailand.

## Trip Theme

**Dive · Climb · Unwind**

## Highlights

- PADI Open Water course in Ao Nang
- Rock climbing in Railay / Tonsai
- Flexible recovery and weather backup days
- Hotels, food, transport, maps and practical daily cards
- GitHub Pages friendly static site

## Project Structure

```text
krabi-2026/
├── index.html
├── README.md
├── .gitignore
└── assets/
    └── images/
        ├── hero.png
        ├── map/
        ├── hotels/
        ├── diving/
        ├── climbing/
        ├── food/
        └── activities/
```

## Image Notes

- Hotel photos are the traveler's own supplied images.
- The Krabi overview map and Step 3 thematic visuals are custom project artwork.
- Thematic SVG cards are intentionally stylized location cues, not documentary photos.
- They can later be replaced one-for-one with personal photos or clearly licensed images without changing the HTML layout.

## Live Site

https://chkevinv8.github.io/krabi-2026/


## Step 4 Photo Pass

Five primary location cards now use the supplied reference photos:

- Fire Wall
- Cat Wall
- Melting Wall
- The Dive Ao Nang
- Ao Nang Local Islands

The earlier SVG artwork remains in the asset folders as a fallback/reference layer.


## Step 5 Photo Pass

The remaining featured food/recovery cards now use supplied location images:

- Café 8.98
- Thongyib Thongyod
- Royal Palm Spa


## Step 6 Code Review

- Removed the accidental duplicate Café 8.98 card under Pending.
- Simplified the OW section to two photo cards plus one compact information row.
- Added course/map links directly to the photo cards.
- Added scroll-aware navigation highlighting.
- Removed obsolete dive-card CSS and hardened external links.

## Step 7 FLEX

- Merged Klong Root / Klong Nam Sai / Ao Thalane into one flexible kayak option.
- Added a 4 Islands snorkeling option focused on Chicken / Poda area.
- Kept Deep Water Solo as the climbing alternative.
- Replaced all three FLEX illustrations with the three user-supplied photos.

## Step 9 · Sharing Ready

- Added Open Graph sharing metadata.
- Added Twitter/X large-image metadata.
- Added a 1200×630 social preview image.
- Added a favicon.
- Uses the latest cover with “Dive Deep. Climb High. Live Slow.” and no party-size label.


## Footer cleanup

- Removed the visible `Step 9 · Sharing Ready` build label from the public footer.

## Step 10 · Interactive Checklist

- Checklist items can be toggled complete/incomplete.
- Completed cards turn light green.
- Progress indicator shows completed count.
- State is saved in browser `localStorage` and restored on the next visit.
- This is device/browser-local persistence; it does not sync across devices.

## Step 11 · Smart Date Navigation

- The date strip is hidden by default.
- Clicking the main `每日行程` navigation item reveals it.
- While viewing the Daily section, the date strip stays sticky below the main navigation.
- Clicking another main section immediately collapses it.
- Scrolling out of the Daily section also collapses it automatically.

## Step 11.1 · Stable Date Navigation

- Moved the date strip directly below the primary sticky navigation.
- Removed the IntersectionObserver-based behavior that could close the strip during smooth scrolling.
- The strip opens only when `每日行程` is selected.
- It stays pinned below the main navigation while browsing Daily.
- It closes when another main section is selected or after scrolling completely out of Daily.

## Step 11.2 · Date Anchor Offset

- Date shortcuts now stop below both sticky navigation bars.
- Added extra visual spacing so the selected day header is never covered.
- Uses a calculated offset based on the actual main-nav and date-nav heights.
