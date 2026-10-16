# docs

Technical write-ups and knowledge-sharing articles drawn from hands-on project experience: building, migrating and modernizing large-scale software systems across cloud-native platforms, enterprise architecture and applied GenAI.

These are written as blog-style articles rather than reference documentation. Each one tries to capture what was actually learnt on real projects: the problems teams faced, the approaches that worked, the trade-offs, and the lessons that can be reused. Some articles are also published on other forums, and this repository is the home for the source text and images.

> **This is a living collection.** New write-ups will be added over time as I work on new problems and learn from them. Watch or star the repository to follow along.

## Articles

| Article | Summary | Also published at |
|---------|---------|-------------------|
| [AWS in the Sports Technology Industry](AWSinSportsTechnologyIndustry/article.md) | Why sports betting and content platforms differ from banking or e-commerce (bursty, event-driven traffic, millisecond latency, strict availability and regulation). How a cloud-native architecture on AWS, guided by the Well-Architected Framework, addresses them. Covers the results seen after migration and the lessons learnt. | [Thoughtworks Insights – The evolving landscape of the sports industry](https://www.thoughtworks.com/insights/blog/digital-transformation/evolving-landscape-sports-industry) (also shared on LinkedIn) |
| [Some Learnings from Large Projects](someLearningsFromLargeProjects/article.md) | Lessons from large, complex programmes in digital consumer industries: why modernization is more than a cloud migration, and the practices that helped. These include Architecture Advice Forums and ADRs, domain-driven / platform-first design, thin-slice delivery, "tech follows business", cross-functional requirements and documentation. It also covers what goes wrong when teams don't share information. | This repository only, for now |
| [0 → 1 with RAG](0to1withRAG/article.md) | A practical starting point for engineers new to Retrieval-Augmented Generation, using a fictional bank's internal knowledge assistant as a running example. Covers terminology, the building blocks (ingestion, chunking and embeddings, vector database, retrieval, reranking, response generation), safety and governance, evaluation metrics (Recall@k, Precision@k, MRR), common failure scenarios, and the path from prototype to production. | This repository only, for now |

## Repository layout

```
docs/
├── AWSinSportsTechnologyIndustry/
│   ├── article.md        # article text in Markdown
│   ├── article.docx      # original Word version
│   └── images/           # diagrams referenced by article.md
├── someLearningsFromLargeProjects/
│   ├── article.md
│   └── article.docx
├── 0to1withRAG/
│   ├── article.md
│   ├── article.docx
│   └── images/
└── README.md
```

Each article lives in its own folder. `article.md` is the version to read on GitHub, with relative image links that render in the browser. `article.docx` is the original Word document, which is handy for publishing elsewhere. Articles with diagrams keep them in an `images/` subfolder next to the text.

## How to read these

- **Browse on GitHub:** open an `article.md` from the table above. Diagrams and formulas (the RAG metrics use LaTeX math) render natively.
- **Clone locally:** `git clone git@github.com:sudgargcoding/docs.git`, then open the Markdown in any editor or previewer.

## Who this is for

Software engineers, architects and tech leads who want practical, experience-based perspectives rather than vendor documentation. In particular:

- teams working on modernization or cloud migration of large systems,
- engineers in latency-sensitive, event-driven domains such as sports tech, betting and real-time platforms,
- engineers getting started with GenAI and RAG in an enterprise setting.

## Notes

- The articles reflect my own experience and opinions. They are not official guidance from any employer or client.
- Client and product details are kept general.
- Feedback, corrections and topic suggestions are welcome. Open an issue or reach out.

## Roadmap

More write-ups are planned. Topics in the pipeline will follow the same theme of lessons from real projects: architecture practices, cloud-native delivery and applied GenAI. This section will be updated as articles land.
