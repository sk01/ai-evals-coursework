# AI Evaluation Strategy Canvas

> Repo file `ai-evals/01-evaluation-strategy/strategy-canvas.md` (the repo is your submission).
> Becomes the **Strategy Canvas** slide of the final pitch deck you assemble in Module 6.
>
> Fill this with the **AI Evaluation Strategy Canvas** tool, then **Copy markdown** and paste it over this file. The headings below mirror the tool's output exactly.

## 1. Product Strategy, The Context

- **Target user:** Busy executives.
- **Key use case:** Summarize business updates into key results, risks, and actions.
- **Value proposition:** Make the business more productive and filter out the noise, helping executives make faster, informed decisions.

## 2. Measurements, The Execution

- **User promise.** For busy executives, Ascend IQ promises to summarize business updates into key results, risks, and actions so that they can make faster, informed decisions. This makes the business more productive and filters out the noise.
- **Top 3 trust metrics:**
  - **Hallucination rate**, the percentage of summary claims unsupported by or contradicting the source. Measure unsupported or contradictory claims divided by all summary claims; lower is better. This protects executives from making decisions based on invented information.
  - **Latency**, the 95th-percentile elapsed time from submitting a business update to receiving the complete summary, measured in seconds across test requests. Lower is better. Fast summaries reduce waiting and support executive productivity.
  - **Robustness**, the percentage of test variants with added irrelevant content, reordered sections, or formatting changes where the summary remains faithful and preserves the essential results, risks, and actions identified in a human-labeled checklist. Higher is better. This keeps noise filtering dependable when business updates are messy.
- **Why these three:** Executives need summaries that avoid invented claims, arrive quickly enough to support their work, and remain dependable when business updates are messy. Together, these metrics protect informed decision-making while helping the business stay productive and filter out the noise.

## 3. Strategic Trade-Offs, The Cost

### Trade-off 1 · Lower hallucination rate ↔ Lower latency

We prioritize reducing unsupported claims over minimizing latency, accepting a slightly slower summary when extra verification improves factual reliability. A fast summary loses its value if invented information leads to a poor decision.

### Trade-off 2 · Robustness ↔ Lower latency

We prioritize dependable summaries of messy inputs over minimizing latency, accepting additional processing time to preserve essential results, risks, and actions. Executives should not have to spend time cleaning up business updates before Ascend IQ can summarize them reliably.

---
_Generated from the AI Evaluation Strategy Canvas, M1 lab tool, AI Evals Certification._
