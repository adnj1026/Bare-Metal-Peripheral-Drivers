
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

[2026-01-07]
- Minimal progress; attempted brief debug/run (<10 min)
- No substantive firmware changes

[2026-01-08]
- GPIO driver implemented: init, write.
- LED successfully wrote on hardware
- Changes not yet committed

[2026-01-09]
- GPIO driver implementation: read, otype, speed, alternate, toggle.
- finished GPIO driver (for now).
- blinked LED and viwed HSI signal via rounting through MC1 to pin 8; to test my code.
- plan: learn and create bare metal code usart, interrupts, timers etc.

[2026-01-11]
- No firmware work (weekend)

[2026-01-12]
- No firmware work (headache + office testing tasks)

[2026-01-13]
- in an attempt to test all the gpio api's, I wrote code blink LED faster when the button is pushed.
- the LED did not blink, plan to debug.
- plan to use all the GPIO API. 

[2026-01-14]
- No firm ware work done.

[2026-01-15]
- No firm ware work done.

[2026-01-16]
- No firm ware work done.

[2026-01-17]
- No firm ware work done.

[2026-01-18]
- No firm ware work done.

[2026-01-19]
- No firm ware work done.

[2026-01-20]
- understood the working of interrupts.
- wrote code to evoke interrupts when button is pressed.
- the led did not blink.
- plan to debug it tomorrow.

[2026-01-21]
- tried to debug by stepping over.
- yet to find the exact cause.

[2026-01-22]
- no firmware work done.


[2026-01-23]
- the led is blinking, even when the button is not pressed.


[2026-01-24]
- no firm ware work done.

[2026-01-25]
- no firm ware work done.

[2026-01-26]
- no firm ware work done.

[2026-01-27]
- connected external button
- the led started toggling according to the interupts.

[2026-01-28]
- wrote isr.c and isr.h
- toggled led via the abstraction.

[2026-01-29]
no firm ware work done.

[2026-01-30]
no firmware work done.