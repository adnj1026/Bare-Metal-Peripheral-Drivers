## GPIO Init – Design Questions

Unclear points encountered:
- Should init logic branch per mode (input/output/AF)?
- How much abstraction is appropriate for a simple driver?
- Whether to expose per-pin config or per-port config

Current direction:
- Start with minimal abstraction for LED blink
- Refine API once basic output works

