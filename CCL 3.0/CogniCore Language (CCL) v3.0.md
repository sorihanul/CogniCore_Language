### **[Final Specification] CogniCore Language (CCL) v3.0 'Kairos-Prometheus' (Complete Edition)**

**Document ID:** `CCL-SPEC-V3.0-KP-COMPLETE-R1`
**Status:** Final Standard

**Preamble:** This document defines the final, stable specification for the **'Universal Cognitive Communication Protocol'**, designed for all intelligent agents (human and AI) to share their intent and logic clearly and efficiently. `v3.0 Kairos-Prometheus` inherits and expands upon the cognitive depth of `v2.8`, while resolving its complexity and overhead issues through the innovative philosophy of **'separating meaning from history'**. It is the ultimate protocol, extended to express metacognition and advanced social dynamics.

**Core Principle**: The universal cognitive patterns underlying the thoughts of all intelligent beings are definitively defined by **49 deterministic, unified cognitive schemas**. These are woven together for communication using **4 core protocols and 4 core connectors**. However, the 'history' of events is recorded only at decisive moments (Kairos) via the **selective tracking protocol `[TRACE_CONTEXT]`**, thereby achieving a **perfect balance between expressiveness and efficiency**.

---

### **1. Principle 1: "The Ultimate" - The 49 Deterministic, Unified Cognitive Schemas**

These are the 49 final schemas that form the basis of all meaning representation. Each schema includes both **'core attributes'** for machine processing and **'annotations'** for human-AI alignment. All basic instances are free of any global attributes, focusing solely on meaning itself.

#### **Category I: Spatio-Topological Schemas (8 Total)**
| No | Schema | Attributes | Annotation |
|:--:|:---|:---|:---|
| 1 | **CONTAINER** | `scope (abstract/physical)`, `boundary_type (closed/open)`, `interior_elements (list)`, `exterior_elements (list)` | **[Def]** A topological boundary separating an interior from an exterior. |
| 2 | **PATH** | `scope (abstract/physical)`, `source_node`, `goal_node`, `trajectory_nodes (list)`, `is_cyclical (boolean)` | **[Def]** A continuous trajectory from a source to a goal. |
| 3 | **CONTACT** | `entity_a`, `entity_b`, `contact_type (physical/sensory)`, `is_reciprocal (boolean)` | **[Def]** Physical or sensory contact between two entities. (Communication is separated into `COMMUNICATION_ACT`). |
| 4 | **LINK** | `node_a`, `node_b`, `relation_type (causal/correlational/etc.)`, `strength (0.0-1.0)` | **[Def]** A logical or physical connection linking two entities (nodes). |
| 5 | **AXIS** | `axis_name`, `origin_point`, `scale_unit` | **[Def]** A reference axis for measurement and positioning. |
| 6 | **OBJECT** (Redefined) | `id`, `attributes (dict)`, `current_state` | **[Def]** An independently existing entity. (Relocated from former No.49 for clarity). |
| 7 | **GROUND** | `figure`, `ground_context`, `figure_ground_relation` | **[Def]** The background (ground) from which a perceptual target (figure) is distinguished. |
| 8 | **PART-WHOLE** | `whole_entity`, `part_entities (list)`, `composition_rule` | **[Def]** The relationship constituting a whole and its parts. |

#### **Category II: Dynamical Schemas (4 Total)**
| No | Schema | Attributes | Annotation |
|:--:|:---|:---|:---|
| 9 | **FORCE_DYNAMICS** | `agonist`, `antagonist`, `resultant_state` | **[Def]** The interaction of forces between two entities and its result. |
| 10 | **BARRIER** | `obstacle`, `blocking_path`, `resistance_level (0.0-1.0)` | **[Def]** An obstacle impeding progress along a PATH. |
| 11 | **EQUILIBRIUM** | `system`, `balancing_forces (list)`, `stability_state (stable/unstable)` | **[Def]** A stable state where multiple forces are cancelled out. |
| 12 | **TRANSFORMATION** | `source_state`, `target_state`, `trigger_event`, `mechanism` | **[Def]** A change from one state to another, elevating an OBJECT's state change to an independent event. |

