# Nightly 2026-10-10 — regression

Commit `84db3f3aff5c`, triggered by schedule. [Run](https://github.com/yermakoffivan/spinoza/actions/runs/38039480169)

| | this run | |
|---|---|---|
| jobs | 89 | 2 failed |
| job-minutes | 830.2 (-19.5) | |
| e2e coverage | 65.1% (no change) | |
| mutation score | 100% (no change) | 7809 killed, 0 lived |
| flaky | 1 (no change) | passed only on retry |
| uncovered mutants | 341 (no change) | records across reported build variants |

Mutation score is killed / (killed + lived). Uncovered mutants are excluded from that score; some are uninstrumented constant expressions.

## Separate system coverage

These suites retain their own Go statement denominators. The browser E2E coverage above is unchanged by these profiles.

| suite | covered / total statements | coverage |
|---|---|---|
| cluster-mode-auth | 5245 / 22027 | 23.8% |
| cluster-mode-chromium | 4109 / 22027 | 18.7% |
| cluster-mode-firefox | 4112 / 22027 | 18.7% |
| cluster-mode-webkit | 4113 / 22027 | 18.7% |
| mcp-cli | 833 / 22188 | 3.8% |

## New failures

- cluster-mode-release
- install

## Fixed since the last run

- fuzz / fuzz (./internal/charts, FuzzChartIndex)

## Failing

- cluster-mode-release
- install

## Flaky

| test | file | project | attempts |
|---|---|---|---|
| a drain preview classifies every live pod without touching the node | specs/actions.spec.ts:240 | chromium | 2 |

## Jobs

| job | result | minutes |
|---|---|---|
| cluster-mode-release | skipped | 0 |
| e2e / checks-issues-worklist / chromium | success | 8.7 |
| e2e / checks-issues-worklist / firefox | success | 9.3 |
| e2e / checks-issues-worklist / webkit | success | 9.4 |
| e2e / cluster mode / chromium | success | 7.2 |
| e2e / cluster mode / firefox | success | 7 |
| e2e / cluster mode / webkit | success | 7 |
| e2e / cluster-mode-auth | success | 10.4 |
| e2e / distribution-desktop-install | success | 0.1 |
| e2e / e2e-coverage | success | 0.3 |
| e2e / foundation-security / chromium | success | 4.9 |
| e2e / foundation-security / firefox | success | 4.8 |
| e2e / foundation-security / webkit | success | 5.4 |
| e2e / gitops / chromium | success | 11.7 |
| e2e / gitops / firefox | success | 12.1 |
| e2e / gitops / webkit | success | 11.9 |
| e2e / helm / chromium | success | 5.8 |
| e2e / helm / firefox | success | 5.5 |
| e2e / helm / webkit | success | 6.2 |
| e2e / inspect-compare-rbac-topology / chromium | success | 9.4 |
| e2e / inspect-compare-rbac-topology / firefox | success | 11.6 |
| e2e / inspect-compare-rbac-topology / webkit | success | 11.2 |
| e2e / mcp-cli | success | 3.5 |
| e2e / multicluster-fleet / chromium | success | 10.5 |
| e2e / multicluster-fleet / firefox | success | 10.4 |
| e2e / multicluster-fleet / webkit | success | 11.1 |
| e2e / mutations-protection-history / chromium | success | 4.9 |
| e2e / mutations-protection-history / firefox | success | 5.9 |
| e2e / mutations-protection-history / webkit | success | 6.5 |
| e2e / navigation-interaction / chromium | success | 12.2 |
| e2e / navigation-interaction / firefox | success | 12.7 |
| e2e / navigation-interaction / webkit | success | 12 |
| e2e / observability-traffic / chromium | success | 5.4 |
| e2e / observability-traffic / firefox | success | 4.6 |
| e2e / observability-traffic / webkit | success | 4.8 |
| e2e / outage / chromium | success | 4.7 |
| e2e / outage / firefox | success | 4.7 |
| e2e / outage / webkit | success | 5.3 |
| e2e / resilience-capacity-soak / chromium | success | 9.9 |
| e2e / resilience-capacity-soak / firefox | success | 9.4 |
| e2e / resilience-capacity-soak / webkit | success | 10.2 |
| e2e / resources-live-tables / chromium | success | 10.1 |
| e2e / resources-live-tables / firefox | success | 10.5 |
| e2e / resources-live-tables / webkit | success | 11 |
| e2e / select | success | 0.2 |
| e2e / streams-terminals-forwards / chromium | success | 5.8 |
| e2e / streams-terminals-forwards / firefox | success | 6 |
| e2e / streams-terminals-forwards / webkit | success | 7.2 |
| e2e / suite-contract | success | 0.3 |
| e2e / visual-accessibility / chromium | success | 15.1 |
| e2e / visual-accessibility / firefox | success | 15.4 |
| e2e / visual-accessibility / webkit | success | 16.3 |
| fuzz / fuzz (., FuzzServingCheckPublicURL) | success | 12 |
| fuzz / fuzz (./internal/access, FuzzDecisionAggregation) | success | 11.5 |
| fuzz / fuzz (./internal/auth, FuzzRoleAuthorization) | success | 10.5 |
| fuzz / fuzz (./internal/charts, FuzzChartIndex) | success | 10.5 |
| fuzz / fuzz (./internal/charts, FuzzFetchableRepositoryURL) | success | 10.6 |
| fuzz / fuzz (./internal/checks, FuzzParseRules) | success | 11.6 |
| fuzz / fuzz (./internal/issues, FuzzCursor) | success | 10.6 |
| fuzz / fuzz (./internal/mcp, FuzzProtocol) | success | 11.6 |
| fuzz / fuzz (./internal/mcp, FuzzStdioFraming) | success | 11.2 |
| fuzz / fuzz (./internal/store, FuzzHistoryLimit) | success | 10.8 |
| fuzz / fuzz (./internal/store, FuzzTimelineCellsRoundTrip) | success | 10.7 |
| install | skipped | 0 |
| mutation / mutation (checks-a-e) | success | 12.2 |
| mutation / mutation (checks-f-j) | success | 16.5 |
| mutation / mutation (checks-k-o) | success | 9.5 |
| mutation / mutation (checks-p-r) | success | 10.9 |
| mutation / mutation (checks-s-t) | success | 10.3 |
| mutation / mutation (checks-u-z) | success | 5.1 |
| mutation / mutation (cmd) | success | 2.5 |
| mutation / mutation (internal-a-d) | success | 17.2 |
| mutation / mutation (internal-e-l) | success | 25.7 |
| mutation / mutation (internal-m-r) | success | 17.1 |
| mutation / mutation (internal-s-z) | success | 7.7 |
| mutation / mutation (resources-a-f) | success | 6.7 |
| mutation / mutation (resources-g-l) | success | 2.2 |
| mutation / mutation (resources-m-r) | success | 11.8 |
| mutation / mutation (resources-s-z) | success | 5.5 |
| mutation / mutation (root-default) | success | 7 |
| mutation / mutation (root-desktop) | success | 4.9 |
| mutation / mutation (server-a-c) | success | 19.5 |
| mutation / mutation (server-d-e) | success | 8.2 |
| mutation / mutation (server-f) | success | 22.2 |
| mutation / mutation (server-g-l) | success | 28.2 |
| mutation / mutation (server-m-r) | success | 12.4 |
| mutation / mutation (server-s-z) | success | 33.2 |
| mutation / mutation-total | success | 0.2 |
| repeat | success | 5.4 |
