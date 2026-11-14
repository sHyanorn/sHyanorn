# Aaron Yang

Algorithm engineering and server-side systems, with backend development next to them. Commerce student at the University of Melbourne. Each project below ships its tests in its repository, with its decision log or its pre-registration, and every number on [my site](https://shyanorn.github.io/) traces back to a project repository.

### Algorithms

- **[push-lab](https://github.com/sHyanorn/push-lab)** · [page](https://shyanorn.github.io/projects/push-lab/)
  An offline lab for push notification recommendation: recall and ranking checked on public data, send volume and timing tested only in a simulator, with every result labelled by how far it can be trusted without live traffic.
- **[ope-checks](https://github.com/sHyanorn/ope-checks)** · [page](https://shyanorn.github.io/projects/ope-checks/)
  Pre-registered checks of published off-policy evaluation results. On the two confirmatory campaigns of the Open Bandit benchmark, the IPS estimate pooled over both is 0.974 of the on-policy click rate (0.915 to 1.036 over ten-minute blocks): no shortfall shown.
- **[retrieval-lab](https://github.com/sHyanorn/retrieval-lab)** · [page](https://shyanorn.github.io/projects/retrieval-lab/)
  BM25 and dense retrieval in Go, where each component is accepted against a number that Pyserini publishes for BEIR. BM25 equals the published nDCG@10 and Recall@100 to four decimals on six datasets; BGE-base with exact search is within 0.0006 in nDCG@10 on all six, and within 0.0004 on all but TREC-COVID.
- **[seqrec-lab](https://github.com/sHyanorn/seqrec-lab)** · [page](https://shyanorn.github.io/projects/seqrec-lab/)
  A pre-registered study of Transformer sequential recommenders, SASRec, BERT4Rec and gSASRec, with equal tuning budgets, five to ten seeds per arm and full-ranking evaluation on one rented consumer GPU. On MovieLens-1M and Video_Games, SASRec with full cross-entropy is ahead of BERT4Rec and gSASRec, and SASRec with BCE and one negative trails it by more than 2%. MovieLens-1M's test targets had been read for anchor checks before its final runs. Steam and MovieLens-20M have no results yet.

### Server-side systems

- **[recserve](https://github.com/sHyanorn/recserve)** · [page](https://shyanorn.github.io/projects/recserve/)
  A recommendation serving system in Go: retrieval, features, ranking and rerank behind one HTTP API, with the item vectors on gRPC shard replicas. In kind at 100 requests/s, through rolling restarts of the gateways and of the replicas and a bundle swap, no response failed or was degraded, with stage budgets of 100 ms.

### Backend systems

- **[matching-engine](https://github.com/sHyanorn/matching-engine)** · [page](https://shyanorn.github.io/projects/matching-engine/)
  Go limit order book with a write-ahead command log and open-loop load testing: 5.05M–6.95M commands/s in the core, p99 1.76 ms at 10k requests/s and 41.1 ms at 50k, near saturation.

### Earlier

[vault-share](https://github.com/sHyanorn/vault-share) (end-to-end encrypted file sharing) · [backtest-lab](https://github.com/sHyanorn/backtest-lab) (overfitting checks for backtests) · [local-ledger](https://github.com/sHyanorn/local-ledger) (an encrypted personal finance desktop app)
