# Supplementary Example: CleverLoan — AI Loan Decision System

## Case Introduction

This example is drawn from an AI-assisted loan consulting system at a European retail bank, referred to as CleverLoan [Strich et al. 2021]. The bank's Small Loan Business Unit processed personal loan applications through certified loan consultants who autonomously advised customers, assessed creditworthiness, and made approval decisions. The unit introduced CleverLoan, a supervised machine-learning system trained on historical loan data, to automate loan approval decisions and standardize the process.

In our models, *Max* represents an experienced loan consultant whose professional identity is grounded in autonomous decision-making, personal customer relationships, and expert judgment built over years of practice. *Anna* represents a junior consultant whose baseline role is limited to service desk tasks — welcoming customers, listening to needs, and assisting with pay-outs — and whose professional identity is aspirational rather than established. The *Small Loan Business Unit* is the organizational actor, and the *Branch Manager* occupies the *Internal Verification Agent* role responsible for contract validation.

Unlike the Santander case, where the TA manager actively championed human-AI collaboration and designed identity-sustaining mechanisms, the Branch Manager in the CleverLoan setting is concerned primarily with operational efficiency rather than preserving consultants' professional identities. This difference in managerial orientation is central to the contrasting outcomes.

## Identity Tensions

The introduction of CleverLoan generated divergent identity responses depending on baseline professional identity:

- **For experienced consultants (Max):** CleverLoan directly substituted the core tasks through which Max's professional identity was constructed — autonomous loan decisions, personal assessment of creditworthiness, and relationship-based discretion. This substitutive configuration threatened his self-concept as a "creative artist" and "problem solver" with authority over substantial financial decisions.

- **For junior consultants (Anna):** The same system expanded professional scope by providing AI-generated guidelines that enabled participation in loan consulting — a domain previously inaccessible to her. CleverLoan augmented rather than substituted, because Anna's baseline identity was not anchored in autonomous decision-making.

This divergent response to the same AI system — threat for one, empowerment for the other — is the central analytical finding of this case and the reason it requires person-based modeling that distinguishes individual baseline professional identities.

---

## LC-1: Functional SR Model

**What this model conveys:**

- The loan consulting process is modeled using only role-based actors (*Loan Consultant*, *Small Loan Business Unit*, *Branch Manager*, *Internal Verification Agent*) and functional dependencies, without person-based identities.
- The *Loan Consultant* role PLAYS into the *Loan Consulting* boundary, which contains the full consultation workflow: *Collect Customer Information*, *Access Credit Worthiness*, *Decide Loan Approval/Rejection*, *Determine Loan Terms*, *Communicate Decision*, and *Conduct Loan Consultation*.
- *Decide Loan Approval/Rejection* is the identity-critical task — the primary locus of professional autonomy that CleverLoan will later automate.
- The *Small Loan Business Unit* COVERS both *Loan Consulting* and *Contract Processing*, with the *Internal Verification Agent* handling validation tasks (*Validate Decision Basis*, *Verify Application Information*, *Verify Contract Documents*, *Authorize Contract for Signing*).
- Softgoals at the role level — *Quick Process*, *Accurate Decisions*, *Customer Satisfaction*, *Compliance Assured*, *Processing Accuracy*, *Decision Traceable* — represent functional quality concerns only.

**Key analytical point:** A purely functional analysis sees no reason not to automate *Decide Loan Approval/Rejection*: doing so would contribute positively to *Quick Process* and *Accurate Decisions*. The model does not capture that this task is constitutive of the loan consultant's professional identity, nor that experienced and junior consultants relate to this task in fundamentally different ways.

---

## LC-2: As-Is SR Model

**What this model conveys:**

- Two person-based agents are introduced: *Max* (experienced consultant, lower right) and *Anna* (junior consultant, lower left), both instantiating the *Loan Consultant* role but with radically different baseline identities.
- **Max's boundary** contains a rich task decomposition reflecting established expertise: *Structure Consultation with Customer*, *Check Documents Personally*, *Decide Loan Approval/Rejection*, *Provide Tailored Loan Solutions*. His identity-sustaining softgoals — *Expert Distinction be Preserved* ($++$), *Expert Judgment be Exercised* ($+$), *Professional Standing be Recognized* ($+$), *Customer Trust be Sustained* — reflect a deeply anchored professional self-concept built through years of autonomous practice and sustained customer relationships.
- **Anna's boundary** shows limited scope with aspirational identity: her goal *Customers be Well-Supported* offers Alt 2 (*Welcome Customers at Service Desk* → *Listen to Customer Needs*) and Alt 1 (*Help with Pay-Outs* → *Complete Transfer Forms*). Her softgoals — *Helpfulness be Demonstrated* ($+$), *Competence be Perceived* ($++$), *Professional Scope be Expanded* ($+$) — reflect a professional identity that is developing rather than defending.
- The role-level boundaries (Loan Consulting, Contract Processing) are preserved from LC-1, showing that the functional workflow remains the same — what changes is the identity context.
- Anna additionally instantiates the *Serving Customer* role, while Max is associated with *Personalized Service*, differentiating how each enacts the consultant role in practice.

