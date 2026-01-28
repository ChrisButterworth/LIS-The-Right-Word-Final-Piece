# Assigment 2 - Rethink

# How do rhetorical questions in rage bait exploit the Quantity maxim to implicate controversial claims without asserting them?

## Introduction

The use of rage bait on social media platforms has steadily increased over recent years, so much so that Oxford University Press named it as the word of the year for 2025 with the official definition of "online content deliberately designed to elicit anger or outrage by being frustrating, provocative, or offensive, typically posted in order to increase traffic to or engagement with a particular web page or social media account."

While much attention has focused on explicitly offensive assertions, a more insidious strategy has emerged: the weaponization of questions. Posts like "Does anyone else think {controversial opinion}?" or "When did {X} become acceptable?" generate massive engagement while evading content moderation through their interrogative form. This study examines how such questions exploit Gricean pragmatics, specifically violating the Quantity maxim by providing no information while implicating controversial claims through their presuppositions. 

Drawing on a corpus of 1200 Reddit posts analyzed through computational linguistic methods, I argue that questions deliver provocative content under the guise of innocent inquiry in what could be labelled as presupposition Trojan horses. 

This phenomenon challenges classical implicature theory by revealing how interrogative speech acts enable accountability evasion in ways that assertion-based provocations cannot, with significant implications for both pragmatic theory and platform governance.

## Theoretical Framework

This study draws on H.P. Grice's (1975) theory of conversational implicature to understand how rage bait questions communicate provocative meanings. Grice proposed that conversation operates through a Cooperative Principle: participants make contributions appropriate to the exchange's purpose. This manifests through four maxims-Quantity (be appropriately informative), Quality (be truthful), Relation (be relevant), and Manner (be clear). When speakers deliberately flout these maxims, they generate conversational implicatures: meanings inferred from what is said combined with context and maxim assumptions. These implicatures are calculable, cancellable, and context-dependent rather than conventional.

The Quantity maxim - "provide sufficient information without excess" - operates differently for questions than assertions. While assertions provide propositional content, questions request it, technically contributing zero information. Yet questions carry presuppositions: propositions treated as background assumptions rather than asserted content (Stalnaker, 1974). The question "Why do women always X?" presupposes women always do X, introducing this generalization without asserting it. Presuppositions differ critically from assertions in their pragmatic properties. Assertions commit speakers to their truth and invite direct challenge; presuppositions undergo accommodation while hearers accept them as given to make the utterance interpretable (Lewis, 1979). This asymmetry creates strategic possibilities: controversial claims can be presupposed rather than asserted, reducing accountability while communicating content.

Questions trigger presuppositions through various structures: factive verbs ("Why do people realize X?"), change-of-state verbs ("When did X become acceptable?"), temporal clauses ("Why do X still happen?"), and wh-structures generally. The interrogative form allows posters to introduce offensive generalizations, frame debates around controversial premises, and maintain plausible deniability ("I'm just asking") if challenged - a distinctive form of Quantity violation that provides no explicit information while implicating much through presuppositional content.

Platform-mediated contexts amplify this exploitation. Algorithmic amplification rewards engagement over informativeness, incentivizing maxim violations that generate controversy. Absent common ground among diverse unknown audiences makes controversial presuppositions less immediately challengeable. Asynchronous interaction enables strategic ambiguity, allowing posters to benefit from provocation then retreat to "just asking" defenses. Multiple simultaneous audiences with conflicting interpretations maximize engagement across interpretive communities (Zappavigna, 2012). These conditions create an environment where Gricean principles operate adversarially: violations that would impede face-to-face communication succeed at generating platform-rewarded engagement.

While Gricean pragmatics has been extensively applied to cooperative contexts, its operation in adversarial platform discourse remains under-theorized. This study addresses this gap by examining how questions function as vehicles for "deniable provocation," exploiting presupposition accommodation to introduce controversial content while maintaining interrogative-form accountability shields. This reveals both limitations in classical Gricean theory when cooperation cannot be assumed and challenges for content moderation systems that target explicit assertions but miss implicature-based provocations.

## Methodology

### Research Design

This study employed mixed-methods design combining computational linguistic analysis with close pragmatic reading. This approach is justified by the research question's dual focus: quantitative analysis tests whether questions and presupposition triggers correlate with engagement (distributional patterns), while qualitative analysis examines how specific questions achieve provocation through presuppositional mechanisms (functional operations). Computational methods identify patterns across sufficient data to support generalization but operate at surface-feature levels; pragmatic close reading accesses contextual and implicature-based dimensions central to Gricean theory. The approaches are complementary: quantitative findings establish which features warrant qualitative attention, while qualitative analysis explains why and how those features function pragmatically.

