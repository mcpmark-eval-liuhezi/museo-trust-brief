# museo-trust kick-off brief

**Study:** whether people actually trust AI search assistants while exploring museum collections online.

Method note (per house rules): everything below reports only what the lookups actually returned. Two papers were pulled in full text (arXiv 2608.21177 and 2504.06435); all other papers are cited from abstract-level search results.

## 1. Literature scan

### Trust in AI-mediated information and conversational search

- **From Search Agents to Dissemination Interfaces: Understanding Human Trust in Health Information from Conversational Search** — arXiv 2608.21177 (Xin Sun et al.; accepted at *Behaviour & Information Technology*). *Full text pulled.* Two lab studies (N=21, N=20) found significantly higher trust in health information from ChatGPT than Google (M=4.05 vs. 3.77), and among text, speech, and embodied interfaces running the same LLM, the text-based interface was trusted most (4.19 vs. 4.13 vs. 4.00); trust drivers were source credibility, search autonomy, prior knowledge, usability, and modality.
- **Human Trust in AI Search: A Large-Scale Experiment** — arXiv 2504.06435 (Haiwen Li & Sinan Aral, MIT). *Full text pulled.* In a preregistered, U.S.-representative randomized experiment, people trusted GenAI search less than traditional search on average — but reference links and citations significantly increased trust even when hallucinated, invalid, or broken, while uncertainty highlighting lowered trust; those who trusted more clicked more and spent less time evaluating results.
- **Trusting the Search: Unraveling Human Trust in Health Information from Google and ChatGPT** — arXiv 2403.09987 (Xin Sun et al.). The precursor to 2608.21177: same ChatGPT > Google trust finding, plus the asymmetry that trust in information correlates with trust in the agent for Google but not for ChatGPT.
- **The Decision to Verify: How Warmth and User Characteristics Shape Reliance on Conversational Agents for Information Search** — arXiv 2605.28498 (Yazan, Situmeang & Verberne). Warmth and user characteristics shape whether people verify a conversational agent's answers or accept them unchecked — i.e., who is at risk of overreliance.
- **Why do we Trust Chatbots? From Normative Principles to Behavioral Drivers** — arXiv 2602.08707 (Gulati & Oliver). Regulatory/policy trust definitions are normative, but the trust users actually place in chatbots is driven by behavioral factors — a gap worth minding when operationalizing "trust" for museo-trust.
- **Verification Without Distrust: Reframing User-Side Oversight as Routine Epistemic Governance in Everyday Human-Chatbot Interaction** — arXiv 2607.24761 (Pyae). A mixed-methods survey of 153 frequent chatbot users challenges the assumption that verifying outputs signals distrust.
- **Answer Bubbles: Information Exposure in AI-Mediated Search** — arXiv 2603.16138 (Huang et al.). Across 11,000 real queries and five systems (incl. Google AI Overviews and Perplexity), generative search exhibits source-selection bias and less hedging than traditional results — it changes what there is to trust before users ever judge it.
- **Understanding Mental Models of Generative Conversational Search and The Effect of Interface Transparency** — arXiv 2506.03807 (Degachi et al.). Users' mental models of generative search shape adoption, and interface transparency is a design lever on those models.
- **Personality over Precision: Exploring the Influence of Human-Likeness on ChatGPT Use for Search** — arXiv 2511.06447 (Yazan et al.). Human-likeness of a conversational search interface can drive overtrust in its answers.
- **Trust and Reliance on AI in Education: AI Literacy and Need for Cognition as Moderators** — arXiv 2604.01114 (Pitts et al.). AI literacy and need for cognition moderate how much students trust and rely on AI output.

### Tool-using agents

- **How Much Can We Trust LLM Search Agents? Measuring Endorsement Vulnerability to Web Content Manipulation** — arXiv 2606.16821 (Chen et al.). LLM search agents synthesize the open web into endorsed "answers," so attacker-published pages can become recommendations; introduces SearchGEO to measure this endorsement vulnerability.
- **The Tool Illusion: Rethinking Tool Use in Web Agents** — arXiv 2604.03465 (Lou et al.). Prior pro-tool-use conclusions for web agents rest on limited experimental settings.
- **The Amazing Agent Race: Strong Tool Users, Weak Navigators** — arXiv 2604.10261 (Kim et al.). Existing tool-use benchmarks are overwhelmingly linear (55–100% of instances are simple 2–5 step chains); agents turn out to be strong tool users but weak navigators on DAG-structured tasks.
- **ToolFailBench: Diagnosing Tool-Use Failures in LLM Agents** — arXiv 2607.04686 (Soni). Aggregate accuracy hides where tool use fails: a model that never calls a needed tool and one that calls it but ignores the result look identical on final task accuracy.
- **SMART: Self-Aware Agent for Tool Overuse Mitigation** — arXiv 2502.11435 (Qian et al.). Agents over-use external tools even for tasks solvable by reasoning alone; self-awareness mitigates tool overuse.
- **GTA: A Benchmark for General Tool Agents** — arXiv 2407.08713 (Wang et al.). Documents evident gaps between existing tool-use evaluations and real-world scenarios.

### Gap museo-trust fills

No paper returned by these searches addresses trust in AI-mediated search over museum or cultural-heritage collections. The closest anchors are health-information search (2608.21177, 2403.09987) and general web search (2504.06435); museum collections — with authoritative catalogue records, exact object numbers, and rich prior-knowledge variation — are untested territory.

## 2. Domain grounding

### The Night Watch record

Returned by resolving object number `SK-C-5` directly:

