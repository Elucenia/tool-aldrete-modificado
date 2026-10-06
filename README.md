# Índice de Aldrete modificado

ELUCENIA · Felipe Guedes. Self-contained per-tool calculation and demonstration.

## Documentation in ten languages

- [Português (Brasil)](documentation/pt-BR.md) · [ELUCENIA](https://elucenia.org/pt-br/ferramentas/aldrete-modificado)
- [English](documentation/en.md) · [ELUCENIA](https://elucenia.org/en/tools/aldrete-modificado)
- [Español](documentation/es.md) · [ELUCENIA](https://elucenia.org/es/herramientas/aldrete-modificado)
- [Français](documentation/fr.md) · [ELUCENIA](https://elucenia.org/fr/outils/aldrete-modificado)
- [Deutsch](documentation/de.md) · [ELUCENIA](https://elucenia.org/de/werkzeuge/aldrete-modificado)
- [Italiano](documentation/it.md) · [ELUCENIA](https://elucenia.org/it/strumenti/aldrete-modificado)
- [العربية](documentation/ar.md) · [ELUCENIA](https://elucenia.org/ar/tools/aldrete-modificado)
- [中文](documentation/zh.md) · [ELUCENIA](https://elucenia.org/zh/tools/aldrete-modificado)
- [日本語](documentation/ja.md) · [ELUCENIA](https://elucenia.org/ja/tools/aldrete-modificado)
- [हिन्दी](documentation/hi.md) · [ELUCENIA](https://elucenia.org/hi/tools/aldrete-modificado)

The README introduction is in English; the linked usage, field, method, limits, source and review documentation is available in each listed language. Bibliographic titles and schema identifiers retain their source identity.

## Local use and tests

Serve this directory with a static HTTP server and open index.html. All calculation and presentation run locally; no remote calculation API, account, dependency install, application source tree or database is required. Node: `require("./calculator.js").calculate(input)`. Run `npm test` for original reference and refusal tests, source-output preservation and presentation in all ten languages. Tests verify the immutable package and write no files.

## Edition and current implementation

Method: Modified Aldrete 1995:5 itens 0–2, Sp O 2 substituicor, total 0–10

Implementation: `aldrete-modificado@native-2026-10-05+53d8efad5f85`. The mathematical body, inputs, formula and original numeric references are unchanged. The existing verdict, level, note and detail rows are exposed without adding a threshold or recommendation. The browser demonstration uses the same pinned pure presentation helpers and whole-source, per-tool templates as the platform. Ten authorial interface and documentation editions are included; an unknown clinical phrase keeps explicit source-language attribution.

## Evidence and limits

`source-result-contract.json` records the output-preservation comparison against the same historical method. `documented-result-examples.json` records rendering of those synthetic outputs; neither is an independent clinical oracle. `publication-provenance.json` pins current code, source identity, translations and their independent static review. Historical served proofs remain in evidence with their original revision. Separate current DEV API and representative standalone browser checks are required before publication; no production or clinical approval is inferred.

## Sources and component licences

Scientific sources, inputs, units, conditions and formula remain in tool.json and the ten documentation files. The nine original public legal, attribution and policy files are preserved byte for byte. CODE-COMPONENTS.md maps the preserved software licences; SOURCE-RIGHTS-REVIEW.md separates source-specific instrument wording, questionnaires, datasets and translation conditions. Software tests and software licences do not establish whole-instrument permission, official endorsement, clinical validation or professional language approval.
