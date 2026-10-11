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

## What it does

- **Read:** fast rendering, search, bookmarks, thumbnails, dark mode and accessibility checks.
- **Organize:** reorder, rotate, insert, delete, combine and split pages.
- **Review:** highlights, notes, shapes, stamps and other comments.
- **Fill & sign:** fill forms, add signatures, and sign with a digital ID.
- **Secure:** open and set passwords, respect copy restrictions, and redact content permanently.
- **Print and export:** print, optimize file size, and export text.

## Download

PdfKopi will be available from [kopitiam.io](https://kopitiam.io) and from
[GitHub Releases](https://github.com/kopitiam-io/pdfkopi/releases) for macOS, Windows and Linux.
There is no public release yet; until then, build it from source as below.

## Status

Early alpha. Viewing, search, organizing pages, combining and splitting, comments, forms,
passwords, redaction, basic signatures and printing work today. Editing existing text, OCR beyond
Latin script and Office export are still thin. Report bugs to
[support@kopitiam.io](mailto:support@kopitiam.io).

## Build and run

Needs Rust 1.90 or newer ([rustup](https://rustup.rs)).

```sh
git clone https://github.com/kopitiam-io/pdfkopi
cd pdfkopi
cargo run --release --bin pdfkopi -- some.pdf      # desktop app
cargo run --release --bin pdfkopi-cli -- --help    # command-line tool
```

Development notes are in [docs/development.md](docs/development.md).

## Feedback

Report bugs, ask questions and request features at
[support@kopitiam.io](mailto:support@kopitiam.io).

## License and credits

PdfKopi is dual-licensed under [MIT](LICENSE-MIT) or [Apache-2.0](LICENSE-APACHE), at your option.
Required notices are in [NOTICE](NOTICE). Bundled fonts, icons, images and other assets keep their
own open licenses; each is listed with its author, source and license in
[ATTRIBUTION.md](ATTRIBUTION.md).

PdfKopi is built on [PdfCraft](https://github.com/storytold/pdfcraft), an open-source PDF engine
by the ArtCraft Team and the PdfCraft contributors, whose copyright it carries. PdfKopi is not
made, sponsored or endorsed by them and carries none of their marks (see
[docs/BRANDING.md](docs/BRANDING.md)). Inside the source tree the engine crates keep their
upstream `pdfcraft-*` names so upstream fixes merge cleanly.

<sub>Adobe and Acrobat are trademarks or registered trademarks of Adobe Inc. in the United States
and/or other countries. PdfKopi is an independent project and is not affiliated with,
sponsored by or endorsed by Adobe Inc.; these names are used only to describe compatible
workflows.</sub>
