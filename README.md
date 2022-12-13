
# Download
| 2262-90μs-1000 | 2262-90μs-0100 |  2262-90μs-0010 |
| - | - | -|
| [Download](https://anningtrashbin-my.sharepoint.com/:f:/g/personal/zxkmm_anningtrashbin_onmicrosoft_com/EpZx3Kbb7QJBiEAyth9Fe6oBQq9ppsKStYs3PbijOQUyCw?e=P7cl5d) | [Download](https://anningtrashbin-my.sharepoint.com/:f:/g/personal/zxkmm_anningtrashbin_onmicrosoft_com/ErANoKAuGq9CianuBvCnj1kBb3JvxDSfZXEH2lDvjx0cHg?e=WUL6eh) | [Download](https://github.com/zxkmm/2262Scan/releases/tag/raw)|

# How to use
### 1. Pick one of these freqs
| **Frequenc(MHz)** | **Country/Region** | **Probability Rank** |
|-------------------|--------------------|----------------------|
| **433.92**        | CN/EURO            | 1                    |
| **315**           | CN/US              | 1                    |
| **418**           | CN                 | 2                    |
| **303**           | CN                 | 3                    |
| **310**           | CN                 | 4 |
| **330**           | CN                 | 5 |
| **350**           | CN                 | 6 |
| **370**           | CN                 | 7 |
| **390**           | CN                 | 8 |
| **430.5**         | CN/KR                 | 9 |

### 2. Replay these raw files one by one on your portapack.
# 2262Scan
### There r NO SOURCE CODE since these r just raw files.
### Replay file for portapack, uses for scan 2262 gates/barriers.
# The [Mayhem firmware](https://github.com/eried/portapack-mayhem) support ook scan too(ook scan features by [@anzejarni](https://github.com/anzejarni) and [@cusspvz](https://github.com/cusspvz). Use it first. 

# Explain
PT2262/SC2262/LX2262/HS2262/HX2262 encoder contains 13 bits for each signal. 

| A           | D        | S        |
| ----------- | -------- | -------- |
| Address bit | Data bit | Sync bit |

| 0   | 1   | 2   | 3   | 4   | 5   | 6   | 7   | 8   | 9   | 10  | 11  | 12 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | - |
| A | A | A | A | A | A | A/D | A/D | A/D | A/D | A/D | A/D |S|

But most Chinese 2262 based gate/door/etc were seted to
| 0 | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 | 10 | 11 | 12 |
| - | - | - | - | - | - | - | - | - | - | -- | -- | -- |
| A | A | A | A | A | A | A | A | D | D | D  | D  |S|

And the "open" data for most chinese gate/door/etc are
| 8 | 9 | 10 | 11 |
| - | - | -- | -- |
| 1 | 0 | 0  | 0  |
|0|1|0|0|

For common chinese 2262 based gate/door/etc, the clock is about `90` μs   



Feel free to post a issue if you need other clock/databit files.
