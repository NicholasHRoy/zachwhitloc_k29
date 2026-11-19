# Zach Whitlock, K = 29

A birthday gift for Zach: a portrait of him built entirely from the words of his own publications, with an interactive page for exploring where each word comes from.

## What it is

- **The portrait.** A photo of Zach redrawn in words. The photo was split into 29 tonal regions, and each region is filled with words from one of 29 topics found in his writing.
- **The page.** Open `index.html` to explore it:
  - **Articles** lists his 14 publications. Pick one to light up the words it supplies.
  - **Topics** shows the 29 topics, ordered from fossil fuels to clean technology. Pick one to see its region, its words and the articles behind it.
  - **Click any word** in the portrait to see which articles use it and how often.

## How it was made

14 publications, 2023–2026 (75,749 words) → TF-IDF → NMF topic model fitted at 30 topics, with the two China topics merged, so k = 29. First-author papers are weighted 3×, second-author 1.5×. The photo was k-means-clustered into 29 tonal regions, each speaking one topic. Colours were chosen by hand to suit each topic's word, and every word is shaded to the photo's brightness.

## Files

| File | Contents |
|---|---|
| `index.html` | The interactive page |
| `data.js` | Word positions, topics and per-article word counts |
| `zach.jpg` | The K = 29 portrait |

## Viewing it

Download the folder and open `index.html` in a browser. It needs no installation and no internet connection.

Made by Nick, with Claude (Anthropic). Happy birthday, Zach.
