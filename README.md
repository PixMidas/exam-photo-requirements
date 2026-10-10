# Exam and public-service photo requirements (Brazil)

A small, sourced dataset of the file rules that applicant portals enforce on photo uploads. Every row was read from the official edital PDF, with the section number recorded. No blogs, no forum answers.

**Last verified:** 2026-09-20. Editais can be rectified; check the source before relying on a row.

## Why this exists

There is no single "FGV rule" or "Cebraspe rule". Each edital sets its own limit, and the accepted formats differ by banca:

- FGV editais in this dataset accept JPEG/JPG only. Three cap the photo at 1 MB, one (DPGE-RJ XXIX) allows 5 MB and also PDF.
- Cebraspe (PC-PE 1/2023) also accepts PNG, caps the image at 1 MB and requires a photo taken within the previous six months.

A PNG that passes one upload can be rejected by another with no useful error message.

## Files

- `requirements.csv` and `requirements.json`: the same data in two formats.

Fields: `id`, `process`, `organization`, `banca`, `country`, `document_type`, `section` (clause in the edital), `accepted_formats`, `max_size_mb`, `other_rules`, `source_url`, `last_verified`.

## Method

Primary sources only: the published edital PDF, read for the upload clause. The section number lets you check each row in under a minute. Rows are not scraped.

## Not included, on purpose

- gov.br: no file upload exists in the account verification flow.
- Cebraspe's public upload page publishes no numeric limit; the number is in each edital.
- Rules that only appear behind a login are not published here unless an official document states them.

## License

CC BY 4.0. Use it freely, including commercially. Please credit "PixMidas" and link to https://www.pixmidas.com.

## Corrections

Found a rule that changed? Open an issue with the edital link and section number.

Maintained by [PixMidas](https://www.pixmidas.com), free browser tools that process files on your own device.
