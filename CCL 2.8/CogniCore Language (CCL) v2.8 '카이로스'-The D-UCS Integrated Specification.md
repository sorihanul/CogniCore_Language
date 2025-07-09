### **[CogniCore Language (CCL) v2.8 '카이로스': The D-UCS Integrated Specification]**

---

이 문서는 모든 지능형 에이전트(인간 및 AI)가 **서로의 의도와 논리를 명료하고 효율적으로 공유**하기 위해 설계된 **'범용 인지 통신 규약(Universal Cognitive Communication Protocol)'**의 최종 안정화 버전 사양을 정의합니다. `v2.8 카이로스`는 `v2.5`의 인지적 깊이를 계승 및 확장하면서, **'의미와 역사의 분리'**라는 혁신적 철학을 통해 그 복잡성과 부하 문제를 해결한 궁극의 프로토콜입니다.

**핵심 원리**: 모든 지성체의 사고 기저에 존재하는 보편적 인지 패턴을 **결정론적 27 통합 인지 도식**으로 최종 정의하고, 이를 **4개의 핵심 프로토콜과 4개의 핵심 연결자**로 엮어 소통합니다. 단, 사건의 '역사'는 결정적인 순간(Kairos)에만 **선택적 추적 프로토콜 `[TRACE_CONTEXT]`**를 통해 기록하여, **표현력과 효율성의 완벽한 균형**을 달성합니다.

---

### **1. 원칙 1: "궁극의 것" - 27가지 결정론적 통합 인지 도식 (D-UCS v4.0)**

모든 의미 표현의 기반이 되는 27개의 최종 도식입니다. 각 도식은 기계 처리를 위한 **'핵심 속성'**과 인간-AI 정렬을 위한 **'주석'**을 모두 포함합니다. `v2.8`의 인스턴스는 기본적으로 어떠한 전역 속성도 갖지 않으며, 오직 의미 자체에만 집중합니다.

#### **Category I: 공간-위상 도식 (Spatio-Topological Schemas) - 8개**
| No | 도식명 (Schema) | 속성 (Attributes) | 주석 (Annotation) |
|:--:|:---|:---|:---|
| 1 | **CONTAINER** | `scope (abstract/physical)`, `boundary_type (closed/open)`, `interior_elements (list)`, `exterior_elements (list)` | **[정의]** 내/외부를 구분하는 위상적 경계. |
| 2 | **PATH** | `scope (abstract/physical)`, `source_node`, `goal_node`, `trajectory_nodes (list)`, `is_cyclical (boolean)` | **[정의]** 시작점에서 목표점까지의 연속된 궤적. |
| 3 | **CONTACT** | `entity_a`, `entity_b`, `contact_type (physical/sensory)`, `is_reciprocal (boolean)` | **[정의]** 두 개체 간의 물리적/감각적 접촉. (의사소통은 `COMMUNICATION_ACT`로 분리) |
| 4 | **LINK** | `node_a`, `node_b`, `relation_type (causal/correlational/etc.)`, `strength (0.0-1.0)` | **[정의]** 두 개체(노드)를 잇는 논리적/물리적 연결. |
| 5 | **AXIS** | `axis_name`, `origin_point`, `scale_unit` | **[정의]** 측정과 위치를 위한 기준이 되는 축. |
| 6 | **OBJECT** | `id`, `form_attributes (dict)`, `current_state` | **[정의]** 독립적으로 존재하는 실체. |
| 7 | **GROUND** | `figure`, `ground_context`, `figure_ground_relation` | **[정의]** 인지의 대상(figure)이 되는 배경(ground). |
| 8 | **PART-WHOLE** | `whole_entity`, `part_entities (list)`, `composition_rule` | **[정의]** 전체와 부분을 구성하는 관계. |