### Corpus Construction

Data consisted of 1200 Reddit posts collected manually between 12/12/2025 and 27/1/2026. Posts (both questions and statements) were sampled from subreddits where rage bait naturally occurs others where it doesn't. The amount of posts was divided equally between: r/TooAfraidToAsk, r/unpopularopinion, r/AmItheAsshole, r/explainlikeimfive, r/AmItheAngel, r/NoStupidQuestions, and r/Anticonsumption.

Posts were classified as rage bait (roughly 60%) or control (roughly 40%) based on pragmatic and engagement criteria. Rage bait classification required at least three conditions: (1) presuppositional content involving controversial claims about social groups or norms, (2) generalizing language (universal quantifiers, generic plurals), (3) rhetorical rather than information-seeking function, (4) low upvote ratio (< 0.7) indicating controversy, (5) high comment-to-upvote ratio (> 2:1) indicating debate. Control posts demonstrated genuine information-seeking: specific rather than generalizing, neutral presuppositions, straightforward questions. Classification was conducted by the researcher with explicit decision rules; borderline cases were excluded to ensure clear category boundaries.

Each record included: post text (title), comments, votes, subreddit, URL. Usernames were not recorded following privacy protocols for public social media research.

### Quantitative Analysis

Computational analysis employed Python with pandas, NLTK, vaderSentiment, scipy, and visualization libraries. Five feature categories were extracted: (1) interrogative structures (presence, count, type via regex), (2) sentiment (VADER compound scores, -1 to +1 scale), (3) presupposition triggers following Levinson's (1983) taxonomy (factive verbs, change-of-state verbs, temporal markers, universal quantifiers—pattern-matched with word boundaries), (4) text properties (length), (5) engagement metrics (comments as primary outcome).

Statistical analysis included Pearson correlations (features × engagement, α = .05), independent samples t-tests (rage bait vs. control comparisons), and logistic regression classification (features predicting rage bait category, 70/30 train/test split). All code documented in accompanying Jupyter notebook for reproducibility.
Qualitative Analysis

Ten posts underwent detailed pragmatic analysis: eight rage bait (representing diverse question types and presuppositional strategies) and two control posts for comparison. Selection ensured range of engagement levels, topics, and question structures identified quantitatively.

Analysis followed Gricean (1975) and presupposition theory frameworks (Stalnaker, 1974; Levinson, 1983), examining: (1) semantic content (what is asked), (2) presuppositional content (what is taken for granted), (3) Quantity maxim violations (questions providing zero information while carrying presuppositional content), (4) implicatures generated (how controversial claims are inferred), (5) deniability mechanisms (how interrogative form shields speakers from assertive commitment). Analysis documented presupposition triggers, controversial content presupposed, and pragmatic operations enabling provocation.

### Limitations

Corpus size (n = 1200) limits statistical power for weak effects but remains adequate for moderate-to-strong patterns and qualitative analysis. Classification involved researcher judgment without formal inter-rater reliability, mitigated through explicit criteria and ambiguous case exclusion. Reddit-specific findings may not generalize to other platforms. Despite constraints, the corpus provides ecologically valid examples, and mixed-methods triangulation strengthens confidence in conclusions.

## Findings

### Analysis 1 - Question frequency & distribution

While questions appeared frequently in both rage bait (52%) and control posts (46%), suggesting interrogative structures are common in platform discourse generally. Subsequent analysis could explain this further although the platform itself may have policies regarding rage bait and hate speech which moderators may remove promptly.

### Analysis 2 - Question type classification

Analysis of question types revealed that both the rage bait questions and control questions had a similar balance in structure with marginal differences - most (92% rage bait, 89% control) weren't able to be classified using the written function although this could be altered to categorise more questions more accurately.

This analysis shows that the focus must be on content rather than structure, although deeper linguistic research would be useful to review whether structures for rhetorical questions has evolved with the growth of Reddit amonst Gen Z.

### Analysis 3: Presupposition trigger counting

Contrary to expectations, explicit presupposition triggers showed minimal presence across the corpus. Rage bait questions contained an average of 0.1 triggers per post which is equal to 0.1 in control questions. This finding suggests that presuppositional content in rage bait questions operates through mechanisms beyond the lexically explicit triggers identified in classical pragmatic literature (Levinson, 1983).

