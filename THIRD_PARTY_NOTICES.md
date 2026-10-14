# Third-party components

- Electron: MIT. Chromium and other third-party notices are included with the Electron distribution.
- PDF.js / pdfjs-dist: Apache-2.0. Copyright Mozilla Foundation and contributors. Includes local CMaps, standard font and WASM resources distributed with pdfjs-dist.
- Markdown-it: MIT. Copyright Vitaly Puzrin, Alex Kocharin and contributors. Used for safe Markdown rendering; its license is included in the packaged dependency.
- KaTeX: MIT. Copyright Khan Academy and contributors. Includes bundled math fonts and associated notices.
- Mammoth: BSD-2-Clause. Copyright Michael Williamson and contributors. Used for local Word text extraction; its LICENSE is included in the packaged dependency.
- JSZip: MIT or GPLv3 (used under MIT). Copyright Stuart Knightley and contributors. Used for local EPUB archive reading.
- @xmldom/xmldom: MIT. Copyright contributors. Used for EPUB XML parsing without executing book content.
- Koffi / @koromix/koffi-darwin-arm64: MIT. Copyright Niels Martignène and contributors. ABI-stable native FFI bridge, used only in the main process to call public AppKit, Accessibility and CoreGraphics APIs. Bundled dependency licenses are retained. Project: https://github.com/Koromix/koffi
- @mozilla/readability: Apache-2.0. Copyright Mozilla and contributors. Extracts article content from user-selected public webpages; bundled license retained.
- linkedom: ISC. Copyright Andrea Giammarchi and contributors. Parses HTML locally without executing webpage scripts; bundled license retained.
- Vite: MIT. Build tool only.
- electron-builder: MIT. Packaging tool only.

Exact dependency versions and transitive packages are recorded in `package-lock.json`. The independent sample lecture is authored for this prototype, and is not an official course document.

Daily quotations are short excerpts from public-domain originals, with author and work identified in the interface. Chinese renderings of Western works are original paraphrases marked 译意. Source addresses are recorded in `src/appearance.mjs`. No commercial translation collection is bundled.

Apple Vision / Accessibility / Core Graphics：通过 macOS 公共系统 API 提供本机文字识别与用户主动触发的区域读取；桥接使用上述 Koffi。系统框架随 macOS 提供，不包含第三方 OCR 云服务。

## Local conversion components

This private build includes unmodified calibre 9.16.0 (GPL-3.0), from https://calibre-ebook.com/ . Its license files and bundled dependencies are retained inside `converters/calibre.app`; corresponding versioned source is available at https://download.calibre-ebook.com/9.16.0/ .

DjVuLibre, libwpd and their runtime libraries are verified Homebrew binary packages. Their exact versions, licenses, SHA-256 hashes and origin URLs are in `converters/native/manifest.json`. Project and source references: https://djvu.sourceforge.net/ , https://libwpd.sourceforge.net/ and https://formulae.brew.sh/ . These tools run only for requested imports.
# Optional offline dictionary data

ECDICT by skywind3000 is offered as an optional user-initiated download under
the MIT license: https://github.com/skywind3000/ECDICT.
The application pins revision 82c9872576b23118d7c42e920c11beb77f510ae2 and saves
the source license with the installed dictionary. Dictionary data is not
included in this application package.


## LibreOffice Community 26.2.6 (Apple Silicon)

Unmodified official LibreOffice.app is bundled for local PPT/PPTX to static PDF conversion. It is not affiliated with Pal. Copyright The Document Foundation and contributors. License notices and third-party licenses remain in LibreOffice.app/Contents/Resources/LICENSE.html and NOTICE.

- Binary: https://download.documentfoundation.org/libreoffice/stable/26.2.6/mac/aarch64/LibreOffice_26.2.6_MacOS_aarch64.dmg
- SHA-256: 94bb3248df074c225490a8a6d1d9dc87c7d6783dbb7a8e9f0d0c3d94348552af
- Corresponding source: https://download.documentfoundation.org/libreoffice/src/26.2.6/
- Licensing information (MPL 2.0 and component notices): https://www.libreoffice.org/about-us/licenses/

No binary modifications were made. The original app bundle, bundled licenses, and notices are distributed intact.