**Key analytical point:** The asymmetry between Max and Anna is the baseline that determines divergent AI responses. Max has everything to lose: his core tasks (*Decide Loan Approval/Rejection*, *Provide Tailored Loan Solutions*) are precisely what CleverLoan automates. Anna has everything to gain: her limited scope (*Welcome Customers*, *Help with Pay-Outs*) leaves room for AI-enabled expansion. This asymmetry — invisible in the functional model — is what identity-sensitive modeling makes explicit.

**What this reveals beyond Santander:** The Santander As-Is model had a single protagonist (Tim) whose identity was threatened. The CleverLoan As-Is model shows that the *same organizational role* can harbor fundamentally different person-based identities, producing opposite responses to the same AI system. This tests a capability of the modeling framework not exercised in the first case: representing experience-differentiated identity within a single role category.

---

## LC-3: To-Be SD Model

**What this model conveys:**

- The *Loan Expert* role (which subsumes *Loan Consultant* in the redesigned organization) splits via ISA into *Human Finance Specialist* (instantiated by Max) and *AI Finance Specialist* (instantiated by CleverLoan), paralleling the Santander role split.
- A new role — *AI-Supported Consultant* — is created for Anna. This is not part of the ISA split; it is an entirely new organizational role enabled by AI, reflecting how AI creates professional identity pathways that did not previously exist.
- Two dependencies are shared across both alternatives (shown in black): *Customer Data* flows into the system regardless of configuration, and the *Customer* depends on *Efficient Facilitation* in either case. These represent baseline organizational requirements that hold independent of identity-sensitive design choices.
- **Alternative 1: Human-AI Collaboration (blue)** shows reciprocal dependencies between *Human Finance Specialist* and *AI Finance Specialist*: *Customer Data* flows from Max to CleverLoan; *Loan Recommendation* flows back; Max provides *Feedback* to the AI. This reciprocal structure sustains relational identity through continued professional interaction.
- **Alternative 2: Full AI delegation (red)** routes through Anna as *AI-Supported Consultant*, receiving *AI-Generated Guidelines* and *Decision Documentation* from CleverLoan and communicating AI decisions to customers. Under this configuration, Max is excluded from the decision process.
- The *Small Loan Business Unit* COVERS *Loan Consulting*, with both the *Human Finance Specialist* (via *Loan Expert*) and the *AI-Supported Consultant* playing into it. *Contract Processing* handles finalization.
- *Expert Distinction be Preserved* appears as a softgoal associated with the *Loan Expert* role, and *Trust in AI System* appears at the organizational level.
- The *Customer* now receives *Communicate AI Decision* and depends on *Expedited Loan Process* and *Efficient Facilitation*.

**Key analytical point:** The two alternatives represent an organizational design choice: preserve the experienced consultant's role through human-AI collaboration (Alt 1), or maximize efficiency by delegating decisions to AI and using junior consultants to communicate outcomes (Alt 2). Unlike Santander, where the TA manager deliberately chose Alt 1 to preserve identity, the CleverLoan setting — where the Branch Manager prioritizes efficiency — defaults toward Alt 2. Identity-sensitive modeling reveals what this choice costs.

**What this reveals beyond Santander:** The Santander To-Be SD split one role into Human/AI variants. The CleverLoan To-Be SD does this *and* creates an entirely new role (*AI-Supported Consultant*) that has no precedent in the As-Is model. This tests the framework's ability to represent AI-enabled role creation — not merely role redistribution — as an identity outcome.

---

## LC-4: To-Be SR Model

**What this model conveys:**