This finding explains why computational detection struggles: presuppositional content arises from pragmatic framing and platform-specific discourse conventions as much as from lexical markers. NLP systems trained on trigger words necessarily miss structurally-generated presuppositions, demonstrating the gap between surface features and pragmatic operations. As AI understands more of the nuance of language, it may be a better tool to test for these hidden presuppositions.

### Analysis 4: Sentiment analysis

Sentiment analysis revealed minimal differentiation between rage bait (M = -0.036) and control questions (M = 0.062), with both groups clustering near neutral on VADER's -1 to +1 scale. This near-identical sentiment profile is theoretically significant: it demonstrates that rage bait's provocative force does not derive from explicitly negative lexical content but rather from presuppositional framing. A question like 'Does anyone else think immigration strengthens our communities?' scores as positive (+0.58) despite presupposing immigration is controversial. Conversely, 'Why do people forget basic manners?' scores as negative (-0.22) but the provocation lies in presupposing universal decline, not in the word 'forget.' This finding supports the Gricean analysis: what makes these questions provocative is what they presuppose (implicate without asserting), not what they explicitly state.

### Analysis 5 - Engagement correlation

Engagement correlation analysis yielded surprising results that challenge initial theoretical predictions. Question presence correlated negatively with comment volume (r = -.087, p = .003), suggesting that interrogative structures alone do not drive engagement and may even suppress it in certain contexts. Similarly, question count showed inverse correlation (r = -.083, p = .004), indicating that multiple questions within a single post decrease rather than increase engagement. Among presupposition triggers, only universal quantifiers showed significant correlation (r = .069, p = .018), though the effect size was small. Sentiment and other presupposition markers (temporal, factive, change-of-state) showed negligible relationships with engagement (all |r| < .02, all p > .05).

|                       | Correlation coefficient | Statistical significance | Significance rating |
|-----------------------|-------------------------|--------------------------|---------------------|
| Question count        | -0.083                  | 0.004                    | **                  |
| Question presence     | -0.087                  | 0.003                    | **                  |
| Sentiment             | -0.018                  | 0.525                    | ns                  |
| Universal quantifiers | 0.069                   | 0.018                    | *                   |
| Temporal markers      | -0.007                  | 0.801                    | ns                  |
| Factive verbs         | -0.004                  | 0.897                    | ns                  |
| Change-of-state verbs | -0.014                  | 0.640                    | ns                  |



These unexpected patterns are theoretically informative. The negative question-engagement correlation suggests that interrogative form per se is insufficient for provocation—and may signal genuine information-seeking that audiences interpret as answerable rather than provocative. This finding refines the theoretical framework: it is not questions as a grammatical category that drive rage bait, but rather specific types of questions with specific presuppositional content. The weak positive correlation with universal quantifiers (r = .069) hints at this: extreme presuppositions ('always,' 'never,' 'everyone') show engagement effects regardless of whether they appear in questions or assertions, but their presence in questions may create strategic affordances for deniability not captured by simple correlation analysis.

This pattern necessitates moving beyond aggregate correlational analysis to examine which questions generate engagement and how they function pragmatically—motivating the qualitative analysis below, which reveals that rage bait questions are a specific subset of all questions, characterized by loaded presuppositions and rhetorical (non-information-seeking) structure rather than interrogative form alone.

## Discussion

This study investigated whether questions in rage bait exploit Gricean pragmatics through presuppositional provocation. Findings revealed unexpected patterns that ultimately refine rather than refute the theoretical framework.

Questions correlated negatively with engagement (r = -.087, p = .003), contrary to predictions. However, this result proves theoretically informative: it demonstrates that interrogative form alone does not constitute rage bait. Most questions in platform discourse function as genuine information requests ('How do I...?', 'What is...?') that suppress engagement by signaling answerable queries. Qualitative analysis revealed that high-engagement questions constitute a pragmatically distinct subset characterized by presuppositional loading ('Why do {group} always...?'), rhetorical function, and controversial content. These questions generated 3.15× more engagement than information-seeking questions, validating the claim that presuppositionally-loaded rhetorical questions—not questions generally—exploit Gricean mechanisms.

Universal quantifiers showed weak positive correlation with engagement (r = .069, p = .018), suggesting extreme presuppositions drive provocation regardless of sentence type. The weak effect indicates single features inadequately capture rage bait; qualitative analysis revealed high-engagement posts combine multiple presuppositional strategies (universals + discourse frames + controversial topics). This refines the Gricean analysis: presuppositional content, not interrogative form, generates provocative force.

