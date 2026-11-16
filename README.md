# Roger Holenweger

Systems engineer in Bangkok, UTC+7. Full-time in Thailand from December 2026,
or part-time async contract work for remote employers. Swiss national.

Python since 2002, Java 2008-2012, Rust since 2025 by specification. I decide
what goes into a system and what has to be true of it; a coding agent writes the
code and the tests; I review, comment and measure what it produces; the compiler,
the strict lints and the suite decide whether it ships.

## 2025 to now, self-funded

Four systems. One in production since October 2026; three stopped at a measured wall.

**nanotoll** (June to October 2026, live since October 2026) - a Rust service that compresses LLM payloads at a fixed price per
call, by mode. 17 crates, about 51,000 lines, 854 test functions, byte-identical
output across six parallel worker profiles. Metered billing: HTTP 402 challenge,
credit ledger in SQLite/WAL, USDC deposits on Base credited at 12 confirmations.
Each request returns a 20-field Ed25519-signed receipt, so a caller can prove what
was done to their payload without trusting the operator. MCP server for agent
runtimes; the 30 s p95 ceiling is held by an admission gate sized to a measured
latency curve, not to an opinion.

**chesig** (March to June 2026) - chess models trained on 3M grandmaster games, 50 million positions:
GNN and deep learning pipelines on rented GPUs, Haystack with LLMs turning the
positional features detected in a position into human-readable commentary, and a
Weaviate RAG to find similar positions. Stopped at a scaling wall above 200 GB of
RAM.

**Alpha Foundry** (December 2025 to March 2026) - a NEAT graph grown from features extracted from candle data
and indicators, rewired by evolutionary computation. Features clustered by
correlation, one survivor per cluster by recursive elimination, then a boosted
ranking that keeps twelve of them for each walk-forward window; Bayesian
hyperparameter search. Stopped when the viability gate found no out-of-sample
edge. That is an answer, so I stopped.

**KCE** (August to December 2025) - a neurosymbolic corporate due-diligence knowledge graph on Memgraph and Weaviate,
built from GLEIF, ICIJ, SEC and OpenWiki data, plus a crawler that pulled nodes and
edges out of search results. An agent decided which parts of the graph were worth
exploring; an LLM decided whether two records were the same company before merging
nodes. That merge could not be audited, and a wrong merge is inherited by
everything downstream, so I stopped. Pitched to Southeast Asian VCs, no reply.

## Before that

**CityData.ai, 2015-2025.** Location intelligence on a graph database:
Neo4j modelling, geo-temporal correlation, matching human-submitted addresses to
geolocated values, building trajectories inside virtual maps. Wrote the Linux and
bash ETL that processed over 1 TB a day and inferred a 20-million-person
population distribution for New York City from public census data: households by
block, ages, incomes, genders. Full-stack developer in Zürich 2015-2018, then Head
of Engineering in Bangkok 2018-2025.

**Events.com, 2013-2015.** Senior Python developer. Cloud cost cut by rescaling,
centralised logging on AWS, Django APIs, event-text deduplication.

**Gablit, 2012-2013.** Python developer. Plugin-based classifier framework, NLTK
Naive Bayes with a retrain cycle, Twitter stream mining, Jenkins CI.

**NoMagic Asia, 2008-2012.** Java. BPMN 2.0 modelling, BPMN to XPDL
transformation, Cameo DataHub serialisation.

## Toolbox

Python (PyTorch, pandas, numpy, Pydantic), Java, SQL, Neo4j, Memgraph, Weaviate,
Docker, Linux and bash, AWS, GCP, RunPod, Hetzner, Netcup. Rust as agent-directed
work, described above.

## Looking for

Full-time work in Thailand from December 2026: backend and data engineering, data
pipelines, evaluation harnesses, graph work. On-site, hybrid or remote. Not a
leadership role.

For remote employers, part-time async contract work: 20-30 hours a week over three
or four days. I invoice as an individual from Thailand, in USD.

[roger.holenweger@proton.me](mailto:roger.holenweger@proton.me)
[linkedin.com/in/roger-holenweger](https://www.linkedin.com/in/roger-holenweger)
