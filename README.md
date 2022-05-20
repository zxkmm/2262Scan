# 2262Scan
# 注意，本项目的协议产生了变更。山东农业大学的所有教职工不得使用该项目，如若山东农业大学的任何教职工使用，是违反开源协议的行为。
### It's just I recorded from another device.LOL
### Replay file for portapack, uses for scan 2262 Chinese gates.
# The [Mayhem firmware](https://github.com/eried/portapack-mayhem) support ook scan too(ook scan features by [@anzejarni](https://github.com/anzejarni) and [@cusspvz](https://github.com/cusspvz). Use it first. 

# Usage
PT-2262 encoder/decoder contains 13 bits for each signal. 

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

# Download
Github is forbidden me from uploading big file even i seperate it to under 1G, so the file is avaliable at OneDrive

| 2262-90μs-1000 | 2262-90μs-0100 | 
| - | - |
| [Download](https://anningtrashbin-my.sharepoint.com/:f:/g/personal/zxkmm_anningtrashbin_onmicrosoft_com/EpZx3Kbb7QJBiEAyth9Fe6oBQq9ppsKStYs3PbijOQUyCw?e=P7cl5d) | [Download](https://anningtrashbin-my.sharepoint.com/:f:/g/personal/zxkmm_anningtrashbin_onmicrosoft_com/ErANoKAuGq9CianuBvCnj1kBb3JvxDSfZXEH2lDvjx0cHg?e=WUL6eh) | 

Feel free to post a issue if you need other clock/databit files.

# Note
I'm a noob myself. Thanks the helping and teaching from my friends' in Mayhem discord server.