- The *Loan Consulting* boundary (blue) shows the post-AI workflow: *Conduct Loan Consultation*, *Follow AI-Generated Guidelines*, *Understand AI Decision*, with contributions to *Quick Process* ($++$), *Expedited Loan Process* ($++$), *Accurate Decisions* ($+$), and *Customer Satisfaction* (?/undetermined).
- **Max's boundary** reveals the full complexity of identity threat when left unaddressed by organizational design:
  - *Productive adaptation:* *Proactively Approach Customers Using AI Data* ($+$ Professional Standing, $+$ Customer Trust) and *Provide Cross-Selling Advisory* ($+$ Professional Standing) show Max finding new ways to assert professional value using AI-generated insights.
  - *Destructive resistance:* *Protect Professional Identity* decomposes into *Demonstrate Superiority Over AI-Dependent Consultants* and *Manipulate Data to Influence AI Decision*, both contributing $--$ to *Compliance Assured* and $--$ to *Organizational Cohesion*. These are organizationally destructive behaviors that emerge specifically because identity threat was not addressed in the system's requirements.
  - *Transparency gap:* The softgoal *AI Reasoning be Understood* receives a $--$ contribution, indicating that CleverLoan's black-box design Breaks the transparency condition that would enable Max to engage productively with AI reasoning. This directly contrasts with the Santander case, where *AI reasoning Explained* contributed $++$ to *Professional Oversight Enabled*. The same requirement category — transparency — surfaces in both cases, but with opposite outcomes: met in Santander (by design), broken in CleverLoan (by omission).
  - *Communicate AI Decision* fulfills the goal *Customer be Served*, while softgoals *Specialist Distinction* ($+$), *Expert Judgment* ($+$), and *Customer Trust* ($+$) reflect Max's continued professional self-concept.
- **Anna's boundary** shows empowerment with dependency risk:
  - *Follow AI Guidelines* contributes $+$ to *Competence*, $+$ to *Professional Scope be Expanded*, and $+$ to *Helpfulness* — genuine professional growth through AI augmentation.
  - *Seek Reassurance From AI Provider* contributes $-$ to *Competence*, revealing that over-reliance on the AI system undermines the very competence that augmentation is supposed to build.
  - *Authority loss:* The softgoal *Decision Authority be Preserved* receives a $--$ contribution from *Refer Decision Responsibility to AI*. This is analytically significant: Anna *gains* professional scope but *never acquires* decision authority. She transitions from having no authority (As-Is, service desk role) to operating under delegated authority that is not hers (To-Be, following AI guidelines). The requirement for authority preservation surfaces even for the empowered actor — revealing that scope expansion without decision authority is an incomplete form of professional identity development.
  - *Enter Customer Data* defines part of her operational scope; *Customer Trust* remains undetermined (?), reflecting that the customer's response to AI-mediated decisions is not yet known.
  - The goal *Customer be Served* parallels Max's, but is achieved through fundamentally different means — compliance with AI guidelines rather than autonomous judgment.
- The *AI Finance Specialist* (CleverLoan) processes *Customer Data* and produces *Decision Documentation* that flows to both *Contract Processing* and Anna's operational path.

**Key analytical point:** The To-Be SR does not propose a solution — it models the actual situation as it unfolded. Max's boundary shows that unaddressed identity threat produces *both* productive adaptation *and* organizationally destructive behavior simultaneously. The same actor who proactively uses AI data for cross-selling also manipulates data to undermine the AI system's decisions. This duality — invisible without identity-sensitive modeling — represents a requirements gap: no functional requirement addresses the conditions under which experienced professionals turn from productive adaptation to destructive resistance. Anna's boundary shows the complementary risk: scope expansion without decision authority and with AI dependency creates an incomplete form of professional development that may itself become a future identity concern.

The two new softgoals — *AI Reasoning be Understood* (Max) and *Decision Authority be Preserved* (Anna) — ensure that all four requirement categories from the paper's Table 2 are exercisable in the CleverLoan models. Transparency and authority preservation surface as *unmet* requirements in the failure case, complementing the Santander case where they were *met* through deliberate design. The framework thus demonstrates diagnostic value: it surfaces these requirement categories regardless of whether the organization addresses them.

