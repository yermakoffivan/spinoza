# Nightly 2026-10-17 — regression

Commit `d0cd2415da7f`, triggered by schedule. [Run](https://github.com/yermakoffivan/spinoza/actions/runs/39012580426)

| | this run | |
|---|---|---|
| jobs | 89 | 2 failed |
| job-minutes | 730.4 (-92.4) | |
| e2e coverage | 65% (-0.2) | |
| mutation score | 100% (no change) | 7824 killed, 0 lived |
| flaky | 1 (no change) | passed only on retry |
| uncovered mutants | 341 (no change) | records across reported build variants |

Mutation score is killed / (killed + lived). Uncovered mutants are excluded from that score; some are uninstrumented constant expressions.

## Separate system coverage

These suites retain their own Go statement denominators. The browser E2E coverage above is unchanged by these profiles.

| suite | covered / total statements | coverage |
|---|---|---|
| cluster-mode-auth | 5250 / 22065 | 23.8% |
| cluster-mode-chromium | 4121 / 22065 | 18.7% |
| cluster-mode-firefox | 4119 / 22065 | 18.7% |
| cluster-mode-webkit | 4116 / 22065 | 18.7% |
| mcp-cli | 833 / 22226 | 3.7% |

## New failures

- cluster-mode-release
- install

## Fixed since the last run

- e2e / visual-accessibility / chromium

## Failing

- cluster-mode-release
- install

## Flaky

| test | file | project | attempts |
|---|---|---|---|
| at 200% browser zoom › the whole workspace stays reachable by scrolling | specs-full/viewport.spec.ts:89 | webkit | 2 |

## Jobs

| job | result | minutes |
|---|---|---|
| cluster-mode-release | skipped | 0 |
| e2e / checks-issues-worklist / chromium | success | 7.4 |
| e2e / checks-issues-worklist / firefox | success | 7.2 |
| e2e / checks-issues-worklist / webkit | success | 7.9 |
| e2e / cluster mode / chromium | success | 6.3 |
| e2e / cluster mode / firefox | success | 6 |
| e2e / cluster mode / webkit | success | 6.6 |
| e2e / cluster-mode-auth | success | 10.2 |
| e2e / distribution-desktop-install | success | 0.1 |
| e2e / e2e-coverage | success | 0.3 |
| e2e / foundation-security / chromium | success | 3.7 |
| e2e / foundation-security / firefox | success | 3.7 |
| e2e / foundation-security / webkit | success | 3.8 |
| e2e / gitops / chromium | success | 9.5 |
| e2e / gitops / firefox | success | 10.9 |
| e2e / gitops / webkit | success | 11.1 |
| e2e / helm / chromium | success | 4.1 |
| e2e / helm / firefox | success | 4.5 |
| e2e / helm / webkit | success | 4.3 |
| e2e / inspect-compare-rbac-topology / chromium | success | 8.9 |
| e2e / inspect-compare-rbac-topology / firefox | success | 9.4 |
| e2e / inspect-compare-rbac-topology / webkit | success | 9.5 |
| e2e / mcp-cli | success | 3.4 |
| e2e / multicluster-fleet / chromium | success | 8.5 |
| e2e / multicluster-fleet / firefox | success | 8.9 |
| e2e / multicluster-fleet / webkit | success | 10.4 |
| e2e / mutations-protection-history / chromium | success | 4.5 |
| e2e / mutations-protection-history / firefox | success | 4.5 |
| e2e / mutations-protection-history / webkit | success | 5 |
| e2e / navigation-interaction / chromium | success | 10.3 |
| e2e / navigation-interaction / firefox | success | 10.8 |
| e2e / navigation-interaction / webkit | success | 11.5 |
| e2e / observability-traffic / chromium | success | 3.7 |
| e2e / observability-traffic / firefox | success | 3.5 |
| e2e / observability-traffic / webkit | success | 3.8 |
| e2e / outage / chromium | success | 3.6 |
| e2e / outage / firefox | success | 3.6 |
| e2e / outage / webkit | success | 3.5 |
| e2e / resilience-capacity-soak / chromium | success | 8.9 |
| e2e / resilience-capacity-soak / firefox | success | 8.2 |
| e2e / resilience-capacity-soak / webkit | success | 8.5 |
| e2e / resources-live-tables / chromium | success | 9.4 |
| e2e / resources-live-tables / firefox | success | 8.3 |
| e2e / resources-live-tables / webkit | success | 10.2 |
| e2e / select | success | 0.2 |
| e2e / streams-terminals-forwards / chromium | success | 4.7 |
| e2e / streams-terminals-forwards / firefox | success | 4.9 |
| e2e / streams-terminals-forwards / webkit | success | 5.5 |
| e2e / suite-contract | success | 0.4 |
| e2e / visual-accessibility / chromium | success | 13.4 |
| e2e / visual-accessibility / firefox | success | 14.8 |
| e2e / visual-accessibility / webkit | success | 14.9 |
| fuzz / fuzz (., FuzzServingCheckPublicURL) | success | 11.4 |
| fuzz / fuzz (./internal/access, FuzzDecisionAggregation) | success | 10.8 |
| fuzz / fuzz (./internal/auth, FuzzRoleAuthorization) | success | 10.3 |
| fuzz / fuzz (./internal/charts, FuzzChartIndex) | success | 10.4 |
| fuzz / fuzz (./internal/charts, FuzzFetchableRepositoryURL) | success | 10.4 |
| fuzz / fuzz (./internal/checks, FuzzParseRules) | success | 10.4 |
| fuzz / fuzz (./internal/issues, FuzzCursor) | success | 10.3 |
| fuzz / fuzz (./internal/mcp, FuzzProtocol) | success | 10.6 |
| fuzz / fuzz (./internal/mcp, FuzzStdioFraming) | success | 10.6 |
| fuzz / fuzz (./internal/store, FuzzHistoryLimit) | success | 10.8 |
| fuzz / fuzz (./internal/store, FuzzTimelineCellsRoundTrip) | success | 10.8 |
| install | skipped | 0 |
| mutation / mutation (checks-a-e) | success | 11 |
| mutation / mutation (checks-f-j) | success | 9.9 |
| mutation / mutation (checks-k-o) | success | 9.4 |
| mutation / mutation (checks-p-r) | success | 10 |
| mutation / mutation (checks-s-t) | success | 9.7 |
| mutation / mutation (checks-u-z) | success | 5.2 |
| mutation / mutation (cmd) | success | 1 |
| mutation / mutation (internal-a-d) | success | 15.9 |
| mutation / mutation (internal-e-l) | success | 28.8 |
| mutation / mutation (internal-m-r) | success | 15 |
| mutation / mutation (internal-s-z) | success | 8.4 |
| mutation / mutation (resources-a-f) | success | 5.3 |
| mutation / mutation (resources-g-l) | success | 1.1 |
| mutation / mutation (resources-m-r) | success | 13.4 |
| mutation / mutation (resources-s-z) | success | 3.8 |
| mutation / mutation (root-default) | success | 5.7 |
| mutation / mutation (root-desktop) | success | 4.5 |
| mutation / mutation (server-a-c) | success | 20.7 |
| mutation / mutation (server-d-e) | success | 6.7 |
| mutation / mutation (server-f) | success | 14.7 |
| mutation / mutation (server-g-l) | success | 19.1 |
| mutation / mutation (server-m-r) | success | 10.9 |
| mutation / mutation (server-s-z) | success | 32.1 |
| mutation / mutation-total | success | 0.1 |
| repeat | success | 4 |
