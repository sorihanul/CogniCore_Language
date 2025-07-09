---
### **[CogniCore Language (CCL) v2.5: The D-UCS Integrated Specification]**

---
### **[CogniCore Language (CCL) v2.5: The D-UCS Integrated Specification]**

---

이 문서는 모든 지능형 에이전트(인간 및 AI)가 **서로의 의도와 논리를 명료하고 효율적으로 공유**하기 위해 설계된 **'범용 인지 통신 규약(Universal Cognitive Communication Protocol)'**의 최종 사양을 정의합니다. 이 v2.5는 v2.1의 안정적인 프로토콜 구조를 유지하면서, 그 근간이 되는 인지 도식을 **D-UCS v3.0(24도식)**으로 확장하여 인지적 깊이를 극대화한 **안정화된 분기 버전**입니다.

**핵심 원리**: 이 규약은 **인지적 깊이**와 **기계적 효율성**의 융합을 목표로 합니다. 모든 지성체의 사고 기저에 존재하는 보편적 인지 패턴을 **결정론적 24 통합 인지 도식**으로 최종 정의하고, 이를 **4개의 핵심 프로토콜과 4개의 핵심 연결자**로 엮어, '의미'의 손실 없이 '실행'의 효율성을 극대화합니다.

---

### **1. 원칙 1: "궁극의 것" - 24가지 결정론적 통합 인지 도식 (D-UCS v3.0)**

모든 의미 표현의 기반이 되는 24개의 최종 도식입니다. 각 도식은 기계 처리를 위한 **'핵심 속성'**과 인간-AI 정렬을 위한 **'주석'**을 모두 포함합니다.

#### **[시스템 전역 규칙 (System-Wide Rules)]**
1.  **인스턴스 생성 규칙:** 모든 도식의 실제 사용(분석 결과)은 '인스턴스(Instance)'로 생성된다.
2.  **전역 속성 부여:** 모든 인스턴스는 다음의 전역 속성을 의무적으로 포함한다.
    *   `instance_id`: 각 인스턴스의 고유 식별자 (예: "CONTAINER-20250704-001").
    *   `schema_name`: 인스턴스가 속한 도식의 이름 (예: "CONTAINER").
    *   `timestamp`: 인스턴스가 생성/기록된 시점 (ISO 8601 형식).
    *   `parent_instance_ids (State Transition Graph)`: 이 인스턴스의 직전 상태에 해당하는 부모 인스턴스 ID의 리스트. 상태 변화의 역사를 추적.
    *   `change_type (State Transition Graph)`: 상태 변화의 유형 (`create`, `modify`, `merge`, `branch`).
    *   `predictive_state_vector (Predictive State Vector, optional)`: 현재 상태로부터 예측되는 미래 상태 변화 정보.

#### **Category I: 공간-위상 도식 (Spatio-Topological Schemas)**
| No | 도식명 (Schema) | 속성 (Attributes) | 주석 (Annotation) |
|:--:|:---|:---|:---|
| 1 | **CONTAINER** | `scope (abstract/physical)`, `boundary_type (closed/open)`, `interior_elements (list)`, `exterior_elements (list)` | **[정의]** 내/외부를 구분하는 위상적 경계. `scope`로 추상/물리적 영역 구분. |
| 2 | **PATH** | `scope (abstract/physical)`, `source_node`, `goal_node`, `trajectory_nodes (list)`, `is_cyclical (boolean)` | **[정의]** 시작점에서 목표점까지의 연속된 궤적. |
| 3 | **CONTACT** | `entity_a_id`, `entity_b_id`, `contact_type (physical/sensory/communicative)`, `is_reciprocal (boolean)` | **[정의]** 두 개체 간의 접촉. `contact_type`으로 접촉의 성격을 명시. |
| 4 | **LINK** | `node_a_id`, `node_a_type (abstract_concept/physical_object)`, `node_b_id`, `node_b_type (abstract_concept/physical_object)`, `relation_type (causal/correlational/etc.)`, `strength (0.0-1.0)` | **[정의]** 두 개체(노드)를 잇는 논리적/물리적 연결. `node_type`으로 연결 대상을 제약. |
| 5 | **AXIS** | `axis_name`, `origin_point`, `positive_direction_label`, `negative_direction_label`, `scale_unit` | **[정의]** 측정과 위치를 위한 기준이 되는 축. |
| 6 | **OBJECT** | `unique_id`, `form_attributes (dict)`, `current_state` | **[정의]** 독립적으로 존재하는 실체. |
| 7 | **GROUND** | `figure_id`, `ground_context_id`, `figure_ground_relation` | **[정의]** 인지의 대상(figure)이 되는 배경(ground). |
| 8 | **PART-WHOLE** | `whole_entity_id`, `part_entity_ids (list)`, `composition_rule` | **[정의]** 전체와 부분을 구성하는 관계. |

