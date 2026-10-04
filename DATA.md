# Data

Use the three original TripleTen / Y.Afisha educational datasets supplied with the project. Create `data/` and place these CSVs inside:

- `visits_log_us.csv`: 359,400 sessions; Uid, Device, Start Ts, End Ts, Source Id.
- `orders_log_us.csv`: 50,415 orders; Uid, Buy Ts, Revenue.
- `costs_us.csv`: 2,542 daily source expenses; source_id, dt, costs.

Visits and expenses cover June 2017 through May 2018. Orders extend briefly into June 1, 2018. No currency is assumed beyond the units of the supplied revenue and cost fields. Raw files are not redistributed; obtain them through authorized course access.

## Quality and attribution

Two negative session durations are excluded from duration metrics while the session records remain in activity counts. One user's first-session timestamp is tied; stable ordering of the input rows selects one source. All 50,415 orders match a unique first-observed source through a validated many-to-one left join. Missing source costs remain unknown rather than being treated as zero.

## File fingerprints

- `costs_us.csv`: `f6e47f518201ea38e2cab930b8759e4afbdda36e18325ca2cb3832eacaeaa639`
- `orders_log_us.csv`: `d06042bc76612758ea48900eb471f1b249ecaf16e5047dbcd80862e440a9ac86`
- `visits_log_us.csv`: `421674ac4cdac63b34ce87e13b057083f3f2fb8bbd56439763acfc8de36265d2`
