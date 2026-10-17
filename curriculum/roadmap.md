# Frontier AI Engineering Career Roadmap

This roadmap connects fundamentals to public work and role families at Google DeepMind, Anthropic, and OpenAI. It is a learning plan, not a promise of employment. Company practices and role requirements change, so use current official publications and job descriptions when choosing what to study next.

## Phase 0 — Orient to the frontier-AI stack

**Understand:** model, application, agent, orchestrator, evaluation harness, inference system, and research experiment.

**Deliverable:** one architecture diagram that distinguishes model capability from product reliability.

**Company lens**
- DeepMind: research-to-engineering, learning systems, planning, multimodal and world-model research.
- Anthropic: effective agent design, evaluations, model behavior, reliability and interpretability.
- OpenAI: foundation models, product systems, post-training, reasoning and inference.

## Phase 1 — Python and PyTorch foundations

**Topics:** Python fluency, NumPy, tensor shapes, broadcasting, autograd, gradient descent, optimizers, datasets, batching, train/eval modes, reproducibility.

**Build:** linear regression, an MLP classifier, a training loop, and tests for tensor shapes and gradients.

**Interview questions:** Why does a gradient become zero? What does `model.eval()` change? Why can training loss fall while validation performance worsens?

**Exit evidence:** a small repository with tests, plots, a README, and an explanation of each tensor dimension.

## Phase 2 — Deep learning and transformer internals

**Topics:** initialization, normalization, regularization, embeddings, attention, positional information, causal masks, residual paths, tokenization, loss functions.

**Build:** attention from basic tensor operations, a transformer block, and a tiny language model.

**Research practice:** compare a baseline with one change; state the hypothesis before running the experiment.

**Exit evidence:** reproducible results, learning curves, error analysis, and a short technical note.

## Phase 3 — Training and inference systems

**Topics:** profiling, memory use, batching, mixed precision, caching, throughput/latency trade-offs, distributed-training concepts, serving.

**Build:** benchmark a model under different batch sizes and sequence lengths; report quality, memory, throughput and latency.

**Company lens:** understand the general systems problems that arise when training or serving large models without claiming knowledge of proprietary infrastructure.

## Phase 4 — Post-training, reasoning and reinforcement learning

**Topics:** supervised fine-tuning, preference data, reward models, policy optimization concepts, exploration, reward hacking, inference-time compute and evaluation.

**Build:** a small controlled optimization experiment or a preference-ranking baseline, with clear limitations.

**Research questions:** What is being optimized? What can the metric miss? How would you detect reward hacking or benchmark overfitting?

## Phase 5 — Agents, orchestration and evaluation

**Topics:** tools, state, control flow, retries, memory, workflow vs agent loop, multi-agent coordination, graders, test sets, statistical uncertainty, regressions.

**Build:** compare a fixed workflow and an agentic solution on the same task set. Measure task success, tool errors, latency and cost.

**Company lens:** use Anthropic's public agent/evaluation engineering posts, OpenAI's public agent and evaluation materials, and DeepMind's public research to compare approaches without assuming one architecture is universally best.

## Phase 6 — Interpretability, reliability and safety

**Topics:** probing, feature attribution limits, mechanistic interpretability concepts, adversarial evaluation, robustness, calibration, uncertainty, safety cases.

**Build:** a small behavior-evaluation suite with documented failure categories and reproducible tests.

**Research question:** What evidence would change your mind about the proposed explanation?

## Phase 7 — Research reproduction

Choose a public paper with an experiment that can be reproduced using accessible compute.

1. Write the central claim and assumptions in your own words.
2. Implement a baseline first.
3. Define metrics and a test protocol before experiments.
4. Reproduce a core result or document why it cannot be reproduced.
5. Run at least one ablation and one failure analysis.
6. Publish code, environment details, results, limitations, and a short report.

## Phase 8 — Flagship project

Suggested direction: **uncertainty-aware world models for decision-making**.

Build a controlled environment where a learned predictive state supports a downstream decision. Compare against simple baselines, measure uncertainty and downstream outcomes, and document where the model fails. This can connect your statistics and model-validation experience with research engineering.

## Phase 9 — Interview and application loop

Maintain a tracker for each target role with:
- Exact role title, location, level and official posting
- Required skills and evidence gaps
- One matching project or paper
- Coding, ML fundamentals, systems and research questions
- Resume bullets backed by measurable results
- Outreach contacts and follow-up dates

Do not apply only on the basis of company prestige. Match each application to the specific team's problem and role requirements.

## Weekly cadence

A sustainable default is five focused sessions per week:
- 2 implementation sessions
- 1 paper-reading and note-taking session
- 1 experiment/debugging session
- 1 interview explanation or project write-up

Increase or reduce the workload based on your available time. Depth, reproducibility and feedback matter more than collecting certificates or rushing through topics.