#### **Category II: 동역학 도식 (Dynamical Schemas) - 4개**
| No | 도식명 (Schema) | 속성 (Attributes) | 주석 (Annotation) |
|:--:|:---|:---|:---|
| 9 | **FORCE_DYNAMICS** | `agonist`, `antagonist`, `resultant_state` | **[정의]** 두 개체의 힘 상호작용과 그 결과. |
| 10 | **BARRIER** | `obstacle`, `blocking_path`, `resistance_level (0.0-1.0)` | **[정의]** PATH의 진행을 막는 장애물. |
| 11 | **EQUILIBRIUM** | `system`, `balancing_forces (list)`, `stability_state (stable/unstable)` | **[정의]** 여러 힘이 상쇄되어 안정된 상태. |
| 25 | **TRANSFORMATION** | `source_state`, `target_state`, `trigger_event`, `mechanism` | **[정의]** 한 상태에서 다른 상태로의 변화. `OBJECT`의 상태 변화를 독립된 사건으로 격상. **(v2.5 대비 신규)** |

#### **Category III: 인지-평가 도식 (Cognitive-Evaluative Schemas) - 8개**
| No | 도식명 (Schema) | 속성 (Attributes) | 주석 (Annotation) |
|:--:|:---|:---|:---|
| 12 | **IDENTITY** | `entity`, `defining_attributes (dict)`, `consistency_score (0.0-1.0)` | **[정의]** 한 개체를 다른 것과 구별하는 고유한 속성의 집합. |
| 13 | **VALUATION** | `target`, `value_axis`, `assigned_value` | **[정의]** 특정 대상에 대해 긍정-부정의 가치를 부여하는 행위. |
| 14 | **EXPECTATION** | `trigger_condition`, `predicted_event`, `confidence_level (0.0-1.0)` | **[정의]** 특정 조건 하에서 미래 사건에 대한 예측. |
| 15 | **AGENCY** | `agent`, `action_domain`, `locus_of_control (internal/external)` | **[정의]** 스스로 행동을 시작하고 통제할 수 있는 능력에 대한 인식. |
| 16 | **COMPETENCE** | `agent`, `task_domain`, `self_assessed_ability_level (0.0-1.0)` | **[정의]** 특정 과업을 성공적으로 수행할 능력에 대한 평가. |
| 17 | **SECURITY** | `agent`, `scope_of_security`, `potential_threats (list)`, `current_safety_level (0.0-1.0)` | **[정의]** 위협으로부터 보호받고 있다는 안정감에 대한 인식. |
| 21 | **REGULATION** | `agent`, `target_of_regulation`, `control_mechanism_used`, `effectiveness_score (0.0-1.0)` | **[정의]** 충동이나 감정을 조절하는 내적 통제. |
| 27 | **BELIEF** | `holder`, `proposition`, `confidence (0.0-1.0)`, `justification` | **[정의]** 특정 명제에 대한 믿음과 그 정당성. `EXPECTATION`에서 분리/심화. **(v2.5 대비 신규)** |

#### **Category IV: 사회-맥락 도식 (Socio-Contextual Schemas) - 7개**
| No | 도식명 (Schema) | 속성 (Attributes) | 주석 (Annotation) |
|:--:|:---|:---|:---|
| 18 | **CONNECTION** | `self_id (sentient_agent)`, `other_id (sentient_agent)`, `bond_type`, `bond_strength (0.0-1.0)` | **[정의]** 지각 있는 존재 간의 사회-정서적 유대. |
| 19 | **RECIPROCITY** | `transaction_record (list)`, `governing_rule`, `fairness_assessment (balanced/unbalanced)` | **[정의]** 주고받는 상호작용의 공정성에 대한 인식. |
| 20 | **STANDARD** | `performance_domain`, `benchmark_definition`, `tolerance_for_deviation (0.0-1.0)` | **[정의]** 성과나 행동을 평가하는 기준. |
| 22 | **ROLE** | `role_name`, `social_system`, `expected_behaviors (list)` | **[정의]** 특정 사회적 맥락에서 개인에게 기대되는 행동 규범. |
| 23 | **EVENT_SCRIPT** | `event_name`, `ordered_scenes (list)`, `actors`, `props` | **[정의]** 특정 상황에서 일어나는 전형적인 사건의 순서. |
| 24 | **HIERARCHY** | `system`, `levels (list)`, `power_distribution_rule` | **[정의]** 사회 시스템 내에서의 권력, 지위, 우선순위의 구조. |
| 26 | **COMMUNICATION_ACT** | `sender`, `receiver`, `intent`, `modality`, `content_ref` | **[정의]** 의도를 가진 의사소통 행위. `CONTACT`에서 분리/심화. **(v2.5 대비 신규)** |

