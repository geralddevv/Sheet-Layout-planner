# **Nyxen**
### Print Layout Engine for Labels & Coupons

Nyxen turns sticker, label, and coupon sheet planning into a visual, drag-free workflow. You enter the page size, label cell, and gap dimensions, and Nyxen figures out the grid, renders a realistic preview, and spools out a PDF with trim marks that you can send straight to press.

**Highlights**
- Instant visual grid preview with live row/column counters
- Portrait/landscape flip plus auto-centered margins (with manual overrides)
- PDF export that keeps trim marks, gutters, and bleed in sync
- Built for standards-based page sizes (ISO A/B/C and US formats) plus custom dimensions

## Overview
Nyxen is a single-page tool built on React + Vite that helps designers, print techs, and production teams batch-planned layouts for labels, coupons, tickets, and similar sheeted media. Because it keeps the calculations visible and tied to an on-screen canvas, you can tweak gutters, margins, and trim settings with confidence before exporting a proof-ready PDF.

## Usage
1. Choose a preset (A/B/C series or US format) or type a custom size.
2. Enter the label/coupon cell width, height, and gutter spacing.
3. Toggle orientation (portrait/landscape) and let Nyxen auto-center the margins—or tweak them manually.
4. Watch the floor-plan preview update with the live grid count.
5. When the layout looks right, click **Generate PDF** to see the sheet with trim marks.

### Margin Controls
- `Reset Margin` snaps everything back to equal edges for centered layouts.
- Manual overrides allow you to lock one or both margins when you need asymmetry for production constraints.

## PDF Export
The PDF output is created with `@react-pdf/renderer` and `pdf-lib`. Every export includes:
- Trim marks aligned to the printable area
- Optional alignment lines so you can check registration
- Embedded metadata so downstream tools know the sheet size and orientation

You can preview the PDF inline (powered by `@embedpdf/snippet`) before downloading the file for print review.

## Tech Stack
- **Framework:** React 18 + Vite
- **Styling:** Tailwind CSS
- **PDF generation:** `@react-pdf/renderer`, `pdf-lib`
- **Preview:** `@embedpdf/snippet`
- **Animation:** Framer Motion for subtle UI feedback

## License & Distribution
© 2026 Gerald. All rights reserved. This repo is intended for personal use only; copying, modifying, or commercial distribution is not permitted under the current license.

If you'd like to collaborate or extend the project, feel free to reach out and we can pair on a forked version or feature branch.
