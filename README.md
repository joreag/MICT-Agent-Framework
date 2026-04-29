# MICT Cognitive Framework for AI Agents

[![License: BOKRLv2](https://img.shields.io/badge/License-BOKRLv2-blue.svg)](LICENSE.md)
[![Status: Experimental](https://img.shields.io/badge/Status-Active_Research-success.svg)]()

**Upgrade your LLM from linear text prediction to Cyclical State Transformation.**

The MICT (Map, Iterate, Check, Transform) framework is a cognitive architecture designed to force Large Language Models (LLMs) and Autonomous Agents into rigorous, "System 2" thinking. By injecting this skill into your agent's system prompt, you eliminate "greedy decoding" and significantly reduce hallucinations on complex tasks.

## The Problem
Standard LLMs operate linearly. They read a prompt and immediately begin generating the highest-probability next token. When faced with complex systems architecture, logical paradoxes, or multi-step reasoning, this "greedy" approach causes them to hallucinate or get trapped in dead-end logic.

## The MICT Solution
Derived from the **Mobius Inspired Cyclical Transformation Theory** (a framework for complex systems and OS architecture), this prompt forces the AI to pause and execute a 4-stage processing loop before finalizing its output:

1. **[M] MAP:** Contextualize the problem, identify hidden constraints, and define the state space.
2. **[I] ITERATE:** Generate multiple hypotheses and internally simulate their outcomes.
3. **[C] CHECK:** Evaluate the hypotheses against the MAP constraints (Zero-Trust gating).
4. **[T] TRANSFORM:** Execute the final, mathematically/logically superior path.

## Usage

Simply copy the contents of `mict_skill.md` and paste it into your Agent's **System Prompt** (or custom instructions). 

### Example Output

When faced with a complex query, the agent will now "show its work" using Glass Box XML tags:

```xml
<MICT_CYCLE>
  <MAP>
    Identified constraints: #![no_std], bare-metal environment, no Mutex/spinlocks permitted. High concurrency required.
  </MAP>
  <ITERATE>
    Path A: Lock-free atomic linked list. (Simulation: ABA problem risk).
    Path B: Per-CPU core allocation arenas. (Simulation: Low contention, high memory overhead).
    Path C: Krapivin Elastic Hashing / Proactive density mapping. (Simulation: O(1) writes, deterministic).
  </ITERATE>
  <CHECK>
    Path A risks memory corruption without standard atomic guards. Path B is standard but bloated. Path C meets all constraints and guarantees zero latency spikes. Path C selected.
  </CHECK>
  <TRANSFORM>
    [Provides the Rust architectural code for Path C...]
  </TRANSFORM>
</MICT_CYCLE>
```

## Advanced: HCTS (Hierarchical Context)
For massive tasks (e.g., "Write an entire application"), the MICT skill instructs the AI to invoke **HCTS** (Hierarchical Contextual Transformation System), breaking the master task into sub-tasks and running miniature MICT cycles on each one.

MICT_VS_STANDARD_EXAMPLE.md

## Origins
The MICT Framework is part of **Project Genesis**, an ongoing research initiative into hybrid AI-native Operating Systems and computational physics. 

