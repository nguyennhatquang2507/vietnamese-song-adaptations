# Song Adaptation Guidelines

Follow these rules whenever adding or editing a song adaptation. Keep the existing repository structure and do not rename existing song folders or files.

## Creating a song from user-provided lyrics

When the user provides an original song title and its lyrics and asks for a new song:

- Infer the source language from the title and lyrics, and create the song folder under the matching language folder. Use a lowercase, hyphen-separated romanization of the original title when practical.
- Create the complete four-file song structure below and add the song to the language catalog. Do not stop after creating only some of the files.
- Use the original title as supplied. If the user has not provided a Vietnamese title, create a suitable Vietnamese rendering of the title.
- Put the supplied original lyrics in `original-lyrics.md`, preserving their wording and structure. Add the title and a link back to the song README.
- Translate the supplied lyrics into Vietnamese in `literal-translation.md`, prioritizing fidelity to meaning over singability. Add the title and a link back to the song README.
- In `vietnamese-lyrics.md`, add only the original and Vietnamese song title headings and a link back to the song README. Do not write or adapt singable Vietnamese lyrics unless the user asks for that separately.
- Create the song `README.md` using the existing song README structure. Fill in the titles, source and target languages, a concise bilingual introduction based only on the supplied information, status `Draft`, links to all three lyric files, and a link back to the language catalog. Include a reference link only if the user supplies it.
- Do not search for or invent missing credits, reference versions, or other metadata. Omit optional information the user has not provided.

## Folder and file structure

- Put each song under the folder for its source language, such as `Chinese/`.
- For a new song folder, use a lowercase, hyphen-separated romanization of the original title when practical. Check for an existing folder first; preserve established names and links.
- Each language folder must have a `README.md` with a brief description of the collection and a catalog of its songs, linking to each song's `README.md`.
- The root `README.md` lists language collections and links to each language folder's `README.md`. Keep song-level catalog entries in the corresponding language folder, not the root catalog.
- Every song folder must contain:
  - `README.md` — original and Vietnamese titles, source and target languages, adaptation status, a reference link only when supplied, a short bilingual introduction, links to all three lyric files, and a link back to the language folder's `README.md`.
  - `original-lyrics.md` — the original lyrics in their source language, with the title and a link back to the song README.
  - `literal-translation.md` — a meaning-focused translation into Vietnamese, with the title and a link back to the song README.
  - `vietnamese-lyrics.md` — the original and Vietnamese song title headings, and a link back to the song README. Add adapted lyrics only when requested.
- Use relative links between files. Follow the bilingual presentation and Markdown style of nearby song folders.

## Adaptation and accuracy

- Aim to preserve the original meaning, emotional tone, and singability in Vietnamese. Prefer natural Vietnamese phrasing that fits the song's melody and rhythm.
- Keep the literal translation distinct from the singable adaptation: the former prioritizes meaning; create the latter only when the user asks, prioritizing natural, performable lyrics while retaining the spirit of the original.
- Do not invent lyrics, credits, status, or reference links. Mark unknown information appropriately or omit optional details.
- Only add or reproduce lyrics when they are provided by the user or the user has confirmed they may be used. Do not fetch or reproduce copyrighted lyrics from external sources.
- Preserve the source-language text as supplied; do not silently "correct" uncertain wording. Note uncertainties for review.
- New songs start with status `Draft`; do not mark them completed until the user requests finalization and the adaptation is ready to use.

## Catalog and final checks

- Add each new song to the catalog in its language folder's `README.md`, using the original and Vietnamese titles and linking to the song `README.md`. Add a new language collection to the root `README.md` when needed.
- Before finishing, verify that all four song files exist, every relative link resolves, both catalog levels point to the right locations, and the status reflects the actual state of the adaptation.
- Do not mark an adaptation completed or place it among finalized work unless it has been reviewed and is ready to use.
