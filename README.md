# Master-thesis-for-AI-program-at-Open-Source-LAB---FAU
Does Knowing the Speaker Help? Interview-Grounded Participant Profiles for LLM-Assisted Qualitative Coding in Software Engineering Research

Abstract
Large language models (LLMs) are increasingly used to code qualitative interview data, but they
usually code each segment in isolation. Human analysts instead read the whole interview first and
interpret each statement in light of what the participant has said elsewhere. This thesis tests whether
giving an LLM a participant profile, generated from the other parts of the same interview and grounded
in quotations, improves its agreement with human coding of software-engineering interviews. Profiles
are built with a two-fold cross-fitting scheme so that the text being coded never contributes to its own
profile. To establish that any improvement comes from knowledge of the speaker rather than from
additional text, topical cues or general knowledge of the study, real profiles are compared with four
matched control profiles, the most important being the profile of another participant of the same study.
Replacement-based interventions test whether the model causally relies on the evidence it cites, and a
pre-specified mechanism analysis examines when and why profiles help or harm. The thesis reuses
interviews for which hundreds of students have each submitted a separate coding in QDAcity with
the same codebook. This yields a stable human reference and a full distribution of individual human
coders within which the LLM can be placed, while keeping the annotation effort feasible within six
months.

Contents
1 Introduction 3
1.1 Background . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 3
1.2 Problem Statement . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 3
1.3 Purpose and Scope . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 3
2 Theoretical Framework: Why Speaker Context Should Matter 3
2.1 Indexicality and the Two Contexts of Interpretation . . . . . . . . . . . . . . . . . . . . 4
2.2 The Part and the Whole in Qualitative Analysis . . . . . . . . . . . . . . . . . . . . . . 4
2.3 Why Software-Engineering Interviews Are Especially Context-Dependent . . . . . . . . 4
2.4 Why a Compact Profile Rather Than the Full Transcript . . . . . . . . . . . . . . . . . . 4
2.5 Expected Mechanisms . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 4
3 Literature Review 5
3.1 LLM-Assisted Qualitative Coding . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 5
3.2 The Missing Speaker . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 5
3.3 Grounded Profiles and Personas . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 5
3.4 Evaluating LLM Coding . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 5
3.5 Research Gap . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 5
4 Research Questions and Hypotheses 6
4.1 Research Questions . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 6
4.2 Hypotheses . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 6
4.3 Definitions of Key Terms . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 6
5 Methodology 7
5.1 Research Design Overview . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 7
5.2 Data: Existing Human-Coded Interviews . . . . . . . . . . . . . . . . . . . . . . . . . . 7
5.3 Units and Reference Labels . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 8
5.4 Interview-Grounded Participant Profiles . . . . . . . . . . . . . . . . . . . . . . . . . . 8
5.5 Experimental Conditions and Controls . . . . . . . . . . . . . . . . . . . . . . . . . . . 9
5.6 Coding Procedure . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 9
5.7 RQ1: Effect of Profiles . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 10
5.8 RQ2: Speaker Specificity . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 10

5.10 RQ4: Mechanism Analysis . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 11
5.11 Statistical Analysis and Pre-Registration . . . . . . . . . . . . . . . . . . . . . . . . . . 11
5.12 Validity . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 12
6 Scope, Assumptions and Limitations 12
7 Ethical and Data-Protection Considerations 13
8 Expected Contributions 13
9 Work Plan 13
10 Risks and Mitigation 13
11 Preliminary Thesis Outline
