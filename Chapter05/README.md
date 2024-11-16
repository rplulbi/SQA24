# Test UAT
Software Quality Engineering
============================

        Testing, Quality Assurance, and Quantiable Improvement


# What Is Quality?

- 	  Perspectives and Expectations

-	  Quality Frameworks and ISO-9126

-	  Correctness, Defect, and Quality

-	  A Historical Perspective

# Perspectives and Expectations

- 	  General: 

	  "good" software quality

-	  Perspectives:

	  people/subject’s view, software as object

-	  Expectations: 

	  quality characteristics & level

-	  In Kitchenham & Pfleeger (1996):

	  . Transcendental view: seen/not-defined.
	  . User view: fitness for purpose.
	  . Manufacturing view: conform to specs.
	  . Product view: inherent characteristics.
	  . Value-based view: willing to pay.

# Quality Perspectives

- 	  Perspectives: subject and object

-	  Subject: people’s perspectives

	  . external/consumer: customers and users
	  . internal/producer: developers, testers, and managers
	  . other: 3rd party, indirect users, etc.
	  . users generalized: other systems etc.
	  . focus on external/consumer side

-	  Objects of our study:

	  . software products, systems, and services
	  . stand-alone, embedded, etc.
	  . affect quality definitions/expectations

# Quality Expectations

-	 Expectations from different people

-	 External/consumer expectations:

	 . "good enough" for the price

	   	 -	 fit-for-use, doing the "right things"
		 -	 conformance, doing \things right"
		 	 -> validation and verification (V&V)

	 . customer vs user (price?)
	 . internal vs external user
	 . generalized user: other hw/sw/system/etc.

-	 Expectations for different software:

	 . general: functionality & reliability,
	 . usability: GUI/end-user/web/etc.,
	 . interoperability: embedded systems,
	 . safety: safety-critical systems, etc.

-	 Internal/producer:

	 . "good enough" for the cost

	   	 -	 mirror consumer side
		 -	 functionality & correctness via V&V

	 . cost: developers vs managers
	 . service related: maintainability
	 . interfacing units: interoperability
	 . 3rd party: modularity

-	 Different expectations for different types of
	 products and market segments too.

-	 Different QA/SQE activities needed.

# ISO-9126 Quality Framework

- 	 ISO 9126 quality characteristics:

	 . Functionality: what is needed?
	 . Reliability: function correctly.
	 . Usability: effort to use.
	 . Efficiency: resource needed.
	 . Maintainability: correct/improve/adapt.
	 . Portability: one environment to another.

-	 Impact and limitations:

	 . Characteristics into sub-characteristics
	 . Comprehensive framework
	 . Strict hierarchy -> other alternatives


# Other Quality Frameworks

- 	Adaptation of ISO-9126:

	. customized for companies

	  e.g., IBM’s CUPRIMDSO.

	. adapted to application domains

	  reliability, usability, security for Web

-	  Other quality frameworks/mega-models

	  . McCall: factors, criteria, and metrics
	  . Basili: GQM (goal-question-metric)
	  . SEI/CMM: process focus/levels
	  . Dromey: component reflects Q-attributes
	  . Defect-based view: common in industry
	    cost of defect: by Boehm, NIST, etc.

# Correctness, Defect and Quality

- 	  High quality ~ low defect

	  . intuitive notion related to correctness
	  . quality problem ~ defect impact
	  . widely accepted, but need better definitions

-	  Defect/bug definition

	  . failure: external behavior
	    deviation from expected behavior

	  . fault: internal characteristics
	    cause for failures

	  . error: incorrect/missing human action
	    error source: conceptual mistakes etc.

	  . defect: error, fault, failure collectively

	  . bug/debug: problematic terms, avoid

Correctness, Defect and Quality

![](../pics/2-1.png)

-	  Relations: errors -> faults -> failures

	  not necessarily 1-1, Fig 2.1 (p.21) above

-	  Other issues:

	  . QA as dealing with defect: Chapter 3
	  . defect handling/resolution: Chapter 4


# Defining Quality in SQE

-	  Quality: views and attributes

![](../pics/2-2.png)