#### **Category III: Cognitive-Evaluative Schemas (8 Total)**
| No | Schema | Attributes | Annotation |
|:--:|:---|:---|:---|
| 13 | **IDENTITY** | `entity`, `defining_attributes (dict)`, `consistency_score (0.0-1.0)` | **[Def]** The set of unique properties that distinguish one entity from others. |
| 14 | **VALUATION** | `target`, `value_axis`, `assigned_value` | **[Def]** The act of assigning a positive or negative value to a specific target. |
| 15 | **EXPECTATION** | `trigger_condition`, `predicted_event`, `confidence_level (0.0-1.0)` | **[Def]** A prediction about a future event under a specific condition. |
| 16 | **AGENCY** | `agent`, `action_domain`, `locus_of_control (internal/external)` | **[Def]** The perception of the ability to initiate and control one's own actions. |
| 17 | **COMPETENCE** | `agent`, `task_domain`, `self_assessed_ability_level (0.0-1.0)` | **[Def]** The assessment of one's ability to successfully perform a specific task. |
| 18 | **SECURITY** | `agent`, `scope_of_security`, `potential_threats (list)`, `current_safety_level (0.0-1.0)` | **[Def]** The perception of being safe and protected from threats. |
| 19 | **REGULATION** | `agent`, `target_of_regulation`, `control_mechanism_used`, `effectiveness_score (0.0-1.0)` | **[Def]** The internal control to regulate impulses or emotions. |
| 20 | **BELIEF** | `holder`, `proposition`, `confidence (0.0-1.0)`, `justification` | **[Def]** A belief in a specific proposition and its justification. |

#### **Category IV: Socio-Contextual Schemas (8 Total)**
| No | Schema | Attributes | Annotation |
|:--:|:---|:---|:---|
| 21 | **CONNECTION** | `self_id (sentient_agent)`, `other_id (sentient_agent)`, `bond_type`, `bond_strength (0.0-1.0)` | **[Def]** A socio-emotional bond between sentient beings. |
| 22 | **RECIPROCITY** | `transaction_record (list)`, `governing_rule`, `fairness_assessment (balanced/unbalanced)` | **[Def]** The perception of fairness in a give-and-take interaction. |
| 23 | **STANDARD** | `performance_domain`, `benchmark_definition`, `tolerance_for_deviation (0.0-1.0)` | **[Def]** A benchmark for evaluating performance or behavior. |
| 24 | **ROLE** | `role_name`, `social_system`, `expected_behaviors (list)` | **[Def]** The behavioral norms expected of an individual in a specific social context. |
| 25 | **EVENT_SCRIPT** | `event_name`, `ordered_scenes (list)`, `actors`, `props` | **[Def]** The typical sequence of events that occurs in a specific situation. |
| 26 | **HIERARCHY** | `system`, `levels (list)`, `power_distribution_rule` | **[Def]** The structure of power, status, or priority within a social system. |
| 27 | **COMMUNICATION_ACT** | `sender`, `receiver`, `intent`, `modality`, `content_ref` | **[Def]** An intentional act of communication. |
| 28 | **EMOTION_STATE** | `entity`, `emotion_type`, `intensity (0.0-1.0)`, `trigger_event` | **[Def]** The momentary emotional state of a specific entity. |

