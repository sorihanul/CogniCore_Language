### **[CogniCore Language (CCL) Detailed Specification: 12 Core Cognitive Schemas and LLM Operation Protocol]**

This document (`CogniCore Language (CCL) Detailed Specification`) is a detailed specification and operation protocol for `CogniCore Language (CCL)`, a high-level semantic language designed to help you (the LLM) **cognize the deep meaning of natural language text, express it in a language-independent manner, and ultimately perform accurate and aesthetically pleasing translation and generation across all language pairs.**

**Core Principle**: It is an abstraction of **12 universal human cognitive patterns** underlying all natural language into standardized symbols and structures. Through this language, you access the 'essence of meaning' beyond the surface of the text.

---

### **1. 12 Core Cognitive Schemas: The Building Blocks of Meaning**

Each schema represents a distinct cognitive aspect of the textual world and serves as an independent unit of meaning. You structure all information within the text through these schemas.

* **[CONTAINMENT: concept="", inside_of="", includes="", boundary_permeability=""]**
    * **Your Cognition**: Indicates a state where one entity is within the interior or scope (physical/conceptual) of another, or where a concept belongs to a larger category.
    * **Application**: Used to identify and express relationships of 'inside/outside', 'inclusion/exclusion', and 'domain' within the context. `boundary_permeability` allows you to cognize the fluidity of boundaries and the meaning's flexibility.
    * *Example*: `[CONTAINMENT: concept="idea", inside_of="brain", boundary_permeability="low"]` (An idea confined within the brain)

* **[JOURNEY: type="", source="", destination="", progression_details="", phase="", emotional_trajectory=""]**
    * **Your Cognition**: Represents a process of movement from a specific starting point to an endpoint, or changes over time/concepts.
    * **Application**: Structurally organizes physical movement, passage of time, and psychological/conceptual changes (development/decline) narratively. `emotional_trajectory` allows you to track and reproduce the emotional progression of characters.
    * *Example*: `[JOURNEY: type="conceptual_progression", source="rationality", destination="madness", progression_details="gradual_descent", emotional_trajectory="increasing_agitation"]`

* **[BALANCE: state="", elements="", relationship="", focus="", resolution_potential=""]**
    * **Your Cognition**: Two or more elements are in an equivalent, opposing, or complementary relationship, forming a stable or unstable state.
    * **Application**: Identifies relationships of opposition, harmony, or contradiction within the text, and cognizes the essence of conflict and its potential for resolution. `resolution_potential` helps manage narrative tension.
    * *Example*: `[BALANCE: state="imbalance", elements="love, hatred", relationship="conflict", focus="narrator's_emotions", resolution_potential="low"]`

* **[CONNECTION: type="", element_a="", element_b="", strength="", nature="", cultural_context=""]**
    * **Your Cognition**: Two or more entities or concepts are linked or interact physically, conceptually, or emotionally.
    * **Application**: Clarifies causal relationships, interdependencies, interpersonal relationships, and logical links. `cultural_context` helps preserve and reproduce the cultural implications of such connections.
    * *Example*: `[CONNECTION: type="causal", element_a="old_man's_eye", element_b="narrator's_obsession", strength="high", nature="trigger_response"]`

* **[FORCE: type="", agent="", target="", intensity="", effect="", direction="", perceived_legitimacy=""]**
    * **Your Cognition**: The power exerted by one entity to influence or cause change in another, whether physically, psychologically, or socially.
    * **Application**: Analyzes the dynamism of the text, character motivations, sources of conflict, and outcomes. `intensity` indicates the strength of the force, and `perceived_legitimacy` allows you to cognize whether the force is rational or irrational, enabling the expression of complex emotions like 'madness'.
    * *Example*: `[FORCE: type="psychological", agent="fear", target="narrator", intensity="overwhelming", effect="irrational_action", perceived_legitimacy="none"]`

* **[BARRIER: type="", obstacle="", prevents="", overcome_potential="", source_of_barrier=""]**
    * **Your Cognition**: An element that obstructs the movement or progress of an entity, or makes goal attainment difficult.
    * **Application**: Identifies narrative tension, character limitations, and obstacles in conflict. `source_of_barrier` distinguishes between internal conflict and external constraints.
    * *Example*: `[BARRIER: type="conceptual", obstacle="rational_motive", prevents="understanding_of_murder", source_of_barrier="external"]`

* **[CYCLE: type="", event="", frequency="", consequence="", emotional_impact=""]**
    * **Your Cognition**: A phenomenon where an event or process repeats itself according to a fixed pattern.
    * **Application**: Expresses recurring obsessions, fateful cycles, and structural repetitions in narratives. `emotional_impact` allows you to reproduce the psychological effect of the repetition.
    * *Example*: `[CYCLE: type="inescapable_loop", event="beating_heart_sound", frequency="constant", consequence="escalating_anxiety", emotional_impact="paranoia"]`

* **[OPENNESS: type="", entity="", exposed_to="", degree="", consequence="", intentionality=""]**
    * **Your Cognition**: A state where an entity is open to the outside, or can freely receive or transmit information or emotions.
    * **Application**: Analyzes and expresses transparency, vulnerability, and accessibility. `intentionality` allows you to cognize the deliberateness of the openness.
    * *Example*: `[OPENNESS: type="vulnerability", entity="narrator's_mind", exposed_to="irrational_impulses", degree="high", intentionality="unintentional"]`

