# Northern lights odds by place, month and length of stay (Fairbanks, Abisko, Reykjavík, Keflavík)

For each place, month (September to April; Abisko September to March), aurora level and stay of 1 to 14 consecutive nights, the share of real runs of nights in the historical record that included at least one clear evening hour while the aurora was active at that level. Levels are Kp 1 or more (faint), Kp 2 or more (a proper display) and Kp 3 or more (a strong show), each during a clear hour in the evening window. Next to each figure is the chance the usual independent-nights formula gives, so the gap caused by runs of cloudy nights can be seen directly. Weather comes from hourly airport reports at Fairbanks (PAFA), Reykjavík (BIRK) and Keflavík (BIKF) via the Iowa Environmental Mesonet, and SMHI station 188790 at Abisko; geomagnetic activity is the GFZ Kp index. Records cover 26–27 seasons at Fairbanks (from 2000), 14–15 at Reykjavík and Keflavík (from 2012) and 7 at Abisko (from 2019). 1,302 rows. This is not a forecast.

- Method: https://northernlightsplanner.com/methodology/
- Dataset page: https://northernlightsplanner.com/data/
- Calculator: https://northernlightsplanner.com/northern-lights-odds-calculator/

## Files

- `aurora-odds.csv`: the table, one row per place × month × level × nights.
- `aurora-odds.json`: the same figures in the shape the calculator reads.
- `datapackage.json`: column types (Frictionless Data Package).

## Columns

| Column | Meaning |
|---|---|
| `place` | Fairbanks, Abisko, Reykjavík or Keflavík |
| `country` | Country (and state for Fairbanks) |
| `month` | Sep–Apr (Abisko Sep–Mar) |
| `level` | 1, 2, 3 = Kp 1+, 2+, 3+ in a clear evening hour |
| `nights` | Length of stay, 1–14 consecutive nights |
| `chance_real_runs` | Share of real runs of that many nights with at least one qualifying hour (0–1) |
| `chance_simple_formula` | The same chance if nights were independent (0–1) |
| `seasons` | Number of seasons counted |
| `years` | Span of seasons counted |

`years` is the span of seasons counted. A season runs September to April and is named by its start and end year, so 2000-2026 means the seasons 2000–01 to 2025–26. September has one more season than the other months (for example 2000-2027, 27 seasons at Fairbanks) because September 2026, the first month of the 2026–27 season, is already observed.

## Limits

One weather station per place; airport cloud sensors miss thin high cloud, so clear-sky figures are if anything slightly generous; Abisko has 7 winters of records, so its figures are less certain than Fairbanks'.

## Licence and credit

CC BY 4.0 (see `LICENSE`). Credit: "Northern Lights Planner (northernlightsplanner.com), Deepak R".

Upstream: Kp index from GFZ German Research Centre for Geosciences, CC BY 4.0 (Matzka et al. 2021, doi:10.1029/2020SW002641; doi:10.5880/Kp.0001); Abisko cloud from SMHI open data, CC BY 4.0, processed; airport reports from the Iowa Environmental Mesonet, Iowa State University (public domain, attribution appreciated).

## Keywords

aurora, northern lights, aurora borealis, Kp index, geomagnetic activity, cloud cover, Fairbanks, Iceland, Reykjavík, Abisko, travel planning, tabular, csv

## Citation

R, Deepak (2026). *Northern lights odds by place, month and length of stay* (v1.0.0) [Data set]. Northern Lights Planner. DOI: pending (Zenodo).

Update frequency: once a season.
