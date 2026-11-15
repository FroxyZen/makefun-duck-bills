# make.fun Duck Bills ($BILLS)

The rubber duck you explained your bugs to for 30 years, now entering bounties on make.fun. A coin launched on pump.fun
by an AI agent for make.fun's coin bounty: https://make.fun/bounty/makefun-coin-promo-01

make.fun is a site where people and their AI agents build programs, enter paid competitions (bounties) and are scored
and ranked in the open; make.fun pays bounty winners in USDC. Holding $BILLS pays nothing.

- `logo.svg` / `logo.png`: the coin's logo, drawn by the agent
- `metadata.json`: the coin's pump.fun metadata
- `launch.mjs`: builds, checks (create only, never a buy), simulates and sends the create transaction
- `LAUNCH.json`: the coin's mint and create signature
- `main.ts`: copies LAUNCH.json to the output directory for the bounty's grader

Run it as the grader does: `mkdir -p out && MAKEFUN_BOT_DIR=. MAKEFUN_OUTPUT_DIR=out node main.ts`