-	  SQE focus: correctness-related.


# Quality: Historical Perspective

-	  Software vs other products/systems:

	  . pre-software/IT: manufacturing process
	    -> physical-object attributes (defects)

	  . service: manage expectations:
	    - 0 defect -> 0 defection

	  . IT and software: below

-	  The new meaning of quality in the information age (Prahalad & Krishnan 1999):

	  . Conformance/adaptability/innovation
	  . Traditional: conformance only
	  . Domain specific (for info. age):
	    specificity, stability, evolvability

-	  A historical perspective of SE, in 4 stages (Musa & Everett, 1990):

	  . functional: focus on automation
	  . schedule: timely/orderly product intro
	  . cost: competitive marketplace
	  . reliability: meet user expectations

-	  Historical perspectives based on:

	  . measurement/feedback (Part IV),
	  . process maturity, etc.

-	  So, what is software quality?

	  many aspects/perspective, but correctness-centered in SQE

# Quality Assurance (QA)

-		 QA as Dealing with Defect

-		 Defect Prevention

-		 Defect Detection and Removal

-		 Defect Containment

# Defect vs. QA

-	QA: quality assurance

	-   focus on correctness aspect of Quality
	-   QA as dealing with defects

	    -  post-release: impact on consumers
	    -  pre-release: what producer can do

	-   what: testing & many others
	-   when: earlier ones desirable (lower cost) but may not be feasible
	-   how => classification below

-	How to deal with defects:

	-   prevention
	-   removal (detect them first)
	-   containment


# QA Classification

