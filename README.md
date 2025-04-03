# TPT-PE Thematic Analysis

This repository contains the code used in the article titled "Uncovering shifts in the history of Physics education: a systematic, NLP-based, thematic analysis of articles from The Physics Teacher and Physics Education journals (1966 - 2020)" written by Martina Caramaschi and Tor Ole B. Odden.

## Overview

The project aims to uncover shifts in the history of Physics education by applying a systematic NLP-based thematic analysis to articles published in "The Physics Teacher" and "Physics Education" journals from 1966 to 2020.

## First Data Collection and Cleaning

We downloaded the articles of TPT and PE in two different moments:
- TPT in mid 2020
- PE in 2024

The articles were downloaded in PDF format. Several cleaning steps were performed on the articles' texts:
- Removed documents with very short texts (under 400 characters) since most of these articles were advertisements or announcements.
- Removed documents without an author in the metadata, as these were usually journal business.
- Performed a general cleaning on titles to fix bad scans, titles with lots of spaces, bad formatting, and so on, to better identify journal business.
- Identified articles with the same raw text, which were almost all book reviews or journal business. The majority of the removal (7399 documents) was done in this step.
- Found articles that all share the same page number (as well as volume/issue number) in metadata, which usually indicates that they are very short book reviews, all on the same page. The author is usually listed as the “physics-review-committee” or the editor.
- Removed articles with specific headers: ANNOUNCEMENT (#128), NEWS (#141), AAPT (#189), BOOKS RECEIVED (#153), Service Citation (#49), BOOK REVIEWS (#76), SCRAPS (#52), LETTERS TO THE EDITOR (#68).

## Notebook 02
### Second Dataset Cleaning

In the second dataset cleaning, articles were removed based on specific text in the title:
- For TPT: 'Correction', 'BOOKS FOR YOUNG PEOPLE', 'century textbook illustrations'.
- For PE: “News”, "SIGNING OFF”, “PEOPLE”, “People”, “Reply to comment”, “Erratum”, “book review”.

Moreover, articles where authors or article text was missing were removed. 

Finally, articles with less than 500 words were removed. 

### Final Dataset

The final dataset contained:
- 6445 articles from PE (1966-2024)
- 7203 articles from TPT (1963-2020)

## Notebook 03
- We improved the correctness of texts by removing all un-needed text before titles

## Authors

- Martina Caramaschi
- Tor Ole B. Odden

## Repository

[GitHub Repository](https://github.com/martinacaramaschi/TPT-PE-thematic-analysis)

## License

[MIT License](LICENSE)

## Contact

For any questions, please contact [Martina Caramaschi](https://github.com/martinacaramaschi).
