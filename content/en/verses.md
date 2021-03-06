---
title: Get Verses
subtitle: This is a sample file
# menuTitle: Verses
description: ""
position: 2
category: "Verses"
---

Get list of [verses]()

You can filter verses by <code>chapter</code>, <code>page</code>, <code>juz</code>, <code>rub</code> and <code>hizb</code>.

### Customizing the results

# Welcome to StackEdit!

Hi! I'm your first Markdown file in **StackEdit**. If you want to learn about StackEdit, you can read me. If you want to play with Markdown, you can edit me. Once you have finished with me, you can create new files by opening the **file explorer** on the left corner of the navigation bar.

# Files

StackEdit stores your files in your browser, which means all your files are automatically saved locally and are accessible **offline!**

API will send minimal ayah and words fields, ayah [Translation](), [Tafsir]() or [AudioFile]() is also not included by default. You can customize the results using following query strings.

<ul>
    <li>
        <p><code>words</code> words are inlcuded by default, pass any fasly value(false, f, 0) if you don't want to include ayah words</p>
    </li>
    <li>
        <p><code>translations</code> comma separated ids of translations you want to fetch for each ayah. See <a href="/v4/resources/translations" class="undefined">Translations</a> endpoint to fetch list of available translations.</p>
    </li>
    <li>
        <p><code>tafsirs</code> comma seperated ids of tafsirs you want to fetch for each ayah. See <a href="/v4/resources/tafsirs" class="undefined">Tafsirs</a> endpoint to fetch list of available tafsirs.</p>
    </li>
    <li>
        <p><code>audio</code> single integer value of recitaiton you want to fetch for each ayah. See <a href="/v4/resources/recitations" class="undefined">Recitations</a> endpoint for available recitations.</p>
    </li>
    <li>
        <p><code>fields</code> comma seperated list of  <a href="/v4/models/verse" class="undefined">Verse</a> fields. Use this query string if you need to fetch more fields of each ayah.</p>
    </li>
    <li>
        <p><code>word_fields</code> api is sending <code>code_v1</code> QCF font for words. Use this query string if you need to fetch other fields of each words. e.g <code>word_fields=text_uthmani</code> will return Uthmani text of each word.</p>
    </li>
    <li>
        <p><code>translation_fields</code> if you need to fetch more fields of translations. See translation model for available fields.</p>
    </li>
    <li>
    <p><code>tafsir_fields</code> if you need to fetch more fields for tafsir.</p>
    </li>
</ul>

## By Specific Verse By Key

```bash
/verses/by_key/{verse_key}
```

Get a specific ayah with key. Key is combination of surah number and ayah number. <code>1:1</code> is first ayah of first surah for example.

<code>10:5</code> is 5th ayah of 10th surah.

<code>https://api.quran.com/api/v4/verses/by_key/{verse_key}?language=en&words=true</code>

<!-- ```bash
https://api.quran.com/api/v4/verses/by_key/{verse_key}?language=en&words=true
``` -->

<api-call></api-call>

// TODO:
Here goes API testing tool

```json
{
  "message": "?????????? ?????? api is working fine. Please see the docs for each version for more help.",
  "versions": {
    "v3": "https://quran.api-docs.io/v3/getting-started/introduction",
    "v4": "https://quran.api-docs.io/v4/getting-started/introduction",
    "qdc": "https://quran.api-docs.io/qdc/getting-started/introduction",
    "graphql": "https://api.quran.com/graphql-playground"
  }
}
```