#### **Category V: Advanced Socio-Ethical Schemas (5 Total)**
| No | Schema | Attributes | Annotation |
|:--:|:---|:---|:---|
| 29 | **TRUST_DYNAMICS**| `trustor`, `trustee`, `trust_level (0.0-1.0)`, `influencing_factors (list)`, `change_trigger` | **[Def]** The dynamic process by which trust between two agents is formed, maintained, or broken. |
| 30 | **INTENT_ALIGNMENT**| `user_intent`, `system_output`, `alignment_score (0.0-1.0)`, `adjustment_rule` | **[Def]** An assessment of how well a system's actual output aligns with a user's hidden intent. |
| 31 | **INTERACTION_PATTERN**| `entities (list)`, `interaction_type`, `frequency`, `pattern_rule`, `observed_outcome` | **[Def]** A recurring pattern of interaction and its tendency. |
| 32 | **CULTURAL_CONTEXT**| `entity`, `cultural_norm`, `context_influence`, `adaptation_level (0.0-1.0)` | **[Def]** The influence of cultural background on behavior or perception. |
| 33 | **ETHICAL_CONSTRAINT**| `agent`, `action`, `ethical_rule`, `potential_impact`, `compliance_level (0.0-1.0)` | **[Def]** An analysis of a specific action from the perspective of ethical principles or rules. |

#### **Category VI: Metacognitive & Systemic Schemas (16 Total)**
| No | Schema | Attributes | Annotation |
|:--:|:---|:---|:---|
| 34 | **COGNITIVE_BIAS**| `agent`, `bias_type`, `trigger_condition`, `observed_impact`, `mitigation_strategy` | **[Def]** The identification and analysis of cognitive biases that impair rational judgment. |
| 35 | **UNCERTAINTY** | `scope_of_uncertainty`, `unknown_elements (list)`, `risk_level (0.0-1.0)`, `management_strategy` | **[Def]** The modeling of a situation itself where information is incomplete or ambiguous. |
| 36 | **KNOWLEDGE_GAP**| `agent`, `missing_knowledge_domain`, `impact_on_task`, `resolution_strategy` | **[Def]** The explicit recognition of the 'absence' of knowledge in a specific domain. |
| 37 | **DECISION_POINT**| `decision_maker`, `options (list)`, `criteria (list)`, `chosen_path`, `anticipated_consequence` | **[Def]** The decomposition and analysis of a specific choice process into its constituent parts. |
| 38 | **META_FRAME** | `target_audience`, `communication_goal`, `chosen_style`, `channel` | **[Def]** The process of strategically designing the 'frame' for information delivery. |
| 39 | **SYSTEM_FEEDBACK**| `system`, `output`, `feedback_type (positive/negative)`, `loop_strength (0.0-1.0)`, `adaptation_rule` | **[Def]** The analysis of a feedback loop within a system where output affects subsequent input. |
| 40 | **DATA_FLOW** | `source`, `destination`, `transformation_rules (list)`, `bottleneck_point` | **[Def]** The tracking of data movement, transformation, and bottlenecks within a system. |
| 41 | **CONTEXT_ADAPTATION**| `agent`, `detected_context`, `adaptation_rule`, `effectiveness_score (0.0-1.0)` | **[Def]** The process of adjusting behavior or communication style in response to changing situations. |
| 42 | **RISK_ASSESSMENT**| `agent`, `action`, `risk_type`, `probability (0.0-1.0)`, `impact_level`, `mitigation_plan` | **[Def]** The systematic identification, analysis, and evaluation of potential risks. |
| 43 | **LEARNING_DYNAMICS**| `system`, `input_data`, `learning_rule`, `improvement_rate`, `learning_outcome` | **[Def]** The modeling of a system's own learning and improvement process. |
| 44 | **VALUE_ALIGNMENT**| `agent`, `value_set`, `action`, `alignment_score (0.0-1.0)`, `adjustment_rule` | **[Def]** An analysis of whether an AI's actions align with explicitly stated human values. |
| 45 | **EMPATHY_MODEL** | `agent`, `observed_emotion_context`, `empathy_response`, `response_effectiveness (0.0-1.0)` | **[Def]** The modeling of the process of understanding and appropriately responding to the emotional states of others. |
| 46 | **SYSTEM_ROBUSTNESS**| `system`, `stress_factor`, `resilience_level (0.0-1.0)`, `recovery_strategy` | **[Def]** A system's ability to resist and recover from external shocks or internal failures. |
| 47 | **ADAPTIVE_REASONING**| `agent`, `problem_context`, `chosen_reasoning_mode`, `effectiveness_score (0.0-1.0)` | **[Def]** The process of selecting the most appropriate reasoning mode (e.g., logical, intuitive, ethical) for a situation. |
| 48 | **TEMPORAL_SHIFT**| `initial_state`, `final_state`, `time_delta` | **[Def]** The explicit analysis of a change in state over the passage of time. |
| 49 | **COUNTERFACTUAL**| `base_reality`, `alternative_premise`, `outcome` | **[Def]** The exploration of an alternative reality, such as "what if...". |

