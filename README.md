# UK bank probate limits

How much each UK bank, building society and investment platform will release to an executor without a grant of probate. Every figure was read on the firm's own website, and each row gives the page it came from and the date it was checked.

- 95 banks and building societies, and 16 investment platforms
- 78 with a published figure; the rest publish none, or say they always ask for a grant
- Checked between 4 and 9 November 2026

Maintained by [Probate Checklist](https://probatechecklist.co.uk), a free probate plan for executors in England and Wales. Each firm has a page there with its limit, its own words and how to tell it about a death, for example [Barclays](https://probatechecklist.co.uk/bank-probate-limits/barclays), [Nationwide](https://probatechecklist.co.uk/bank-probate-limits/nationwide) and [HSBC](https://probatechecklist.co.uk/bank-probate-limits/hsbc). The full list, with a checker for several banks at once, is at [probatechecklist.co.uk/bank-probate-limits](https://probatechecklist.co.uk/bank-probate-limits).

## Files

- `probate-limits.csv`: one row per firm
- `probate-limits.json`: the same rows as JSON

| Column | Meaning |
|---|---|
| `id` | Short name, as used in the Probate Checklist page address |
| `name` | The firm |
| `kind` | `bank` (banks and building societies) or `investment platform` |
| `limit_gbp` | The most it releases without a grant, in pounds, for money in the person's sole name. Blank when it publishes no figure |
| `limit_no_will_gbp` | A lower figure where there is no will, if the firm gives one |
| `always_needs_grant` | `true` when the firm says it always asks for a grant, whatever the amount |
| `may_ask_over_limit` | `true` when the firm says it *may* ask for a grant above the limit, rather than always |
| `note` | What else to know, in plain English |
| `quote` | The firm's own words for its limit, copied exactly from `source_url` |
| `source_url` | The page or PDF the figure was read on |
| `checked` | The date it was read, as YYYY-MM-DD |
| `details` | The firm's page on Probate Checklist |

## Things to know

- A limit is per firm, for all of the person's accounts there added together, and only for money in their sole name. Joint accounts usually pass to the other holder without a grant.
- Firms can ask for a grant below their limit, and some decide case by case. The limit is the firm's policy, not a legal rule.
- Firms change their limits without notice. Check `source_url` before relying on a figure.
- This is guidance, not legal advice.

## Corrections

If a figure has changed, open an issue with the firm's page and the new figure.

## Licence

[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). You can reuse the data, including commercially, if you credit Probate Checklist with a link to https://probatechecklist.co.uk.