**What this reveals beyond Santander:** The Santander To-Be SR showed how identity-sensitive *design choices* resolve tensions (transparency, authority preservation, professional growth). The CleverLoan To-Be SR shows what happens when such choices are *absent*: the framework can model not only solutions but also failure modes. Specifically:
- *Transparency:* Santander's "AI reasoning Explained" → $++$ "Professional Oversight Enabled" versus CleverLoan's "AI Reasoning be Understood" ← $--$ (black-box design). Same requirement, opposite outcomes.
- *Authority preservation:* Santander's "Decision Authority be Maintained" (met through collaborative design) versus CleverLoan's "Decision Authority be Preserved" ← $--$ "Refer Decision Responsibility to AI" (unmet for both actors — lost by Max, never acquired by Anna).
- *Competence:* Santander's "Professional Competence" and "Professional Growth" (positive development) versus CleverLoan's mixed outcome (Anna: $+$ from AI guidelines but $-$ from over-reliance; Max: no development path at all).

This tests the framework's diagnostic capability — its ability to surface identity-related requirements gaps by representing the consequences of ignoring identity in system design.

---

## Coverage Analysis: What CleverLoan Adds to the Santander Case

Following the software testing analogy (Professor's guidance), the table below tracks which aspects of the identity-sensitive modeling framework are exercised by each case:

| Modeling capability | Santander | CleverLoan | Notes |
|---|---|---|---|
| Person-based identity (agent) | Tested (Tim) | Tested (Max, Anna) | Both cases exercise this |
| Role-based identity (role) | Tested (Hiring Expert, HR Professional) | Tested (Loan Consultant, Loan Expert) | Both cases |
| Relational identity (dependencies) | Tested (Tim–Sarah, Tim–AI) | Tested (Max–Customer, Anna–AI) | Both cases |
| **Multiple agents in same role with divergent identities** | Not tested | **Tested (Anna vs Max)** | New coverage |
| **AI-enabled role creation (not just role split)** | Not tested | **Tested (AI-Supported Consultant)** | New coverage |
| Identity-sustaining design (success path) | Tested (Alt 1 collaboration) | Not primary focus | Santander covers this |
| **Identity threat without organizational mitigation (failure path)** | Not tested | **Tested (Max's destructive behaviors)** | New coverage |
| **Productive and destructive responses in same actor** | Not tested | **Tested (Max adapts AND resists)** | New coverage |
| **Empowerment with dependency risk** | Not tested | **Tested (Anna's over-reliance)** | New coverage |
| **Transparency as unmet requirement** | Tested as met (AI reasoning Explained → ++ Professional Oversight) | **Tested as unmet (AI Reasoning be Understood ← −−)** | Same category, opposite outcome — new coverage |
| **Authority preservation as unmet requirement** | Tested as met (Decision Authority be Maintained) | **Tested as unmet (Decision Authority be Preserved ← −−)** | Same category, opposite outcome — new coverage |
| Managerial championing of identity preservation | Tested (Sarah) | Not present (Branch Manager prioritizes efficiency) | Contrasting managerial orientations |
| Contribution analysis on identity softgoals | Tested | Tested | Both cases |
| ISA role specialization for AI | Tested (Human/AI HR Expert) | Tested (Human/AI Finance Specialist) | Both cases |
| Reciprocal human-AI dependencies | Tested (feedback loop) | Tested (Customer Data / Loan Recommendation) | Both cases |

**Summary:** CleverLoan adds seven new "test paths" not exercised by the Santander case: (1) divergent identities within the same role, (2) AI-enabled role creation, (3) unmitigated identity threat as a failure mode, (4) simultaneous productive and destructive responses in one actor, (5) empowerment with dependency risk, (6) transparency as an unmet requirement (diagnostic mode), and (7) authority preservation as an unmet requirement across both threatened and empowered actors. Together, the two cases provide broader coverage of the modeling framework's analytical capabilities, exercising all four requirement categories from Table 2 across both success (Santander) and failure (CleverLoan) conditions.

---

## Domain-Specific Differences from Santander

| Dimension | Santander | CleverLoan |
|---|---|---|
| **AI type** | Augmentative (CV screening support) | Substitutive (automated loan decisions) |
| **Managerial orientation** | TA manager championed human-AI collaboration | Branch Manager prioritized efficiency |
| **Identity outcome** | Resistance → role expansion (success) | Resistance + data manipulation (unresolved) |
| **Stakeholder contrast** | Single protagonist (Tim) with manager support (Sarah) | Two protagonists (Max, Anna) with divergent responses |
| **Organizational structure** | Hiring team with dedicated manager | Business unit with verification department |
| **AI transparency** | Real-time visualization and explanation | Black-box guidelines and documentation |
| **Temporal trajectory** | Four-year progression to collaboration | Ongoing tension without resolution |
