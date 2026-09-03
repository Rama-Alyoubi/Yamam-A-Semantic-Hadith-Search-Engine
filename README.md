# Yamam — يمام

**A Semantic Hadith Search Engine**

Yamam retrieves relevant hadith by understanding the *meaning* of a question rather than matching keywords. Traditional platforms require the reader to already know the right wording; Yamam lets them ask in natural Arabic and surfaces contextually related narrations.

## Project overview

Yamam is a search engine designed to change how users interact with hadith literature. Using advances in natural language processing and semantic search, it provides an intuitive platform to explore and discover hadith with accuracy that keyword search cannot reach.

The project employs a large language model — specifically **AraGPT** — to understand and analyse Arabic text semantically. This lets Yamam interpret the intent and context behind a query rather than matching surface forms.

## The problem

Arabic religious texts are hard to search. Classical vocabulary, diacritics, and the sheer size of the corpus mean keyword search misses relevant narrations whenever a reader phrases a question in modern Arabic. Students, researchers, and general readers end up browsing rather than searching.

## How it works

```
Large source files  →  chunked into passages  →  embedded as vectors
                                                        ↕
                              user query  ⟷  semantic retrieval  ⟷  AraGPT
```

1. The hadith corpus is split into smaller passages so retrieval operates at a meaningful granularity
2. Passages are embedded and stored in a vector index
3. A user question is embedded with the same model and matched against the index
4. **AraGPT** supplies the Arabic language understanding that captures the deeper semantics of both query and passage

## Features

- **Semantic search** — comprehends and responds to natural language queries via AraGPT
- **User-friendly interface** — a streamlined design for an effortless search experience
- **Advanced data processing** — preprocessing and structuring of hadith data for retrieval

## Goals

- Return precise, context-aware results grounded in the semantics of the question
- Make it easy to find narrations on a given subject, ethic, or teaching
- Support researchers, scholars, and general readers in exploring hadith more effectively

## Team

Rama Mohammed Alyoubi · Rimas Alshehri · Rozouf Bandar Alghamdi
University of Jeddah

## Acknowledgment

Developed as part of **The Quran and its Sciences Challenge**, hosted by the University of Jeddah. Our success in this initiative reflects the collaborative effort and support from our mentors and the organizers.

## About this repository

This repository documents the project — its purpose, method, architecture, and results.
The source code is private and is not published here.

---

<div dir="rtl">

## عن المشروع

**يمام** هو نظام بحث دلالي للأحاديث النبوية مدعوم بـ AraGPT، يساعد المستخدمين على الوصول إلى الأحاديث ذات الصلة من خلال فهم معنى السؤال بدلًا من الاعتماد على الكلمات المفتاحية فقط.

يسهّل النظام رحلة البحث للطلاب والباحثين والمهتمين بالمعرفة الإسلامية عبر تقديم نتائج أكثر ارتباطًا بالسياق، وتقليل الوقت اللازم للوصول إلى النصوص المناسبة، ودعم استكشاف الأحاديث بطريقة أوضح وأسهل.

### الأهداف

- تحسين تجربة المستخدم من خلال تقديم نتائج بحث دقيقة ومتعمقة استنادًا إلى السياق الدلالي للاستفسارات
- تسهيل عملية البحث عن الأحاديث ذات الصلة بالمواضيع الأخلاقية والتعاليم الدينية
- دعم الباحثين والعلماء والجمهور العام في استكشاف الحديث بشكل أكثر فعالية وسهولة

</div>
