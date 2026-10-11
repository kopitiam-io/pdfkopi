# Branding

PdfKopi is a Kopitiam product based on PdfCraft by the ArtCraft team.

## Rules

- **No ArtCraft marks.** PdfCraft's brand license (`docs/brand/LICENSE-brand.txt`) requires a fork
  to remove the ArtCraft name, wordmark and logos. They are removed from the app and the README.
  We may say in plain text that PdfKopi is based on PdfCraft by the ArtCraft team, and we do (the
  About dialog, the Help menu's "Based on PdfCraft" link, the README).
- **The product name is PdfKopi.** Every name a user sees says PdfKopi: the window title, menus,
  dialogs, the home screen, catalogs, the CLI's help, and metadata the app writes into PDFs.
- **Internal names stay upstream.** The `pdfcraft-*` crates, the `PdfCraftApp` type and
  `PDFCRAFT_*` environment variables keep their names, so PdfCraft fixes merge with few conflicts.
  Comments are left alone for the same reason.
- **Document markers stay upstream.** The `%PdfCraft` content-stream marker in `crates/edit` tags
  PdfCraft's own edits inside saved PDFs; renaming it would stop PdfKopi from recognising edits made
  by PdfCraft and by earlier builds.
- **Kopitiam's own mark is set in type** (`widgets::kopitiam_logo`, `widgets::kopitiam_mark`) until
  a Kopitiam logo asset exists.

## Still to do

- A Kopitiam app icon to replace `assets/app-icon/` (PdfCraft's icon is MIT/Apache-licensed, not an
  ArtCraft mark, so it is allowed meanwhile).
- New README screenshots: those in `docs/images/` show the ArtCraft mark and are no longer linked.
