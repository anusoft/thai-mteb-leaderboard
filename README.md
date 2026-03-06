# Thai MTEB Leaderboard

ผลทดสอบ Benchmark โมเดล Text Embedding สำหรับภาษาไทย

**[View the Leaderboard](https://anusoft.github.io/thai-mteb-leaderboard/)**

## Overview

This report presents benchmark results for **14 multilingual text embedding models** evaluated on 28 Thai-language tasks from the [MTEB framework](https://github.com/embeddings-benchmark/mteb) (v2.10.0).

Results are submitted to the official [MTEB Results Repository](https://github.com/embeddings-benchmark/results/pull/428).

All evaluations were run on the [LANTA Supercomputer](https://thaisc.io/) with computing resources provided for free by [ThaiSC](https://thaisc.io/)/[NSTDA](https://www.nstda.or.th/), using NVIDIA A100-SXM4-40GB GPUs.

### Top Models (Thai)

| Rank | Model | Avg Score | Tasks |
|------|-------|-----------|-------|
| 1 | Qwen/Qwen3-Embedding-4B | 74.41 | 24/28 |
| 2 | tencent/KaLM-Embedding-Gemma3-12B | 73.92 | 28/28 |
| 3 | ICT-TIME-and-Querit/BOOM_4B_v1 | 71.84 | 19/28 |
| 4 | jinaai/jina-embeddings-v5-text-small | 69.90 | 27/28 |
| 5 | Qwen/Qwen3-Embedding-0.6B | 69.08 | 27/28 |

### Task Coverage

| Type | Count | Tasks |
|------|-------|-------|
| BitextMining | 6 | BibleNLPBitextMining, FloresBitextMining, NTREXBitextMining, Tatoeba, WebFAQBitextMiningQAs, WebFAQBitextMiningQuestions |
| Classification | 9 | LanguageClassification, MTOPDomainClassification, MTOPIntentClassification, MassiveIntentClassification, MassiveScenarioClassification, MultilingualSentimentClassification, SIB200Classification, WisesightSentimentClassification.v2, WongnaiReviewsClassification |
| Clustering | 1 | SIB200ClusteringS2S |
| PairClassification | 1 | XNLI |
| Reranking | 2 | MIRACLReranking, MultiLongDocReranking |
| Retrieval | 9 | BelebeleRetrieval, MIRACLRetrieval, MIRACLRetrievalHardNegatives, MIRACLRetrievalHardNegatives.v2, MKQARetrieval, MrTidyRetrieval, MultiLongDocRetrieval, WebFAQRetrieval, XQuADRetrieval |

### Environment

- **Compute:** LANTA Supercomputer (Cray EX), NVIDIA A100-SXM4-40GB GPUs
- **Framework:** MTEB 2.10.0, sentence-transformers, PyTorch 2.10.0+cu128
- **Evaluation:** `languages=["tha"]` filter, `trust_remote_code=True`

## Acknowledgment

This benchmark was made possible by the free computing resources provided by the [Thailand Supercomputer Center (ThaiSC)](https://thaisc.io/) under the [National Science and Technology Development Agency (NSTDA)](https://www.nstda.or.th/) through the LANTA Supercomputer.

## License

MIT
