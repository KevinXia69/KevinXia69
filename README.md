# Kevin Xia

I contribute to LLM applications, with recent work on conversation context management and multimodal model compatibility.

## Selected open-source contributions

### [HKUDS/DeepTutor](https://github.com/HKUDS/DeepTutor)

#### Conversation compaction budget control · [PR #772](https://github.com/HKUDS/DeepTutor/pull/772)

**Merged into `dev`.**

- Bounded history planning and raw-summary rebuild eligibility at 131,072 tokens, and summary output at 16,384 tokens or the lower active generation limit.
- Kept recent-history allocation independent of the summary output cap, preserving headroom between compactions. Added regression coverage for large context windows and small generation limits.

This keeps compaction budgets from scaling unchecked with a model's context window. The history budget remains a planning target; the newest non-empty message is preserved even when it exceeds that target.

#### Qwen3.8-Max vision compatibility · [PR #770](https://github.com/HKUDS/DeepTutor/pull/770)

Added Qwen3.8-Max vision capability recognition, with regression coverage for multimodal fallback and LlamaIndex image ingestion.

**Integrated into `dev` via a maintainer's local rebase**, with my authorship preserved in [commit `115a78ae`](https://github.com/HKUDS/DeepTutor/commit/115a78ae1ba905098c8a637a65c063763bcd8fb7). GitHub displays the original PR as **Closed**, rather than **Merged**; the [maintainer's confirmation](https://github.com/HKUDS/DeepTutor/pull/770#issuecomment-5204043730) records how the contribution was incorporated.

[View all my DeepTutor pull requests](https://github.com/HKUDS/DeepTutor/pulls?q=is%3Apr+author%3AKevinXia69)
