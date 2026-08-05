# SoundCarrot Translations

This repository contains the translation files used by [SoundCarrot](https://soundcarrot.com), a directory for discovering great kids' podcasts.

The repository exists purely to make SoundCarrot's translation files available to translators and collaborators without exposing the main SoundCarrot codebase.

## Files

- `en.json` — the English source/reference file.
- `es.json` — España.
- `de.json` — Deutsch
- `fr.json` — Français.
- `nl.json` — Nederlands.

Additional languages can be added as separate JSON files using their language code, for example `it.json`.

## Translating

The English file is the source of truth for the wording and structure.

When translating:

- **Keep all JSON keys unchanged.** Translate the values, not the keys.
- **Keep placeholders unchanged.** For example, `{country}`, `{age}`, `{count}`, `{email}`, `{query}`, `{title}`, `{topics}`, `{year}`, `{seasonWord}`, `{n}`, `{plural}` and similar placeholders must remain exactly as written.
- **Keep the JSON valid.** Use normal JSON syntax and escape quotation marks where necessary.
- **Keep the overall structure where possible.** Sections and keys are used by SoundCarrot to find the translated text.
- **Translate naturally.** The goal is good, natural language for the target audience, not a word-for-word translation of the English.
- **Keep the tone.** SoundCarrot is friendly, informal, playful and human rather than corporate or overly formal.
- **Keep proper names unchanged.** This includes SoundCarrot, Team Carrot, Yoto, podcast names, show names and other proper names unless there is an established local version.
- **Keep symbols and UI conventions where they make sense.** Arrows such as `→` and `←`, hearts, and similar interface elements are part of the surrounding UI.
- **Don't translate technical values simply because they appear in a JSON file.** For example, locale-specific slugs may be translated where appropriate.

## A note about context

Some strings are very short and only make sense when you know where they appear on the website. Others are longer pieces of homepage, FAQ or account copy.

If a translation seems ambiguous, check the English wording and the surrounding section first. If it is still unclear, please raise the question rather than guessing.

Some copy is deliberately playful. For example, SoundCarrot uses carrot-related language as part of its personality. A natural equivalent in the target language is preferable to a literal translation when the literal version would sound strange.

## Placeholders

Placeholders are inserted by SoundCarrot when the website is rendered. They must not be translated or removed.

For example:

```text
"recommendedForAges": "{title} is recommended for ages {ages}."
```

A Spanish translation might be:

```text
"recommendedForAges": "{title} está recomendado para {ages}."
```

The surrounding sentence changes, but `{title}` and `{ages}` remain exactly the same.

## Language and regional conventions

The English source is written in British English.

Where a target language has meaningful regional differences, use the most natural wording for families using SoundCarrot in that language. Consistency within a language is more important than following the English structure literally.

## Contributing

If you are contributing a translation:

1. Start from the current `en.json`.
2. Create or update the JSON file for your language.
3. Keep the keys and placeholders intact.
4. Check that the JSON is valid.
5. Submit the translation for review.

Thank you for helping make SoundCarrot more useful to families around the world!
