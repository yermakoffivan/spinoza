# Nightly 2026-11-07 — regression

Commit `6a3f44c7f5ff`, triggered by schedule. [Run](https://github.com/yermakoffivan/spinoza/actions/runs/42358580171)

| | this run | |
|---|---|---|
| jobs | 89 | 2 failed |
| job-minutes | 780.1 (+55.8) | |
| e2e coverage | 64.5% (+17.5) | |
| mutation score | 100% (no change) | 7824 killed, 0 lived |
| flaky | 1 (+1) | passed only on retry |
| uncovered mutants | 341 (no change) | records across reported build variants |

Mutation score is killed / (killed + lived). Uncovered mutants are excluded from that score; some are uninstrumented constant expressions.

## Separate system coverage

These suites retain their own Go statement denominators. The browser E2E coverage above is unchanged by these profiles.

| suite | covered / total statements | coverage |
|---|---|---|
| cluster-mode-auth | 4926 / 21386 | 23% |
| cluster-mode-chromium | 3864 / 21386 | 18.1% |
| cluster-mode-firefox | 3865 / 21386 | 18.1% |
| cluster-mode-webkit | 3864 / 21386 | 18.1% |
| mcp-cli | 794 / 21580 | 3.7% |

## New failures

- cluster-mode-release
- install

## Fixed since the last run

- e2e / checks-issues-worklist / webkit
- e2e / foundation-security / webkit
- e2e / gitops / chromium
- e2e / gitops / firefox
- e2e / gitops / webkit
- e2e / helm / webkit
- e2e / inspect-compare-rbac-topology / chromium
- e2e / inspect-compare-rbac-topology / firefox
- e2e / inspect-compare-rbac-topology / webkit
- e2e / multicluster-fleet / chromium
- e2e / multicluster-fleet / firefox
- e2e / multicluster-fleet / webkit
- e2e / mutations-protection-history / webkit
- e2e / navigation-interaction / chromium
- e2e / navigation-interaction / firefox
- e2e / navigation-interaction / webkit
- e2e / observability-traffic / webkit
- e2e / outage / webkit
- e2e / resilience-capacity-soak / chromium
- e2e / resilience-capacity-soak / firefox
- e2e / resilience-capacity-soak / webkit
- e2e / resources-live-tables / chromium
- e2e / resources-live-tables / firefox
- e2e / resources-live-tables / webkit
- e2e / streams-terminals-forwards / chromium
- e2e / streams-terminals-forwards / firefox
- e2e / streams-terminals-forwards / webkit
- e2e / visual-accessibility / chromium
- e2e / visual-accessibility / firefox
- e2e / visual-accessibility / webkit

## Failing

- cluster-mode-release
- install

## Flaky

| test | file | project | attempts |
|---|---|---|---|
| an empty log filter reports both the empty result and its scope | specs/terminals.spec.ts:197 | chromium | 2 |

## Jobs

| job | result | minutes |
|---|---|---|
| cluster-mode-release | skipped | 0 |
| e2e / checks-issues-worklist / chromium | success | 8.1 |
| e2e / checks-issues-worklist / firefox | success | 8.3 |
| e2e / checks-issues-worklist / webkit | success | 8.3 |
| e2e / cluster mode / chromium | success | 7.4 |
| e2e / cluster mode / firefox | success | 7.1 |
| e2e / cluster mode / webkit | success | 6.1 |
| e2e / cluster-mode-auth | success | 10.7 |
| e2e / distribution-desktop-install | success | 0.1 |
| e2e / e2e-coverage | success | 0.3 |
| e2e / foundation-security / chromium | success | 4.2 |
| e2e / foundation-security / firefox | success | 4.1 |
| e2e / foundation-security / webkit | success | 3.7 |
| e2e / gitops / chromium | success | 11.6 |
| e2e / gitops / firefox | success | 10.6 |
| e2e / gitops / webkit | success | 11.9 |
| e2e / helm / chromium | success | 5 |
| e2e / helm / firefox | success | 4.9 |
| e2e / helm / webkit | success | 5.5 |
| e2e / inspect-compare-rbac-topology / chromium | success | 10.2 |
| e2e / inspect-compare-rbac-topology / firefox | success | 9.5 |
| e2e / inspect-compare-rbac-topology / webkit | success | 9.3 |
| e2e / mcp-cli | success | 3.2 |
| e2e / multicluster-fleet / chromium | success | 8.8 |
| e2e / multicluster-fleet / firefox | success | 9.8 |
| e2e / multicluster-fleet / webkit | success | 10 |
| e2e / mutations-protection-history / chromium | success | 5.5 |
| e2e / mutations-protection-history / firefox | success | 5.8 |
| e2e / mutations-protection-history / webkit | success | 5.8 |
| e2e / navigation-interaction / chromium | success | 10.4 |
| e2e / navigation-interaction / firefox | success | 11.3 |
| e2e / navigation-interaction / webkit | success | 11.9 |
| e2e / observability-traffic / chromium | success | 4.1 |
| e2e / observability-traffic / firefox | success | 4.2 |
| e2e / observability-traffic / webkit | success | 4.5 |
| e2e / outage / chromium | success | 4.1 |
| e2e / outage / firefox | success | 4.2 |
| e2e / outage / webkit | success | 4.8 |
| e2e / resilience-capacity-soak / chromium | success | 9.1 |
| e2e / resilience-capacity-soak / firefox | success | 9.8 |
| e2e / resilience-capacity-soak / webkit | success | 9.3 |
| e2e / resources-live-tables / chromium | success | 10.4 |
| e2e / resources-live-tables / firefox | success | 9.8 |
| e2e / resources-live-tables / webkit | success | 9.1 |
| e2e / select | success | 0.1 |
| e2e / streams-terminals-forwards / chromium | success | 4.9 |
| e2e / streams-terminals-forwards / firefox | success | 6.1 |
| e2e / streams-terminals-forwards / webkit | success | 6.3 |
| e2e / suite-contract | success | 0.4 |
| e2e / visual-accessibility / chromium | success | 14.4 |
| e2e / visual-accessibility / firefox | success | 13.5 |
| e2e / visual-accessibility / webkit | success | 15.4 |
| fuzz / fuzz (., FuzzServingCheckPublicURL) | success | 12.4 |
| fuzz / fuzz (./internal/access, FuzzDecisionAggregation) | success | 11.5 |
| fuzz / fuzz (./internal/auth, FuzzRoleAuthorization) | success | 10.3 |
| fuzz / fuzz (./internal/charts, FuzzChartIndex) | success | 10.2 |
| fuzz / fuzz (./internal/charts, FuzzFetchableRepositoryURL) | success | 10.2 |
| fuzz / fuzz (./internal/checks, FuzzParseRules) | success | 11.4 |
| fuzz / fuzz (./internal/issues, FuzzCursor) | success | 10.3 |
| fuzz / fuzz (./internal/mcp, FuzzProtocol) | success | 11 |
| fuzz / fuzz (./internal/mcp, FuzzStdioFraming) | success | 11.1 |
| fuzz / fuzz (./internal/store, FuzzHistoryLimit) | success | 10.7 |
| fuzz / fuzz (./internal/store, FuzzTimelineCellsRoundTrip) | success | 10.8 |
| install | skipped | 0 |
| mutation / mutation (checks-a-e) | success | 12.4 |
| mutation / mutation (checks-f-j) | success | 15.5 |
| mutation / mutation (checks-k-o) | success | 10 |
| mutation / mutation (checks-p-r) | success | 11.6 |
| mutation / mutation (checks-s-t) | success | 10 |
| mutation / mutation (checks-u-z) | success | 4.6 |
| mutation / mutation (cmd) | success | 1 |
| mutation / mutation (internal-a-d) | success | 15 |
| mutation / mutation (internal-e-l) | success | 27.5 |
| mutation / mutation (internal-m-r) | success | 17.8 |
| mutation / mutation (internal-s-z) | success | 9.4 |
| mutation / mutation (resources-a-f) | success | 4.7 |
| mutation / mutation (resources-g-l) | success | 0.9 |
| mutation / mutation (resources-m-r) | success | 10.8 |
| mutation / mutation (resources-s-z) | success | 4.6 |
| mutation / mutation (root-default) | success | 4.3 |
| mutation / mutation (root-desktop) | success | 5.2 |
| mutation / mutation (server-a-c) | success | 25.9 |
| mutation / mutation (server-d-e) | success | 7.4 |
| mutation / mutation (server-f) | success | 15.7 |
| mutation / mutation (server-g-l) | success | 24.9 |
| mutation / mutation (server-m-r) | success | 11.9 |
| mutation / mutation (server-s-z) | success | 28.2 |
| mutation / mutation-total | success | 0.2 |
| repeat | success | 6.8 |
