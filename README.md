# Suggestive Search for CS-Cart

**🛑 PREMIUM ADD-ON: This repository does not contain the open-source code. It serves as the official listing and documentation page for the WebGraphiq premium add-on.**

**Suggestive Search** is a live AJAX search, autocomplete, and typo-tolerant search add-on for CS-Cart and Multi-Vendor. As a shopper types, matching products, categories, and vendors appear in a drop-down. Misspellings can still find the right product, and the Enter / Search results page uses the same field rules as the dropdown.

## [🛒 Buy & View Live Demo](https://www.webgraphiq.com/suggestive-search.html)

One-time license. No monthly search-service fee. The current price and the live demo are on the product page.

## Why store owners use it

- Shoppers see matches while they type, instead of waiting for a full search-results page.
- **Typo tolerance:** close spellings still find products in the dropdown and after Enter (for example `automx` → Automatic).
- Only the product fields you tick are searched — live suggestions and the full results page use the same rules.
- Each result can show a thumbnail, the product code, and the price.
- A single match can open the product page when the shopper presses Enter or the search icon.
- Search phrases are stored in the admin, so you can see what people actually look for.
- The add-on installs as a normal CS-Cart package and does not replace core files.

## What shoppers see

- A drop-down of products, categories, and — on Multi-Vendor — vendor companies.
- Matching text highlighted in a color you set.
- Optional thumbnails, with a larger image preview on hover.
- A “view all results” link when there are more matches than the drop-down shows.
- Optional incremental search that keeps narrowing the same result set as typing continues.
- Fuzzy matches when normal search finds too few products (if typo tolerance is enabled).

## Typo tolerance and search index

- Normal (exact / partial) search runs first. If fewer than **N** products are found, fuzzy matching runs on a dedicated search index (default N = `3`; set `0` to run fuzzy only when there are zero hits).
- Fuzzy works in the **live dropdown** and on the **full search results page**.
- Accented letters are folded to plain letters. There is no language-specific stemmer.
- The index updates when you save or delete a product. A full **Rebuild search index** sits under Website → Search keywords history.
- Changing which Products fields are searched schedules a rebuild (admin notification). An optional **weekly cron** is a safety net.

## What you control

- Minimum characters before a search starts, and how many products, categories, or companies are listed.
- Product search in the name, short description, full description, **product keywords** (CS-Cart Search words), meta keywords, and product code. Default: name + product keywords.
- Match mode: any of the words, all of the words, or the exact phrase.
- Category search in the category name and meta keywords.
- Vendor search in the company name (Multi-Vendor).
- Whether the full search-results page sorts newest items first.
- Whether phrases are stored while the shopper types, when they submit the search, or both.
- Typo tolerance on/off, the N threshold, index rebuild chunk size, optional live-query cache TTL, and index cron password / max age.

## Search keyword history

Under **Website → Search keywords history** you can review, delete, and clear stored phrases, and rebuild the search index. History is kept per language and per storefront company, with standard CS-Cart pagination.

## Requirements

- CS-Cart or Multi-Vendor **4.12.1** or newer, including **4.21**
- PHP **8.3** or a current 8.x release used by that shop
- Not compatible with the Searchanise add-on

## This repository

<p align="center">
  <a href="https://www.webgraphiq.com/suggestive-search.html">
    <img alt="Buy and view the live demo" src="https://img.shields.io/badge/CS--Cart-Buy%20%26%20View%20Live%20Demo-28a745?style=for-the-badge&labelColor=1A365D">
  </a>
</p>

<p align="center"><strong>One-time license · live search · typo tolerance · no monthly search fee</strong></p>

This is the public product listing. The add-on package, license checks, and source files are not published here. After purchase, the package is readable PHP under the WebGraphiq commercial license, installed from your WebGraphiq account.

Support: [webgraphiq.com](https://www.webgraphiq.com) · webgraphiq@gmail.com

© WebGraphiq. All rights reserved. [License](https://www.webgraphiq.com/license.html)

## Other Premium CS-Cart Add-ons by WebGraphiq

More CS-Cart and Multi-Vendor add-ons are listed on the [WebGraphiq GitHub profile](https://github.com/webgraphiq).
