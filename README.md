# Unit 1 · The Business Letter

[Open the lesson](https://ij-teacher.github.io/business-letter-unit1/) · [Teacher attendance](https://ij-teacher.github.io/business-letter-unit1/teacher.html)

Based on **U1 The Complete Template of a business letter (AI).docx** supplied by the instructor.

## Contents
- Interactive complete letter with 15 explained parts
- Six special notations and ten business vocabulary words
- Three practice activities (multiple choice, matching, sentence completion)
- Student-ID-only check-in and teacher attendance CSV export
- Printable/downloadable class QR code in `assets/class-qr.png`
- Unchanged original Word document and extracted study notes in `materials/`
- Attendance service source in `attendance-service-source.zip`

## Attendance
The website and teaching materials are hosted on GitHub Pages. Because Pages is static, check-ins are submitted to a separate Sites service backed by a private D1 database. Only student ID, Taipei day, server timestamp and a record identifier are stored. Student IDs and teacher credentials are **never committed to this repository**.

Students do not need an account or password. IDs are self-reported, not verified identities. One check-in per student per Taipei calendar day is retained; repeat submissions return the existing check-in. Exercises run on the student's device and are not collected.

Open `teacher.html`, enter the private teacher key provided locally to the instructor, select the date, and export CSV. The key remains only in the page memory and is cleared with **Lock**. The service holds only its SHA-256 hash in a protected environment variable. The record API verifies the key on every request.

If the service is unavailable, the site displays **Not confirmed**, preserves the entered ID and never claims a record was saved. The lesson can still be read.

## Teaching notes
The original handout is unchanged. Interactive activities clarify “meet standards” and accept **collaborating** where the sentence requires it. “Stamp” is a postage stamp in the envelope question and an official mark in the vocabulary definition. Optional letter lines reflect this particular model.

## Updating
Edit the HTML/CSS/JS or replace lesson materials, then push to `main`. GitHub Pages serves the repository root. QR destination: https://ij-teacher.github.io/business-letter-unit1/

For the attendance service, extract its source archive, install dependencies and deploy with Sites using its D1 migrations. Configure `TEACHER_KEY_HASH` as a secret; never put the teacher key in the public website or repository.

## Validation
Local integration tests cover saved check-ins, duplicate prevention, invalid IDs, unauthorized record access, all exercise answer keys, reset controls, responsive layout, QR display, and the letter-explanation WebMCP tool.
