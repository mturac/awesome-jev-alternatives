# Contributing

This list collects open alternatives and building blocks for System One style decision models: fast, typed yes/no, choice, and score judgments. TypeSafe AI's Jev is the closed reference. Software that only calls hosted Jev belongs in an awesome-jev catalog.

## Inclusion

Add an entry only when all of these hold:

- The project is open source, or it is self-hostable code at a public URL. A GitHub license API result of `NOASSERTION` is acceptable only when the LICENSE file itself is a recognizable open-source license.
- The link returns HTTP 200.
- A GitHub repository is not archived, and its default branch was pushed within the last 365 days. Older work is included only when it is the reference for a method still in use. Those exceptions live in `HISTORICAL` inside `scripts/check_links`, and the entry says that it is historical.
- One sentence can say what it is and what you give up relative to hosted Jev. Do not copy benchmark numbers from a README unless this repository re-ran them.
- It is a decision engine, a runtime or port, a zero-shot classifier used as a typed decision, calibration or evaluation tooling, a dataset or benchmark, or a paper on fast calibrated judgments or logprob classification.

## Exclusion

- Applications whose decision step is a call to hosted Jev.
- Private repositories. `mturac/jskills` is out.
- Archived repositories, empty repositories, and repositories with no license file when the code is meant to be reused.
- Repositories with no push in 365 days, other than the historical exceptions named above.
- General structured-generation libraries, generic language-model evaluation harnesses, and memory systems.
- Anything that cannot be verified. Put that name in the pull request under "Excluded / unverified", not in the README.

## Adding an entry

1. Put one bullet in the matching section, in alphabetical order by the link text, using `- [Name](https://example.com) - What it is, and the tradeoff.`
2. Start the description with a capital letter and end it with a period.
3. Run `python3 scripts/check_links` and `npx awesome-lint`. awesome-lint 2.3.0 also reports missing GitHub topics (`awesome`, `awesome-list`) and a license GitHub has not detected on the default branch. Those are repository settings. Do not treat them as README failures.

## License

Contributions are accepted under [CC0-1.0](https://creativecommons.org/publicdomain/zero/1.0/).
