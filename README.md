<h1 align="center">PdfKopi</h1>

<p align="center">
  <b>A free, local-first PDF workbench from <a href="https://kopitiam.io">Kopitiam</a>.</b><br>
  Read, organize, combine, split, fill, sign and secure PDFs in a fast native app, written in Rust.<br>
  macOS · Windows · Linux · FreeBSD · the web
</p>

<p align="center">
  <img alt="License: MIT OR Apache-2.0" src="https://img.shields.io/badge/license-MIT%20OR%20Apache--2.0-12a58a">
  <img alt="Written in Rust" src="https://img.shields.io/badge/written%20in-Rust-0a7563">
  <img alt="No account, no telemetry" src="https://img.shields.io/badge/no%20account-no%20telemetry-0a7563">
</p>

PdfKopi is Kopitiam's PDF app: no account, no upload, no telemetry. Your documents never leave
your machine. It is the first of a family of Kopitiam desktop apps, each named after something
on the kopitiam menu.

PdfKopi is based on [PdfCraft](https://github.com/storytold/pdfcraft) by the ArtCraft team, a
clean-room PDF engine and app built from the ISO 32000 specification. We track PdfCraft closely and
merge its fixes; PdfKopi adds Kopitiam's branding, fixes and features on top.

## Status

Early alpha, like PdfCraft itself. Viewing, search, organizing pages, combining and splitting,
comments, forms, passwords, redaction, basic signatures and printing work today. Editing existing
text, OCR beyond Latin script and Office export are still thin. Known bugs are triaged in the
[issue tracker](https://github.com/kopitiam-io/pdfkopi/issues).

## Build and run

Needs Rust 1.90 or newer ([rustup](https://rustup.rs)).

```sh
git clone https://github.com/kopitiam-io/pdfkopi
cd pdfkopi
cargo run --release -p pdfcraft -- some.pdf   # desktop app
cargo run --release -p pdfcraft-cli -- --help  # command-line tool
```

The internal crates keep their upstream `pdfcraft-*` names so PdfCraft fixes merge cleanly; the
app itself is PdfKopi. Development notes are in [docs/development.md](docs/development.md).

## Feedback

Report bugs and request features on [GitHub](https://github.com/kopitiam-io/pdfkopi/issues).

## License and credits

PdfKopi is dual-licensed under [MIT](LICENSE-MIT) or [Apache-2.0](LICENSE-APACHE), at your option,
as is PdfCraft. Copyright (c) 2026 Kopitiam, and the ArtCraft Team and the PdfCraft contributors.
Required notices are in [NOTICE](NOTICE). Bundled fonts, icons, images and other assets keep their
own open licenses; each is listed with its author, source and license in
[ATTRIBUTION.md](ATTRIBUTION.md).

PdfKopi is not made, sponsored or endorsed by the ArtCraft Team, and carries none of their marks
(see [docs/BRANDING.md](docs/BRANDING.md)).

<sub>Adobe and Acrobat are trademarks or registered trademarks of Adobe Inc. in the United States
and/or other countries. PdfKopi is an independent, open-source project and is not affiliated with,
sponsored by or endorsed by Adobe Inc.; these names are used only to describe compatible
workflows.</sub>
