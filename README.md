# Thai MTEB Leaderboard

ผลทดสอบ Benchmark โมเดล Text Embedding สำหรับภาษาไทย

**[View the Leaderboard](https://anusoft.github.io/thai-mteb-leaderboard/)**

## Overview

This leaderboard presents benchmark results for **21 text embedding models** evaluated on Thai-language tasks from the [MTEB framework](https://github.com/embeddings-benchmark/mteb) (v2.10.0).

- **Full benchmark** (up to 28 tasks): 14 models with detailed per-task scores
- **Screening** (3 fast tasks): 19 models confirmed Thai-capable out of 39 tested

Results are submitted to the official [MTEB Results Repository](https://github.com/embeddings-benchmark/results/pull/428) (merged). Thai benchmark definition [MTEB(tha, v1)](https://github.com/embeddings-benchmark/mteb/pull/4213) is under review.

All evaluations were run on the [LANTA Supercomputer](https://thaisc.io/) with computing resources provided for free by [ThaiSC](https://thaisc.io/)/[NSTDA](https://www.nstda.or.th/), using NVIDIA A100-SXM4-40GB GPUs.

### Top Models (Thai)

| Rank | Model | Score | Tasks | Type |
|------|-------|-------|-------|------|
| 1 | Qwen/Qwen3-Embedding-4B | 74.41 | 24/28 | Full |
| 2 | tencent/KaLM-Embedding-Gemma3-12B | 73.92 | 28/28 | Full |
| 3 | ICT-TIME-and-Querit/BOOM_4B_v1 | 71.84 | 19/28 | Full |
| 4 | jinaai/jina-embeddings-v5-text-small | 69.90 | 27/28 | Full |
| 5 | Linq-AI-Research/Linq-Embed-Mistral | 69.43 | 3/28 | Screening |
| 6 | Qwen/Qwen3-Embedding-0.6B | 69.08 | 27/28 | Full |
| 7 | voyageai/voyage-4-nano | 68.03 | 3/28 | Screening |
| 8 | telepix/PIXIE-Rune-v1.0 | 67.55 | 3/28 | Screening |
| 9 | google/embeddinggemma-300m | 67.53 | 28/28 | Full |
| 10 | Octen/Octen-Embedding-8B | 67.02 | 3/28 | Screening |

### Screening Methodology

39 models were tested on 3 fast Thai tasks (~2-5 min each on A100):
- **WisesightSentimentClassification.v2** — native Thai social media sentiment
- **SIB200Classification** — topic classification
- **XQuADRetrieval** — Thai reading comprehension retrieval

Models scoring >50 avg = Thai-capable. Models <20 = no Thai training data.

### Environment

- **Compute:** LANTA Supercomputer (Cray EX), NVIDIA A100-SXM4-40GB GPUs
- **Framework:** MTEB 2.10.0, sentence-transformers, PyTorch 2.10.0+cu128
- **Evaluation:** `languages=["tha"]` filter, `trust_remote_code=True`

## Acknowledgment

This benchmark was made possible by the free computing resources provided by the [Thailand Supercomputer Center (ThaiSC)](https://thaisc.io/) under the [National Science and Technology Development Agency (NSTDA)](https://www.nstda.or.th/) through the LANTA Supercomputer.

## License

MIT
