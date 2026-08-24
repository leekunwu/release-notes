# Release Notes

A minimal GitHub Pages display that rotates Korean and English phrases from a CSV file.

## Edit phrases

Edit `phrases.csv` in the repository root. The file has **no header**:

- Column 1: Korean phrase
- Column 2: English phrase

```csv
국문 문구,English phrase
다음 국문 문구,Next English phrase
```

If a phrase contains a comma, wrap that cell in double quotes. To include a literal double quote inside a quoted cell, write it twice.

```csv
"음악, 그리고 기억","Music, and memory"
"그는 ""좋다""고 말했다.","He said, ""Good."""
```

## Playback

- Each phrase remains on screen for 8 seconds.
- All rows are shuffled and played once before the next shuffle begins.
- The first phrase in a new shuffle never repeats the immediately preceding phrase.
- Transitions use a 1.6-second cross dissolve with a subtle blur.
- Korean text is slightly larger than English text.

## Publish with GitHub Pages

1. In the repository, open **Settings → Pages**.
2. Under **Build and deployment**, choose **Deploy from a branch**.
3. Select the `main` branch and `/ (root)` folder.
4. Click **Save**.

GitHub Pages will publish the site at:

```text
https://leekunwu.github.io/release-notes/
```

## Typography

The page uses Sandoll Gothic when it is installed on the visitor's device. Otherwise it falls back to Apple SD Gothic Neo, Noto Sans KR, and Arial.
