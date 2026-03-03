# Thai MTEB Leaderboard

ผลทดสอบ Benchmark โมเดล Text Embedding สำหรับภาษาไทย

**[View the Leaderboard](https://anusoft.github.io/thai-mteb-leaderboard/)**

## Overview

This report presents benchmark results for text embedding models evaluated on 28 Thai-language tasks from the [MTEB framework](https://github.com/embeddings-benchmark/mteb) (v2.10.0).

All evaluations were run on the [LANTA Supercomputer](https://thaisc.io/) with computing resources provided for free by [ThaiSC](https://thaisc.io/)/[NSTDA](https://www.nstda.or.th/), using NVIDIA A100-SXM4-40GB GPUs.

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
- **Framework:** MTEB 2.10.0, sentence-transformers 5.2.3, PyTorch 2.10.0+cu128
- **Evaluation:** `languages=["tha"]` filter, `trust_remote_code=True`

## Acknowledgment

This benchmark was made possible by the free computing resources provided by the [Thailand Supercomputer Center (ThaiSC)](https://thaisc.io/) under the [National Science and Technology Development Agency (NSTDA)](https://www.nstda.or.th/) through the LANTA Supercomputer.

## License

MIT
