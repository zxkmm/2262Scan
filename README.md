
# Download
| 2262-90μs-1000 | 2262-90μs-0100 |  2262-90μs-0010 |
| - | - | -|
| [Download](https://anningtrashbin-my.sharepoint.com/:f:/g/personal/zxkmm_anningtrashbin_onmicrosoft_com/EpZx3Kbb7QJBiEAyth9Fe6oBQq9ppsKStYs3PbijOQUyCw?e=P7cl5d) | [Download](https://anningtrashbin-my.sharepoint.com/:f:/g/personal/zxkmm_anningtrashbin_onmicrosoft_com/ErANoKAuGq9CianuBvCnj1kBb3JvxDSfZXEH2lDvjx0cHg?e=WUL6eh) | [Download](https://github.com/zxkmm/2262Scan/releases/tag/raw)|
# 2262Scan
### It's just I recorded from another device. LOL
### There r NO SOURCE CODE since these r just raw files.
### Replay file for portapack, uses for scan 2262 Chinese gates.
# The [Mayhem firmware](https://github.com/eried/portapack-mayhem) support ook scan too(ook scan features by [@anzejarni](https://github.com/anzejarni) and [@cusspvz](https://github.com/cusspvz). Use it first. 

# Usage
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
