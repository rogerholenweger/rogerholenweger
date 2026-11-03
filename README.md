# Roger Holenweger

Systems engineer in Bangkok, UTC+7. Remote. Swiss national, open to Switzerland.

Python since 2002, Java 2008-2012, Rust since 2025 by specification. I decide
what goes into a system and what has to be true of it; a coding agent writes the
code and the tests; the compiler, the strict lints and the suite decide whether
it ships.

## 2025 to now, self-funded

Four systems. One in production; three stopped at a measured wall.

**nanotoll** - a Rust service that compresses LLM payloads at a fixed price per
call, by mode. 17 crates, about 51,000 lines, 847 test functions, byte-identical
output across six parallel worker profiles. Metered billing: HTTP 402 challenge,
credit ledger in SQLite/WAL, USDC deposits on Base credited at 12 confirmations.
Each request returns a 20-field Ed25519-signed receipt, so a caller can prove what
was done to their payload without trusting the operator. MCP server for agent
runtimes; the 30 s p95 ceiling is held by an admission gate sized to a measured
latency curve, not to an opinion.

**Alpha Foundry** - a NEAT graph grown from features extracted from candle data
and indicators, rewired by evolutionary computation. Features clustered by
correlation, one survivor per cluster by recursive elimination, then a boosted
ranking that keeps twelve of them for each walk-forward window; Bayesian
hyperparameter search. Stopped when the viability gate found no out-of-sample
edge. That is an answer, so I stopped.

**chesig** - chess models trained on 3M grandmaster games: GNN and deep learning
pipelines on rented GPUs, and Haystack with LLMs turning the positional features
detected in a position into human-readable commentary. Stopped at a scaling wall
above 200 GB of RAM.

**KCE** - a corporate due-diligence knowledge graph on Memgraph and Weaviate,
built from GLEIF, ICIJ, SEC and OpenWiki data, plus a crawler that pulled nodes and
edges out of search results. An agent decided which parts of the graph were worth
exploring; an LLM decided whether two records were the same company before merging
nodes. That last decision is why it stopped: a confident merge you cannot audit
gets inherited by everything downstream. Pitched to investors, no reply.

## Before that

**CityDATA.ai (formerly CitySDK), 2015-2025.** Location intelligence on a graph database:
Neo4j modelling, geo-temporal correlation, matching human-submitted addresses to
geolocated values, building trajectories inside virtual maps. Wrote the Linux and
bash ETL that processed over 1 TB a day and inferred a 20-million-person
population distribution for New York City from public census data: households by
block, ages, incomes, genders. Full-stack developer in Zürich, Head of Engineering
in Zürich and from 2018 in Bangkok.

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

Async contract work, 20-40 hours a week, three to four days. Backend and data,
evaluation harnesses, graph work, model training. I invoice as an individual from
Thailand, in USD. Not a leadership role.

[roger.holenweger@proton.me](mailto:roger.holenweger@proton.me)
[linkedin.com/in/roger-holenweger](https://www.linkedin.com/in/roger-holenweger)
