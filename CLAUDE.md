# Day trading workspace

The day-trader skill pack lives in `.claude/skills/trader-*`. Rules are in
`trader/config.json` (paper trading on, $5,000 budget, $50 max loss per
trade, $150 daily loss limit, 3 trades a day). Everything else the skills
write to `trader/` stays out of git.

One trade, in order:
/trader-scanner -> /trader-news -> /trader-entry -> /trader-exit ->
/trader-timemachine -> /trader-budget -> /trader-risk -> /trader-broker,
then /trader-alerts while it is open.

No order is placed without the user's explicit yes for that exact order.
