# Java benchmarks

Here are some Java benchmarks I conducted in my free time.

Test system specs:

- AMD Ryzen 7 5800X3D
- AMD Radeon RX 7800 XT (Driver 25.3.1)
- ASRock X570 Pro⁴ (BIOS ver. 5.60)
- G.Skill Aegis 32 GB DDR4 3200 MT/s CL16 RAM
- Crucial P5 Plus 1 TB
- Windows 11 Pro 24H2

# Game loading times

An average of 10 runs of every Java version and garbage collector. This was tested in an [optimized StoneBlock instance](packs-1.12.2.md#stoneblock). Java 8 and 21 were from Adoptium. The time was measured with VintageFix.

![average](<img width="924" height="571" alt="java bench marks" src="https://github.com/user-attachments/assets/c0cdf55d-4401-4c35-8289-3e56ecd5a3d2" />)


GraalVM 24 with G1GC performs best here, followed by GraalVM 24 with Generational ZGC. Java 8 is considerably slower than everything else.

### Data from all 10 runs:

![all 10 runs](<img width="1611" height="998" alt="outro java bench marks" src="https://github.com/user-attachments/assets/4c62536e-20c1-42d8-9322-d14840bc8607" />)

