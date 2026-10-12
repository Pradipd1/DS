# Self-Healing Deep Learning System for Continual Learning in Dynamic Environments


What this demo shows (in order):
1. A base model trained on initial data.
2. Live data streamed in batches -- after batch 8, we simulate
   the environment changing (concept drift).
3. The system MONITORS its own accuracy every batch.
4. When accuracy falls below a threshold, drift is DETECTED.
5. A DIAGNOSIS step (representing the LLM's role) explains why
   accuracy dropped and recommends a repair action.
6. SELF-REPAIR: the model retrains using a memory buffer (old +
   new data) to fix itself WITHOUT forgetting old patterns.
7. A plot shows accuracy recovering right after each repair.