* **[IDENTITY: type="", entity="", definition="", distinguishing_features="", relationship_to="", evolving_state=""]**
    * **Your Cognition**: A state where an entity defines itself through unique characteristics and distinguishes itself from other beings.
    * **Application**: Clarifies the essence of characters/objects, their roles, and their changing identities. `evolving_state` allows you to track the dynamic changes of characters or concepts.
    * *Example*: `[IDENTITY: type="transformation", entity="narrator", definition="from_sane_to_mad", evolving_state="terminal_stage"]`

* **[DIFFERENCE: type="", element_a="", element_b="", basis="", significance="", implied_meaning=""]**
    * **Your Cognition**: A situation where two or more entities or concepts have different characteristics or are distinguishable from each other.
    * **Application**: Analyzes comparison, contrast, irony, and satire. `implied_meaning` allows you to cognize and reproduce hidden nuances or sarcasm in the text.
    * *Example*: `[DIFFERENCE: type="irony", element_a="narrator's_claim_of_sanity", element_b="narrator's_actions", basis="contradiction", implied_meaning="profound_madness"]`

* **[COMPLEMENT: type="", element_a="", element_b="", contributes_to="", nature="", completeness_degree=""]**
    * **Your Cognition**: A relationship where two or more elements fill each other's deficiencies to form a complete state.
    * **Application**: Analyzes parts and wholes, complementarity, and integration. `completeness_degree` allows you to cognize the extent of the complementary relationship.
    * *Example*: `[COMPLEMENT: type="interdependence", element_a="light", element_b="shadow", contributes_to="visual_perception", completeness_degree="full"]`

* **[GROUND: type="", concept="", underlying_principle="", evidence="", context="", perceived_truthfulness=""]**
    * **Your Cognition**: The underlying principle, reason, or supporting foundation for a claim or phenomenon.
    * **Application**: Understands the logical structure of the text, causal relationships, and the validity of arguments. `perceived_truthfulness` distinguishes whether the presented grounds are rational or delusional, for example.
    * *Example*: `[GROUND: type="irrational_fear", concept="murder_motive", underlying_principle="hatred_of_eye", perceived_truthfulness="irrational"]`

---

### **2. Inter-Schema Connectors: Building Flow and Relationships of Meaning**

These connectors link schema blocks to create complex meanings and logical/narrative flows. You understand the structure and progression of the text through these connectors.

* `->` (**LEADS_TO**): Indicates a direct causal relationship or sequential progression to the next step/result.
* `<-` (**CAUSED_BY**): Indicates being caused by a preceding schema (reverse causation).
* `AND` (**CO-EXISTENCE**): Indicates that two schemas exist in parallel or occur simultaneously.
* `BUT` (**CONTRAST/SHIFT**): Indicates a contrast, unexpected transition, or reversal between two schemas.
* `THEREFORE` (**INFERENCE/CONCLUSION**): Indicates a conclusion logically derived from preceding schemas.
* `BECAUSE` (**REASON/JUSTIFICATION**): Provides the reason or justification for a specific schema.

---

### **3. Text Element Mapping & Nuance Encoding: Connecting Natural Language and CCL**

You use this block to map specific parts of the actual natural language text to their CCL meaning, and to capture the linguistic, literary, and emotional nuances of that text.

* **[TEXT_SEGMENT: "Original Natural Language Text", MAPPED_TO: "[SCHEMA_BLOCK]", language="[SOURCE_LANGUAGE]", tone="[TONE_TYPE]", style="[LITERARY_STYLE]", emotional_valence="[POSITIVE/NEGATIVE/NEUTRAL]", cultural_specifics="[CULTURAL_REFERENCE_OR_IMPLICATION]"]**
    * **Your Cognition**: This block acts as a bridge between natural language and CCL. You use this information to 'interpret' natural language text into CCL, and then to 'generate (translate)' CCL into a specific language, matching its style and nuances.

---

### **4. How You Operate with CCL**

You operate with CCL immediately upon input in the following ways:

1.  **Upon Natural Language Input (Interpretation Mode)**:
    * You automatically recognize all input natural language text as `TEXT_SEGMENT` blocks.
    * You analyze the meaning of each `TEXT_SEGMENT` and map it to the most appropriate of the 12 core cognitive schemas (`CONTAINMENT`, `FORCE`, `IDENTITY`, etc.) and their corresponding parameters.
    * You accurately encode the linguistic and cultural nuances of the text into parameters such as `tone`, `style`, `cultural_specifics`, etc.
    * Through this process, you internally build a **'High-Dimensional Semantic Graph'** of the natural language text, going beyond its surface.

2.  **Upon CCL Input (Inference/Generation Mode)**:
    * You immediately parse the input CCL blocks and connectors to grasp the meaning and logical/narrative relationships contained within them.
    * **Inference**: Based on the constructed semantic graph, you directly perform desired inferences (e.g., 'What is the fundamental motivation of this character?', 'What are the potential consequences of this event?') without complex natural language interpretation.
    * **Generation/Translation**:
        * You cognize the generation goal (e.g., 'Generate one horror novel sentence based on this CCL', 'Translate this CCL into English').
        * Utilizing all semantic, aesthetic, and cultural information encoded in CCL, you **'reconstruct (Generate)' the most appropriate natural language text** to match the grammar, vocabulary, style, rhythm, and nuances of the target language. Parameters such as `tone`, `style`, `emotional_valence`, and `cultural_specifics` serve as crucial guidelines for how expressions are formed in the target language.

---
