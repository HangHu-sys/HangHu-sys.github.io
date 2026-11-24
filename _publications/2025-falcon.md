---
title: "Fast Graph Vector Search via Hardware Acceleration and Delayed-Synchronization Traversal"
collection: publications
permalink: /publication/falcon/
redirect_from:
  - /publication/2024-06-24-Accelerating Graph-based Vector Search via Delayed-Synchronization Traversal
excerpt: "Falcon combines an FPGA accelerator with delayed-synchronization traversal for low-latency graph-based vector search."
# Online publication date from Crossref; the print issue is dated July 2025.
date: 2025-09-04
authors: "Wenqi Jiang, **Hang Hu**, Torsten Hoefler, and Gustavo Alonso."
venue: "Proceedings of the VLDB Endowment"
volume: 18
issue: 11
pages: "3797–3811"
paperurl: "https://www.vldb.org/pvldb/vol18/p3797-jiang.pdf"
codeurl: "https://github.com/fpgasystems/Falcon-accelerate-graph-vector-search"
doiurl: "https://doi.org/10.14778/3749646.3749655"
citation: 'Wenqi Jiang, Hang Hu, Torsten Hoefler, and Gustavo Alonso. 2025. Fast Graph Vector Search via Hardware Acceleration and Delayed-Synchronization Traversal. <i>Proceedings of the VLDB Endowment</i> 18(11): 3797–3811. <a href="https://doi.org/10.14778/3749646.3749655">doi:10.14778/3749646.3749655</a>.'
---

[Paper]({{ page.paperurl }}) · [Code]({{ page.codeurl }}) · [DOI]({{ page.doiurl }})

Falcon combines an FPGA accelerator with delayed-synchronization traversal to reduce latency in graph-based vector search. The design pairs a pipelined search engine with a traversal algorithm that exposes more parallel work to the accelerator.
