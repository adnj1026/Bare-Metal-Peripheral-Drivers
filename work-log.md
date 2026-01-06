
[2025-12-29]
- No debugging performed over last 3 days
- Resuming investigation from Hypothesis: DEMCR TRCENA bit

[2025-12-30]
- No embedded or testing work done today
- No progress made due to lack of structured task and supervision
- Plan: resume with 20-minute focused session tomorrow morning

[2025-12-30]
- watched lectures on clock and GPIO
- did not work on hardware
- Plan: work on hardware.

[2026-01-02]
- Implemented bare-metal clock configuration to route HSI to MCO1 (PA8).
- Verified HSI output on oscilloscope via MCO1 pin (worked on first run).
- Plan: Design and implement gpio.c driver (target: 3 days).

[2026-01-06]
- Began designing GPIO initialization flow for bare-metal driver
- Explored init abstractions and conditional handling for pin configuration
- Implemented initial LED blink abstraction
- Encountered build/runtime errors during integration
- Next: resolve GPIO init errors and stabilize LED blink

[2026-01-7]
- managed to debug and flash the bare metal code for blinking led
- hardware led did not blink 
- plan:  inspect GPIO init logic and abstraction assumptions