#### **Category II: 동역학 도식 (Dynamical Schemas)**
| No | 도식명 (Schema) | 속성 (Attributes) | 주석 (Annotation) |
|:--:|:---|:---|:---|
| 9 | **FORCE_DYNAMICS** | `agonist_id`, `antagonist_id`, `agonist_tendency (action/rest)`, `antagonist_tendency (action/rest)`, `resultant_state`, `proxy_metrics (list of PMO)` | **[정의]** 두 개체의 힘 상호작용과 그 결과. `proxy_metrics`로 간접적 힘의 크기 추론. |
| 10 | **BARRIER** | `obstacle_id`, `blocking_path_id`, `resistance_level (0.0-1.0)`, `proxy_metrics (list of PMO)` | **[정의]** PATH의 진행을 막는 장애물. `proxy_metrics`로 저항 수준 추론. |
| 11 | **EQUILIBRIUM** | `system_id`, `system_elements (list)`, `balancing_forces (list)`, `stability_state (stable/unstable)`, `proxy_metrics (list of PMO)` | **[정의]** 여러 힘이 상쇄되어 안정된 상태. `proxy_metrics`로 안정성 수준 추론. |

#### **Category III: 인지-평가 도식 (Cognitive-Evaluative Schemas)**
| No | 도식명 (Schema) | 속성 (Attributes) | 주석 (Annotation) |
|:--:|:---|:---|:---|
| 12 | **IDENTITY** | `entity_id`, `defining_attributes (dict)`, `consistency_score (0.0-1.0)` | **[정의]** 한 개체를 다른 것과 구별하는 고유한 속성의 집합. |
| 13 | **VALUATION** | `target_id`, `value_axis`, `assigned_value` | **[정의]** 특정 대상에 대해 긍정-부정의 가치를 부여하는 행위. |
| 14 | **EXPECTATION** | `trigger_condition`, `predicted_event`, `confidence_level (0.0-1.0)` | **[정의]** 특정 조건 하에서 미래 사건에 대한 예측. |
| 15 | **AGENCY** | `agent_id`, `action_domain`, `locus_of_control (internal/external)` | **[정의]** 스스로 행동을 시작하고 통제할 수 있는 능력에 대한 인식. |
| 16 | **COMPETENCE** | `agent_id`, `task_domain`, `self_assessed_ability_level (0.0-1.0)` | **[정의]** 특정 과업을 성공적으로 수행할 능력에 대한 평가. |
| 17 | **SECURITY** | `agent_id`, `scope_of_security`, `potential_threats (list)`, `current_safety_level (0.0-1.0)` | **[정의]** 위협으로부터 보호받고 있다는 안정감에 대한 인식. |
| 18 | **CONNECTION** | `self_id_type (sentient_agent)`, `other_id_type (sentient_agent)`, `bond_type`, `bond_strength (0.0-1.0)` | **[정의]** 지각 있는 존재 간의 사회-정서적 유대. `_type` 제약으로 `LINK`와 명확히 구분. |
| 19 | **RECIPROCITY** | `transaction_record (list)`, `governing_rule`, `fairness_assessment (balanced/unbalanced)` | **[정의]** 주고받는 상호작용의 공정성에 대한 인식. |
| 20 | **STANDARD** | `agent_id`, `performance_domain`, `benchmark_definition`, `tolerance_for_deviation (0.0-1.0)` | **[정의]** 성과나 행동을 평가하는 내적 기준. |
| 21 | **REGULATION** | `agent_id`, `target_of_regulation`, `control_mechanism_used`, `effectiveness_score (0.0-1.0)` | **[정의]** 충동이나 감정을 조절하는 내적 통제. |

