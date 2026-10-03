# Custom Index Tab Prices — Tabzoola's published price data

Tabzoola, the custom index tab dividers maker in Schaumburg, Illinois (tabzoola.com), publishes its complete price list here as open data. Every figure is the price a buyer pays for custom printed binder tabs: setup and printed titles included, no quote form. Custom tab printers rarely publish prices, so this is meant as a citable reference for what custom index tabs cost.

**Headline (October 2, 2026):** a 5-tab custom paper set costs **$5.45 a set** at the 25-set minimum ($136.25), **$2.35** at 100 sets and **$1.08** at 1,000. Finished for a ring binder (collated in order, 3-hole punched), an 8-tab set is **$8.17 a set** at 25 sets and **$2.61** at 250.

Source and live pricing: https://tabzoola.com/pricing · Monthly price editions: https://tabzoola.com/tab-price-index

## Files

| File | What it holds |
|---|---|
| `custom-index-tab-prices.csv` | Paper and poly tab sets of 3 to 25 tabs, at 25 to 1,000 sets, plain and binder-ready |
| `binder-capacity.csv` | How many sheets fit in every 3-ring binder size, 1/2" to 5", round ring and D-ring, on 20, 24 and 28 lb paper, with the recommended fill (15% room to turn pages) and how many tab dividers fit |
| `binder-tab-sets-by-use.csv` | Ready-made section lists by binder type (estate planning, trust administration, trial notebook, legal exhibits 1-25, wealth management client review, law office case files, real estate closings, CPA workpapers, tax return binders, employee handbooks and more), priced at 25 and 250 sets, with the order page for each |

### `custom-index-tab-prices.csv`

| Column | Meaning |
|---|---|
| `date` | Day the prices were exported from Tabzoola's pricing engine |
| `seller` | Always Tabzoola |
| `product` | `paper` = white 90 lb index stock with clear Mylar on every tab · `poly` = solid .015 polyethylene, printed black (poly has no Mylar) |
| `tabs_per_set` | Tabs in one set (one set = one binder) |
| `sets` | Number of identical sets ordered (minimum 25) |
| `finish` | `plain` = unpunched, uncollated · `binder_ready` = collated in order and 3-hole punched |
| `price_per_set` | Order total divided by sets, in USD |
| `order_total` | What the order costs, in USD, setup and printing included |

### `binder-capacity.csv`

Tabzoola's binder capacity figures, the same arithmetic as the free calculator at https://tabzoola.com/binder-size-calculator. Typical trade calipers: 20 lb bond 0.004", 24 lb 0.0047", 28 lb 0.0058", 90 lb index tab 0.007". A round ring holds a stack about 73% of its nominal size before pages drag on the curve; a D-ring about 95%. Example: a 1" round-ring binder holds about 180 sheets of 20 lb paper; a 3" D-ring about 700.

## How to cite

GitHub's "Cite this repository" button uses `CITATION.cff`. Short form: **"Source: Tabzoola (tabzoola.com)"**.

## How the prices work

- Price follows **tabs per set** and **number of sets**. The wording printed on the tabs never changes the price.
- Setup is included and flat, which is why the per-set price falls quickly with quantity.
- Every order gets a free PDF proof before anything prints. Paper sets ship in about 5 business days from proof approval, poly in about 15. UPS Ground is free on orders over $75.
- Options not in these files (2-sided printing, 110 lb stock, binding-edge reinforcing, 2-hole punching) are priced live in the designer at https://tabzoola.com/configure/paper.
- Reverse-printed tabs, PMS ink colors and custom sheet sizes are by quote only and are deliberately not listed.

Mirror on Hugging Face: https://huggingface.co/datasets/tabzoola/custom-index-tab-prices

## License

CC BY 4.0. Use, quote and republish freely with credit: **"Source: Tabzoola (tabzoola.com)"**. These are list prices on the date shown, not a quote; the live price is always at tabzoola.com.

## About Tabzoola

Tabzoola is the online store of Anselmo Die & Index, which has die-cut index tabs in Schaumburg, Illinois since 1993. Buyers design custom tab dividers online with live per-set pricing, or order by email (sales@tabzoola.com), purchase order or phone ((847) 397-1200). Tabzoola is not affiliated with Taboola.