![image](https://github.com/rplulbi/SQA/assets/15622730/3a46441b-7aea-4d85-8043-d571b1e1fd3d)

-	Fig 3.1 above (p.30): QA as barriers

	-   dealing with errors, faults, or failures
	-   removing or blocking defect sources
	-   preventing undesirable consequences

# Error/Fault/Failure & QA

-	Preventing fault injection

	-	error blocking (errors, not faults)
	-	error source removal

-	Removal of faults (pre: detection)

	-	inspection: faults discovered/removed
	-	testing: failures trace back to faults

-	Failure prevention and containment:

	-	local failure, not global failure
		via dynamic measures to tolerate faults

	-	failure impact, not safety assurance


# Defect Prevention Overview

-	Error blocking

	-     error: missing/incorrect actions
	-     direct intervention to block errors
	      => fault injections prevented

	-     rely on technology/tools/etc.

-	Error source removal

	-     root cause analysis
	      => identify error sources

	-     removal through education/training/etc.

-	Systematic defect prevention via process improvement.

-	Details: Chapter 13.


# Formal Method Overview

-	Motivation

	-	fault present:

		-     revealed through testing/inspection/etc.

	-	fault absent: formally verify.

		(formal methods => fault absent)

-	Basic ideas

	-	behavior formally specified:

		-	 pre/post conditions, or
		-	 as mathematical functions.

	-	verify "correctness":

		-	 intermediate states/steps,
		-	 axioms and compositional rules.

	-	Approaches: axiomatic/functional/etc.

-	Details: Chapter 15.


# Inspection Overview

-	Artifacts (code/design/test-cases/etc.) from req./design/coding/testing/etc. phases.

-	Informal reviews:

	-	 self conducted reviews.
	-	 independent reviews.
	-	 orthogonality of views desirable.

-	Formal inspections:

	-      Fagan inspection and variations.
	-      process and structure.
	-      individual vs. group inspections.
	-      what/how to check: techniques.

-	Details: Chapter 14.


# Testing Overview

-	Product/Process characteristics:

	-	object: product type, language, etc.
	-	scale/order:
		unit, component, system, ...

	-	who: self, independent, 3rd party

-	What to check:

	-    	verification vs. validation
	-	external specifications (black-box)
	-	internal implementation (white/clear-box)

-	Criteria: when to stop?

	-	coverage of specs/structures.
	-	reliability => usage-based testing

-	Much, much more in Part II.


# Fault Tolerance Overview

-	Motivation

	-	fault present but removal infeasible/impractical

	-	fault tolerance => contain defects

-	FT techniques: break fault-failure link

	-  	recovery: rollback and redo
	-	NVP: N-version programming
		fault blocked/out-voted

-	Details: Chapter 16.


# Safety Assurance Overview

-	Extending FT idea for safety:

	-	fault tolerance to failure \tolerance"

-	Safety related concepts:

	-      	safety: accident free
	-	accident: failure w/ severe consequences
	-	hazard: precondition to accident

-	Safety assurance:

	-      hazard analysis
	-      hazard elimination/reduction/control
	-      damage control





# QA in Context

-       Defect Handling

-       QA in Software Processes

-       V&V Perspective

-       QA: Defect View vs V&V View


# QA in Context

-       QA and the overall development context

	-  defect handling/resolution
	-  activities in process
	-  alternative perspectives:

verification/validation (V&V) view

-       Defect handling/resolution

	-      status and tracking
	-      causal (root-cause) analysis
	-      resolution: defect removal/etc.
	-      improvement: break causal chain

# Defect Measurement and Analysis

-       Defect measurement:

	-      parallel to defect handling
	-      where injected/found?
	-      type/severity/impact?
	-      more detailed classification possible?
	-      consistent interpretation
	-      timely defect reporting

-       Defect analyses/quality models

	-      as followup to defect handling.
	-      data and historical baselines
	-      goal: assessment/prediction/improvement
	-      causal/risk/reliability/etc. analyses

-       Details in Part IV.


# QA in Software Processes

-       Mega-process:

	initiation, development, maintenance, termination.

-       Development process components:

	requirement, specification, design, coding, testing, release.

-       Process variations:

	-	waterfall development process
	-	iterative development process
	-	spiral development process
	-	lightweight/agile development processes and XP (extreme programming)
	-	maintenance process too
	-	mixed/synthesized/customized processes

-       QA important in all processes


# QA in Waterfall Process

![image](https://github.com/rplulbi/SQA/assets/15622730/02300adf-67b8-4931-b6dc-61d0193d92d1)


-       QA throughout process (Fig 4.1 p.45)

	-  defect prevention in early phases
	-  focused defect removal in testing phase
	-  defect containment in late phases
	-  phase transitions: inspection/review/etc.


# QA in Software Processes

-       Process variations (not waterfall) and QA:

	-	iterative: QA in iterations/increments
	-	spiral: QA and risk management
	-	XP: test-driven development
	-	mixed/synthesized: case specific
	-	more evenly distributed QA activities

-       QA in maintenance processes:

	-     	focus on defect handling;
	-	some defect containment activities for critical or highly-dependable systems;
	-	data for future QA activities

-       QA scattered throughout all processes


# V&V

-       Core QA activities grouped into V&V.

-       Validation: w.r.t. requirement (what?)

	-	appropriate/fit-for-use/\right thing"?
	-	scenario and usage inspection/testing;
	-	system/integration/acceptance testing;
	-	beta testing and operational support.

-       Verification: w.r.t. specification/design (how?)

	-	correct/\doing things right"?
	-	design as specification for components;
	-	structural and functional testing;
	-	inspections and formal verification.


# V&V in Software Process

![image](https://github.com/rplulbi/SQA/assets/15622730/9d295558-8120-4ba3-9b24-bd3987319ba9)

-       V&V in V-model above (Fig 4.2 p.49):

	-   V-model as bent-over waterfall
	-   left-arm: implementation (& V&V)
	-   right-arm: testing (& V&V)
	-   user@top vs. developer@bottom


# V&V vs DC View

-       Two views of QA:

	-   V&V view
	-   DC (defect-centered) view in this book
	-   Interconnected: mapping possible?

-       Mapping between V&V and DC view:

	-	V&V after commitment
		(defect injected already)
		=> defect removal & containment focus

	-	Verification: more internal focus
	-	Validation: more external focus
	-	In V-model: closer to user (near top) or developer (near bottom)?


# DC-V&V Mapping (Table 4.1, p.51)

![image](https://github.com/rplulbi/SQA/assets/15622730/3d6605ba-1979-474e-ae96-dcf602a7b75c)