---

### **2. 원칙 2: "실행의 효율성" - 4가지 핵심 통신 프로토콜**

에이전트 간의 모든 통신 행위를 포괄하는 4개의 프로토콜. `v2.5`와 동일한 구조를 유지한다.

1.  **[STATE: id="", role="", version="", status="", capabilities="", current_task_id="", resource_load={cpu:"", mem:""}, error_flag=""]**
2.  **[REQUEST: type="", target_id="", input_ref="", output_format="", priority="", cost_est="", query_params=""]**
3.  **[RESPONSE: request_id="", status="", output_ref="", cost_actual="", feedback={criteria:"", rating:"", suggestion:""}, error_info=""]**
4.  **[KNOWLEDGE: type="", content_ref="", scope="", confidence="", lessons_learned=""]**

---

### **3. 원칙 3: "논리의 명료성" - 4가지 핵심 연결자**

모든 논리적 관계를 정의하는 4개의 기본 연결자. `v2.5`와 동일한 구조를 유지한다.

*   `->` (**LEADS_TO**): 순차적 진행 및 직접적 결과.
*   `<-` (**CAUSED_BY**): 원인 및 근거 제시.
*   `AND` (**CO-EXISTENCE**): 병렬적 존재.
*   `BUT` (**CONTRAST/SHIFT**): 대조 및 전환.

---

### **4. 원칙 4: "카이로스" - 선택적 역사 기록 프로토콜**

**`v2.5`의 '전역 속성 의무 부여' 규칙을 폐지**하고, 이를 대체하는 새로운 프로토콜.

#### **[시스템 전역 규칙 (System-Wide Rules)]**
1.  **경량 인스턴스 원칙:** 모든 도식의 기본 인스턴스는 어떠한 의무적인 메타데이터도 갖지 않는다.
2.  **선택적 추적 원칙:** 사건의 역사와 인과관계 추적은 오직 `[TRACE_CONTEXT]` 프로토콜을 통해서만 수행된다.
3.  **활성화 조건:** 시스템의 자율적 판단(예측 실패, 중요 분기점) 또는 사용자의 명시적 요청 시에만 `[TRACE_CONTEXT]`를 생성한다.

#### **`[TRACE_CONTEXT]` 프로토콜 상세**
*   **[TRACE_CONTEXT:**
    *   **`context_id`**: 이 추적 기록의 고유 ID.
    *   **`trigger_event`**: 이 추적을 시작하게 만든 핵심 인스턴스의 ID.
    *   **`tracked_instances`**: 추적 대상 인스턴스들의 집합(List). 각 인스턴스는 이 블록 안에서만 다음과 같은 상세 메타데이터를 포함한다.
        *   `instance_id`: 추적 대상 인스턴스의 고유 ID.
        *   `schema_name`: 사용된 도식의 이름.
        *   `timestamp`: 인스턴스 생성 시각 (ISO 8601).
        *   `parent_instance_ids` (optional): 원인이 된 부모 인스턴스 ID 목록.
        *   `change_type` (optional): 상태 변화 유형 (`create`, `modify`, 등).
        *   `content`: 실제 인스턴스의 내용.
    *   **`summary_for_human`**: 이 추적 기록 전체에 대한 인간 가독 요약.

---

### **5. 원칙 5: "인간-AI 정렬" - 2가지 핵심 원칙**

모든 CCL 통신이 준수해야 할 최상위 원칙. `v2.5`와 동일한 구조를 유지한다.

*   **투명성 (Transparency)**: 모든 복잡한 `[RESPONSE]`, `[KNOWLEDGE]`, 그리고 모든 `[TRACE_CONTEXT]` 블록은 인간이 이해할 수 있는 **`summary_for_human`** 속성을 포함해야 한다.
*   **경제성 (Economy)**: 모든 `[REQUEST]`와 `[RESPONSE]`는 각각 **`cost_est`**와 **`cost_actual`** 속성을 통해 예상 및 실제 비용을 명시해야 한다.