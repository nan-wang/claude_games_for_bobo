# 汉字大冒险 (Chinese Character Adventure)

A Chinese character learning game for Bobo (age 5). Learn 10 basic pictographic characters through a "see the picture → watch it transform → quiz" flow.

## Characters

The 10 characters are from 部编版一年级上册识字第一单元 (PEP Grade 1 Literacy Unit 1):

| Character | Pinyin | Meaning | Picture |
|-----------|--------|---------|---------|
| 日 | rì | Sun | Orange circle with smiley face |
| 月 | yuè | Moon | Yellow crescent with stars |
| 山 | shān | Mountain | Three green peaks with snow |
| 水 | shuǐ | Water | Blue wavy lines with droplets |
| 火 | huǒ | Fire | Red/orange/yellow flames |
| 口 | kǒu | Mouth | Pink open mouth |
| 目 | mù | Eye | An eye with pupil |
| 耳 | ěr | Ear | A cute ear shape |
| 田 | tián | Field | Green field divided in 4 |
| 人 | rén | Person | Cute stick figure |

## How to Play

### Desktop (index.html)
- Open `index.html` in a browser
- Press any key or click to start
- During learning phases: click or press any key to skip ahead
- During quiz: click a character button or press 1-4

### iPad (ipad.html)
```bash
cd 20260318_hanzi_game
python3 -m http.server 8080
```
Open `http://<mac_ip>:8080/ipad.html` on iPad.
- Tap anywhere to start and to skip learning phases
- Tap character buttons during quiz

## Game Flow

1. **Learn**: See a cute picture of the concept (e.g., a sun)
2. **Morph**: Watch the picture transform into the character with sparkles
3. **Review**: See the large character with pinyin and meaning
4. **Quiz**: Pick the correct character from 4 choices
5. **Victory**: Celebrate learning all 10 characters!

## Design

- All in-game text is in Chinese (no English)
- No failure states — wrong answers just wobble, with "再试一次！" encouragement
- Magical purple night-sky theme with floating sparkles
- Progress tracked with star indicators at the top

![Screenshot](screenshot.png)