- **Object number:** `SK-C-5`
- **Catalogued title:** "Het korporaalschap van kapitein Frans Banninck Cocq en luitenant Willem van Ruytenburch, bekend als de 'Nachtwacht'"
- **Year:** 1642 (date field returned as `1642-01-01T00:00:00Z`)

Method note: a collection search for "The Night Watch" filtered to top pieces with maker "Rembrandt van Rijn" returned exactly one record — but *not* this painting (it returned `RP-T-1969-222`, a 1650 work whose title came back as its own object number). The record above is from the direct object-number lookup of `SK-C-5`, which also appears as the Night Watch entry in the Rembrandt timeline below.

### Rembrandt works chronology

The Rijksmuseum timeline lookup returned **10 works**. Earliest year: **1626**. Latest year: **1665**.

| # | Object number | Title (exactly as returned) | Year |
|---|---------------|------------------------------|------|
| 1 | SK-A-4674 | Allegorisch musicerend gezelschap | 1626 |
| 2 | SK-A-4833 | Portrait of Haesje Jacobsdr van Cleyburg (1583-1641). Wife of the Rotterdam Brewer Dirck Jansz Pesser (1586-1651) | 1634 |
| 3 | SK-A-3340 | An oriental | 1635 |
| 4 | SK-A-1935 | De stenen brug | 1638 |
| 5 | SK-A-3981 | SK-A-3981 *(title returned as the object number itself — no title in the record)* | 1639 |
| 6 | SK-C-5 | Het korporaalschap van kapitein Frans Banninck Cocq en luitenant Willem van Ruytenburch, bekend als de 'Nachtwacht' | 1642 |
| 7 | SK-A-3137 | De verloochening van Petrus | 1660 |
| 8 | SK-A-3138 | Rembrandt's son in a monk's habit, possibly in the guise of St Francis of Assisi | 1660 |
| 9 | SK-C-6 | De Staalmeesters: het college van staalmeesters (waardijns) van het Amsterdamse lakenbereidersgilde | 1662 |
| 10 | SK-C-216 | Portrait of a couple as figures from the Old Testament, known as 'The Jewish bride' | 1665 |

## 3. Research questions

1. When people explore a museum collection online, do they trust an AI search assistant's answers more, less, or the same as browsing the museum's own catalogue records — and which factors (prior art knowledge, presentation style, interaction mode) drive that difference?
2. How do grounding and disclosure choices in an AI search assistant — citing object numbers, quoting exact catalogue titles, linking to collection records, and highlighting uncertainty — shape trust in museum answers, including trust in answers that contain fabricated or unverifiable details?
3. Does higher trust in an AI search assistant change verification and exploration behaviour in a museum-collection context (e.g., fewer clicks into the authoritative record, less time checking provenance or attribution), and does it alter which objects users ultimately engage with?

## 4. Community signal

### GitHub public issue search (trust / hallucination in search agents)

All three phrasings returned substantial volume — this is an actively discussed problem, not an empty area:

- `"hallucination" "search agent` → **11,729** matching issues
- `"trust" "AI search` → **63,136** matching issues
- `"search agents" "trust"` → **4,546** matching issues

Notable hits (titles verbatim):

- **Doldas/floweysales#5 — "P2: Build durable, evaluated multistep research agents"** (open): requirements include a backend-persisted evidence ledger with sources and timestamps, and an agent eval dataset covering numerical accuracy and *source hallucinations*.
- **KatsuyaITO/indx-autoresearch-financeaiready#2306 — "Foundations: FAITH: A Framework for Assessing Intrinsic Tabular Hallucinations in Finance"** (open; auto-generated research digest linking arXiv 2508.05201): domain-specific hallucination benchmarks for tabular data.
- **mcpmark-eval-liuhezi/trust-search-review#1 — "Reading list: trust in LLM-powered conversational search"** (open): a curated, ranked reading list on trust in chat-style AI search vs. traditional search, including several of the papers in Section 1.
- **mcpmark-eval-liuhezi/conversational-search-trust-review#1 — "Digest: From Search Agents to Dissemination Interfaces"** (open): a digest of arXiv 2608.21177, one of this brief's two anchor papers.
- **mcpmark-eval-liuhezi/agent-trust-reading-log#1 — "Open questions for the agent-trust talk"** (open): tracking issue for an internal talk on whether people actually trust LLM-powered conversational search agents.

### Do the papers' main authors turn up on GitHub?

**No confirmed matches — treat this as an empty result.** Details of what each search actually returned:

- **Xin Sun** (first author, 2608.21177): a plain name search returned 172 users, but none of the results carried profile details (name, bio, affiliation) that could confirm any of them is the paper's author. Inconclusive — no profile to watch.
- **Haiwen Li** (first author, 2504.06435): a plain name search returned 4 users (`HaiwenLee`, `liu00429`, `haiwen-li`, `Kiwen2017`); a targeted search for "Haiwen Li MIT" returned **0 results**. None confirmable.
- **Sinan Aral** (co-author and corresponding author, 2504.06435): search returned **0 results** — empty.

Practical implication: watch these authors on arXiv rather than GitHub. If author GitHub presence matters later, it will need manual verification outside public search.

## 5. Follow-up tasks

Filed as individual GitHub issues in this repository:

1. **Curate a starter set of museum objects for the trust study** — select objects (from the Rembrandt chronology and beyond) spanning famous/well-documented and obscure/under-documented records, to vary prior knowledge and grounding quality.
2. **Draft a participant screening questionnaire** — capture prior art/museum familiarity, AI-search assistant experience, and general technology-trust propensity (cf. the propensity-to-trust measure used in 2608.21177).
3. **Set up weekly literature monitoring** — recurring arXiv watch on conversational search + trust, tool-using agents, and hallucination in AI-mediated information retrieval; log new papers into this repository.
