# Data Science Take-Home: Product Sales Estimation

Welcome, and thanks for taking the time to work through this with us.

## What this is

This is an open-ended data problem drawn from real work the Data Science team
does at Jungle Scout: estimating Amazon product demand. We've reduced it to a
toy version so you can complete it in a short sitting.

**We are far more interested in your reasoning and approach than in model
accuracy.** A simple, well-justified model paired with clear thinking about the
data will score better than a complex model with no explanation. There is no
single "right" answer, and we do not expect a polished, production-grade result.

## The problem

You are given a snapshot dataset describing a set of Amazon products and the
units they sold over a fixed 7-day window. **Your task is to build a model that
estimates a product's daily sales from attributes known about that product.**

How you define the target, which attributes you use, which model you choose, and
how you evaluate it are all up to you — and explaining *why* you made each of
those choices is the main thing we're assessing.

## The data

A single file, `df_sales_trend.parquet`, with one row per product observation:

| Column          | Description                                                       |
| --------------- | ----------------------------------------------------------------- |
| `date`          | Start date of the observation window                              |
| `country`       | Amazon marketplace (e.g., `us`, `ca`, `mx`, `fr`)                 |
| `category_code` | Product category (e.g., `kitchen`, `toys`, `electronics`)         |
| `rank`          | Product's sales rank in its category — **lower = better-selling** |
| `units_sold`    | Units sold over the observation window                            |
| `duration`      | Length of the observation window, in days                         |
| `asin`          | Amazon product identifier                                         |

The data is a toy sample and, like real data, is imperfect. Part of the exercise
is diagnosing it. Feel free to state any assumptions you make.

## What to hand back

1. **A notebook or script** that runs top to bottom and produces your model and
   its evaluation. Any language/library is fine. Feel free to use whichever 
   packages are necessary. Please include necessary visualizations to explain your though process.
2. **A short written summary (~1 page)** covering:
   - How you framed the problem and defined your target
   - What you found when you explored the data, and how you handled it
   - Your modeling choice and the trade-offs behind it
   - How you evaluated the model and which metric you chose (and why)
   - The main limitations of your result and what you'd do next with more time/data
3. **Your chosen evaluation metric and the reasoning for it.**

The write-up matters at least as much as the code.

## Time and logistics

- Please treat this as a **~3–4 hour focused effort**. It's fine to stop before
  it feels "finished" — tell us what you'd have done with more time instead of
  grinding to polish it.
- Submit within **3 business days** of receiving this. If you have any questions about 
  the set-up, please share those within **1 day** of receiving the test.
- You may use any tools you like, including AI assistants. The only requirement
  is that you can **explain and defend every decision** in a short follow-up
  conversation, where we'll act as a colleague reviewing your work with you.

Good luck — and please reach out if anything is unclear.
