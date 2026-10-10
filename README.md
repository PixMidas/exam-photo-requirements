# Exam and public-service photo and file requirements (Brazil)

A small, sourced dataset of the file rules that applicant portals enforce on uploads: accepted formats, size limits and, where published, dimensions. Each row points to the official edital PDF or service page it was read from, with the clause number when the source has one. No blogs, no forum answers.

Each row carries its own `last_verified` date. Editais can be rectified and portals change; check the source before relying on a row.

## What the data shows

- There is no single "FGV rule" or "Cebraspe rule". Each edital sets its own limit. Among the FGV photo rows, three cap the photo at 1 MB and one (DPGE-RJ XXIX) allows 5 MB and also accepts PDF.
- Accepted formats differ between institutions. FGV photo rows accept JPEG/JPG only, while Cebraspe (PC-PE 1/2023) also accepts PNG. A file that passes one upload can be refused by another.
- Detran-SP's recurso de multa (JARI) flow does not list JPG or PNG among accepted formats. A photo has to be turned into a PDF first.
- Detran-SP vehicle services limit each attachment to 1.2 MB and all attachments together to 15 MB.

## Files

- `requirements.csv` and `requirements.json`: the same data in two formats.

Fields: `id`, `process`, `organization`, `issuer`, `country`, `document_type`, `section` (clause in the source), `accepted_formats`, `max_size_mb`, `max_files`, `max_total_mb`, `dimensions`, `other_rules`, `source_url`, `last_verified`. Empty means the source does not state it.

## Method

Primary sources only: the published edital PDF or the official service page, read for the upload rule. The clause number lets you check a row in under a minute. Rows are written by hand, not scraped.

## Not included, on purpose

- gov.br account verification: it uses live camera capture, not a file upload.
- Cebraspe's public upload page publishes no numeric limit; the number is in each edital.
- ENEM 2026 has no candidate photo upload at registration.
- Rules that sit only behind a login are not published here unless an official document states them.

## License

CC BY 4.0, see `LICENSE`. Use it freely, including commercially. Please credit "PixMidas" and link to https://www.pixmidas.com.

## Corrections

Found a rule that changed? Open an issue with the source link and clause number.

Maintained by [PixMidas](https://www.pixmidas.com), free browser tools that process files on your own device.
