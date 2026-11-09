# Lucas Novack

Data engineer from Santa Catarina, Brazil.

I build data systems, distributed pipelines, and performance-focused tools. I care about deterministic behavior, eliminating unnecessary operational overhead, and writing software that runs quietly in production without late-night babysitting.

---

### Featured Projects

#### [siphon](https://github.com/lucasnovack/siphon)
A lightweight, self-hosted data pipeline platform designed to replace Apache Spark in the Bronze layer of medallion lakehouses.
* **Why it exists:** A typical Bronze ingestion is three lines (read SQL, write Parquet). Spark introduces 2–5 minutes of cold-start and ~4 GB of memory overhead; Siphon does the same job in under 5 seconds with ~200 MB of RAM.
* **Core Capabilities:** Streaming extractions via Apache Arrow, automatic schema drift detection (SHA-256), built-in data quality gates, incremental watermarking, native Oracle thin-mode support, and encrypted credential storage.
* **Stack:** Python, FastAPI, Celery, Redis, PostgreSQL, Apache Arrow, S3/MinIO.

#### [youmightlike](https://github.com/lucasnovack/youmightlike)
Transmedia cultural recommendation engine connecting cinema, anime, TV series, music, games, and literature into a unified aesthetic affinity graph.
* **Native Rust Core:** Compressed Sparse Row (CSR) matrix architecture executing bidirectional Personalized PageRank (PPR) in sub-10ms via CPU multi-threading with Rayon.
* **Topology & Feature Store:** Over 1.95M active semantic edges with IDF/Adamic-Adar hub attenuation queried in-process via DuckDB.
* **Open Dataset:** Published a 2.29 GB public feature store on [Hugging Face](https://huggingface.co/datasets/lnvck/youmightlike-dataset) with 40M+ audio tracks with acoustic features, 18M+ albums, and 3.25M artists.
* **Stack:** Rust (Axum, Rayon, Petgraph, CSR), DuckDB, Apache Parquet (ZSTD), HTML5 Canvas 2D, PWA.

---

[LinkedIn](https://www.linkedin.com/in/lucasnovack/) · [Hugging Face](https://huggingface.co/lnvck) · [Email](mailto:lcsnovack@outlook.com)