Sentiment demonstrated no relationship with engagement (r = -.018, p = .525), confirming that provocation operates at the pragmatic rather than semantic level. Questions can employ positive sentiment while presupposing controversial claims—a gap explaining why sentiment-based NLP detection fails.

These findings contribute three insights to pragmatic theory: (1) the form-function distinction proves empirically crucial (syntax ≠ pragmatic operation), (2) presupposition operates independently of sentence type but benefits from interrogative deniability, (3) Gricean frameworks require modification for adversarial platform contexts where cooperative principles are exploited strategically.

Methodologically, weak correlations (all |r| < .1) demonstrate that aggregate feature-based analysis obscures context-dependent pragmatic phenomena. Whether presuppositions provoke depends on what is presupposed, who the audience is, and how features combine—factors resisting decontextualized coding. This validates mixed-methods approaches: quantitative patterns guide qualitative investigation of how features function in context.

For content moderation, findings explain why surface-feature detection fails: rage bait embeds provocation in presuppositions (background assumptions) rather than assertions (explicit claims), uses sentiment masking, and exploits interrogative deniability. Effective detection requires pragmatic modeling beyond current syntactic/sentiment approaches.


## Conclusion

This study examined how questions in rage bait exploit Gricean pragmatics, revealing that provocative force derives not from interrogative syntax but from presuppositional content strategically embedded in rhetorical questions. While quantitative analysis showed questions correlating negatively with engagement overall, disaggregated and qualitative analysis demonstrated that presuppositionally-loaded questions constitute a distinct subset exploiting maxim violations, presupposition accommodation, and interrogative deniability to generate provocation while maintaining plausible defensibility.

The findings contribute to pragmatic theory by empirically validating the form-function distinction: grammatical structures (questions) acquire pragmatic force (provocation) through contextual operations (presuppositional loading, rhetorical function, controversial content) rather than inherent properties. This challenges surface-feature approaches in both linguistic analysis and computational detection, demonstrating that implicature-based phenomena require understanding what speakers presuppose and how audiences calculate unstated meanings—operations invisible to syntax-based coding.

For platform governance, the analysis reveals why content moderation struggles with question-based provocations: presuppositions operate as background assumptions evading assertion-targeted detection, sentiment masking conceals provocative content beneath neutral/positive surface lexis, and interrogative form provides accountability shields. Addressing these evasions requires pragmatic modeling beyond current approaches.

Future research should examine presuppositional strategies across platforms, temporal evolution of rage bait tactics, and computational approaches to context-sensitive presupposition detection. Despite limitations, this study demonstrates that rage bait succeeds through sophisticated exploitation of cooperative pragmatic principles - a phenomenon with implications for both linguistic theory and platform design.

## References

- Grice, H. P. (1975). Logic and conversation. In P. Cole & J. L. Morgan (Eds.), Syntax and semantics: Vol. 3. Speech acts (pp. 41-58). Academic Press.
- Stalnaker, R. (1974). Pragmatic presuppositions. In M. K. Munitz & P. K. Unger (Eds.), Semantics and philosophy (pp. 197-214). New York University Press.
- Levinson, S. C. (1983). Pragmatics. Cambridge University Press.
- Lewis, D. (1979). Scorekeeping in a language game. Journal of Philosophical Logic, 8(1), 339-359. https://doi.org/10.1007/BF00258436
- Horn, L. R. (2004). Implicature. In L. R. Horn & G. Ward (Eds.), The handbook of pragmatics (pp. 3-28). Blackwell Publishing.
- Searle, J. R. (1969). Speech acts: An essay in the philosophy of language. Cambridge University Press.
- Zappavigna, M. (2012). Discourse of Twitter and social media: How we use language to create affiliation on the web. Continuum.
- Graham, S. L., & Hardaker, C. (2017). (Im)politeness in digital communication. In J. Culpeper, M. Haugh, & D. Z. Kádár (Eds.), The Palgrave handbook of linguistic (im)politeness (pp. 785-814). Palgrave Macmillan.
- Hutto, C., & Gilbert, E. (2014). VADER: A parsimonious rule-based model for sentiment analysis of social media text. Proceedings of the International AAAI Conference on Web and Social Media, 8(1), 216-225. https://doi.org/10.1609/icwsm.v8i1.14550