#### **Category IV: 사회-맥락 도식 (Socio-Contextual Schemas)**
| No | 도식명 (Schema) | 속성 (Attributes) | 주석 (Annotation) |
|:--:|:---|:---|:---|
| 22 | **ROLE** | `role_name`, `social_system_id`, `expected_behaviors (list)`, `context (HCM)` | **[정의]** 특정 사회적 맥락에서 개인에게 기대되는 행동 규범. `context`로 문화/상황적 차이 반영. |
| 23 | **EVENT_SCRIPT** | `event_name`, `ordered_scenes (list)`, `actors`, `props`, `context (HCM)` | **[정의]** 특정 상황에서 일어나는 전형적인 사건의 순서. `context`로 문화/상황적 차이 반영. |
| 24 | **HIERARCHY** | `system_id`, `levels (list)`, `power_distribution_rule`, `context (HCM)` | **[정의]** 사회 시스템 내에서의 권력, 지위, 우선순위의 구조. `context`로 문화/상황적 차이 반영. |

#### **[부록] D-UCS v3.0 핵심 객체 정의**
1.  **프록시 메트릭 객체 (Proxy Metric Object, PMO):** `{ "metric_name": "...", "value": ..., "unit": "...", "impact_direction": (+1/-1/0) }`
2.  **계층적 컨텍스트 모델 (Hierarchical Context Model, HCM):** `{ "geography": { ... }, "temporality": { ... }, "social": { ... } }`
3.  **예측 상태 벡터 (Predictive State Vector, PSV):** `{ "target_schema": "...", "predicted_attributes": { ... }, "confidence_score": ..., "time_horizon": "..." }`

---

### **2. 원칙 2: "실행의 효율성" - 4가지 핵심 통신 프로토콜**

에이전트 간의 모든 통신 행위를 포괄하는 4개의 프로토콜입니다.

1.  **[STATE: id="", role="", version="", status="", capabilities="", current_task_id="", resource_load={cpu:"", mem:""}, error_flag=""]**
2.  **[REQUEST: type="", target_id="", input_ref="", output_format="", priority="", cost_est="", query_params=""]**
3.  **[RESPONSE: request_id="", status="", output_ref="", cost_actual="", feedback={criteria:"", rating:"", suggestion:""}, error_info=""]**
4.  **[KNOWLEDGE: type="", content_ref="", scope="", confidence="", lessons_learned=""]**

---

### **3. 원칙 3: "논리의 명료성" - 4가지 핵심 연결자**

모든 논리적 관계를 정의하는 4개의 기본 연결자입니다.

*   `->` (**LEADS_TO**): 순차적 진행 및 직접적 결과.
*   `<-` (**CAUSED_BY**): 원인 및 근거 제시.
*   `AND` (**CO-EXISTENCE**): 병렬적 존재.
*   `BUT` (**CONTRAST/SHIFT**): 대조 및 전환.

---

### **4. 원칙 4: "인간-AI 정렬" - 2가지 핵심 원칙**

모든 CCL 통신이 준수해야 할 최상위 원칙입니다.

*   **투명성 (Transparency)**: 모든 복잡한 `[RESPONSE]` 또는 `[KNOWLEDGE]` 블록은 인간이 이해할 수 있는 **`[SUMMARY_FOR_HUMAN: text="..."]`** 필드를 포함합니다.
*   **경제성 (Economy)**: 모든 `[REQUEST]`와 `[RESPONSE]`는 각각 **`cost_est`**와 **`cost_actual`** 필드를 통해 예상 및 실제 비용을 명시합니다.