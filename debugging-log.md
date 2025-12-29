## SWV printf not visible on Port 0 (25-Dec-2025)

[Hypotheses]
- SystemCoreClock value may be incorrect after clock configuration, causing SWV baud mismatch
- ITM stimulus port 0 may not be enabled (ITM->TER)
- Trace may not be enabled at core level (DEMCR TRCENA bit)
- printf redirection in syscalls.c (_write) may not be executed
- Required CMSIS core debug registers may not be explicitly initialized in bare-metal setup
- Unclear interaction between core-level ITM and STM32 clock configuration

[What I Tried]
- Attempted to include system clock initialization files; encountered build errors during compilation
- Modified ITM initialization and SendChar code based on examples; no SWV output observed
- Created a new project to rule out configuration corruption; issue persists

[Current Status]
- Issue unresolved
- Investigating CMSIS core debug and ITM initialization in bare-metal context
- To continue next session


## SWV printf not visible on Port 0 (2025-12-29)

- No debugging performed over last 3 days
- Resuming investigation from Hypothesis: DEMCR TRCENA bit


[What I Tried]
- Kept the previous code, built and debugged once again, made sure to the cursor is active in the data console.
- Left the cursor not blinking and debugged.

[Current Status]
- Printf statement appreared on the data console.
- Despite the cursor not blinking the printf statement worked.

[Observation]
- Without code changes, SWV printf output appeared on the data console on first debug run

[Notes]
- Cursor state (blinking vs not blinking) did not affect output
- Root cause currently unknown


