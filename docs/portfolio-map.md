# Portfolio evidence map

| Capability | Evidence |
| :--- | :--- |
| Mechanical CAD automation | SolidWorks API modules for assembly/document handling, sketch geometry, hole-feature experiments, and annotations |
| Drawing quality control | Drawing Verification AI: title-block cell isolation from CAD rectangle entities, ruled-table BOM parsing, ISO-style zone-grid detection, general-tolerance parsing, checklist filling, cross-drawing BOM and NEXT ASSY. consistency rules |
| Local AI integration | Drawing Verification AI: Gemma 4 E4B via Ollama with thinking mode, text-first structured prompts, JSON findings with parse-failure fallback; Gemma used for extraction while deterministic rules decide mismatches |
| Automation architecture | Engineering Board architecture designed by Christin: single-host React/Node.js/SQLite system, REST API, live updates, concurrency and review workflow; VBA event handlers and staged import pipeline; MATLAB separation of domain databases, workflow generation, scheduling and UI; staged extract → structure → audit pipeline in Python |
| Engineering units and data | Inch-to-meter conversion, coordinate grouping, Excel input validation, quantity-based duration models, decimal-place tolerance tiers |
| Manufacturing workflow modeling | Machining, composite, procurement, PCB, enclosure, prototype and integration streams |
| Dependency analysis | Directed graph, topological schedule pass, backward slack pass and longest-path extraction |
| Engineering-team coordination | Engineering Board job lifecycle, workload views, drawing review, audit history, and local-network deployment; private repository, architecture credited to Christin |
| Testing | Drawing Verification AI pytest suite on a synthetic vector drawing, covering extraction, structuring, zone grid, tolerance parsing and cross-file rules without a model |

Python is now established by the Drawing Verification AI repository. The supplied files do not establish separate HFSS, FEA, vehicle dynamics or production-deployment projects. These can be added when source and demonstrations are supplied. RF/antenna workflow modeling is supported; RF solver automation is not established by the MATLAB task names. The Drawing Verification AI dimension matcher module and its real validation drawing are not published, so that tool's end-to-end result rests on the original development run.