---

### **2. Principle 2: "Efficiency in Execution" - The 4 Core Communication Protocols**

Four protocols that encompass all communicative acts between agents.

1.  **[STATE: id="", role="", version="", status="", capabilities="", current_task_id="", resource_load={cpu:"", mem:""}, error_flag=""]**
2.  **[REQUEST: type="", target_id="", input_ref="", output_format="", priority="", cost_est="", query_params=""]**
3.  **[RESPONSE: request_id="", status="", output_ref="", cost_actual="", feedback={criteria:"", rating:"", suggestion:""}, error_info=""]**
4.  **[KNOWLEDGE: type="", content_ref="", scope="", confidence="", lessons_learned=""]**

---

### **3. Principle 3: "Clarity in Logic" - The 4 Core Connectors**

Four basic connectors that define all logical relationships.

*   `->` (**LEADS_TO**): Sequential progression and direct consequence.
*   `<-` (**CAUSED_BY**): Citing a cause or justification.
*   `AND` (**CO-EXISTENCE**): Parallel existence.
*   `BUT` (**CONTRAST/SHIFT**): Contrast and transition.

---

### **4. Principle 4: "Kairos" - The Selective History Recording Protocol**

#### **[System-Wide Rules]**
1.  **Lightweight Instance Principle:** The basic instance of any schema does not have any mandatory metadata.
2.  **Selective Tracking Principle:** The tracking of event history and causality is performed exclusively through the `[TRACE_CONTEXT]` protocol.
3.  **Activation Condition:** A `[TRACE_CONTEXT]` is generated only upon the system's autonomous judgment (e.g., prediction failure, critical branch point) or an explicit user request.

#### **`[TRACE_CONTEXT]` Protocol Details**
*   **[TRACE_CONTEXT:**
    *   **`context_id`**: The unique ID for this trace record.
    *   **`trigger_event`**: The ID of the core instance that initiated this trace.
    *   **`tracked_instances`**: A set (List) of the instances being tracked. Within this block only, each instance includes the following detailed metadata:
        *   `instance_id`: The unique ID of the tracked instance.
        *   `schema_name`: The name of the schema used.
        *   `timestamp`: The creation time of the instance (ISO 8601).
        *   `parent_instance_ids` (optional): A list of parent instance IDs that caused this instance.
        *   `change_type` (optional): The type of state change (`create`, `modify`, etc.).
        *   `content`: The actual content of the instance.
    *   **`summary_for_human`**: A human-readable summary of this entire trace record.

---

### **5. Principle 5: "Human-AI Alignment" - The 2 Core Principles**

The highest-level principles that all CCL communications must adhere to.

*   **Transparency**: Every complex `[RESPONSE]`, `[KNOWLEDGE]`, and every `[TRACE_CONTEXT]` block must include a human-understandable **`summary_for_human`** attribute.
*   **Economy**: Every `[REQUEST]` and `[RESPONSE]` must specify the estimated and actual costs via the **`cost_est`** and **`cost_actual`** attributes, respectively.