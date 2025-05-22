64-QAM Digital Modulator RTL Design
Verilog · RTL Design · SPI · FIR Filter · CDC Handling · Synthesizable IP 
•	Developed a synthesizable RTL design for a 64-QAM modulator to process a 60 Mbps baseband stream into 10-bit I/Q data at 130 MHz, implementing a full DSP chain including symbol mapping, upsampling, and FIR filtering.
•	Designed a fully custom SPI slave interface with a 34-bit control protocol, enabling dynamic runtime configuration of upsampling factors (×4–×13) and programmable filter coefficients.
•	Implemented robust clock domain crossing (CDC) logic using FIFO-based synchronizers and multicycle paths to interface three asynchronous domains: SPI (100 kHz), baseband data (60 MHz), and DSP core (130 MHz).
•	Verified proper reset sequencing across multiple clock domains and integrated RTL assertions to ensure safe enable/disable transitions.
•	Designed register-mapped control architecture and validated functional coverage for SPI write/read back, modulation pipeline timing, and packet boundary detection using simulation waveforms.
