# ISA | General
== V0.0.1 ==

- **Design Choices**
	- RISC‑style,
	- Fixed Width,
	- CISC, variable‑length.

We layer optional CISC-ish extentions, but mainly focus on Risc style. Risc style gives us the determinism we need, while still letting us layer optional CISC-ish extentions. We have decided to use 64-bit registers (GPX0‑31), because most modern scientific codes need 64-bit integers/float; We
can still run 32-bit code by sign-extending. We use 64‑bit GP registers, but keep a compact 32‑register file to limit silicon area and power.