# SkillSignal SA — Research Questions and Hypotheses

| Document Attribute | Details |
|---|---|
| Project Name | SkillSignal SA |
| Project ID | SSA-001 |
| Document | Research Questions and Hypotheses |
| Document Location | `docs/02_Research_Methodology/Research_Questions_and_Hypotheses.md` |
| Version | 2.0 |
| Status | Approved — Section B Finalised |
| Research Orientation | Applied, quantitative and analytical |
| Geographic Scope | South Africa, including qualifying international remote opportunities |
| Research Period | 1 November 2025 – 31 October 2026 inclusive |
| Related Documents | Research Design; Sampling Strategy; Data Dictionary; Statistical Methodology |

---

## 1. Purpose

This document defines the approved research questions and statistical hypotheses for SkillSignal SA.

It establishes what the research intends to investigate and provides the analytical structure connecting:

- The research problem.
- Research aim.
- Research objectives.
- Research questions.
- Statistical hypotheses.
- Required variables.
- Statistical analysis.
- Research findings and reporting.

The questions and hypotheses guide the analytical work but do not predetermine the results.

No research findings or statistical conclusions may be assumed before the relevant data has been collected, validated and analysed.

---

## 2. Research Context

SkillSignal SA investigates the South African technology labour market through qualifying technology job advertisements published between 1 November 2025 and 31 October 2026 inclusive.

The research focuses on seven technology job families:

| Code | Job Family |
|---|---|
| JF01 | Software Development |
| JF02 | Data and Analytics |
| JF03 | Cybersecurity |
| JF04 | IT Infrastructure and Support |
| JF05 | Cloud and DevOps |
| JF06 | Quality Assurance and Testing |
| JF07 | Business Technology |

The research investigates advertised:

- Technical and professional skills.
- Qualifications and certifications.
- Experience and seniority requirements.
- Graduate and entry-level opportunities.
- Geographic characteristics.
- Salary disclosure and remuneration.
- Employment arrangements and working conditions.
- Temporal patterns.
- Relationships between job characteristics and advertised requirements.

### 2.1 Unit of Analysis

The unit of analysis is one unique technology job advertisement representing one advertised employment opportunity.

An advertisement may have multiple job-family assignments and multiple associated skills, qualifications, experience requirements or locations.

All research questions must distinguish between unique advertisement counts and relationship-level counts where relevant.

### 2.2 Research Interpretation

The findings describe patterns in accessible qualifying job advertisements.

They must not automatically be interpreted as:

- Actual recruitment outcomes.
- Actual employee hiring rates.
- The complete South African technology labour market.
- Actual salaries received by employees.
- Statistically representative population estimates.

The project uses non-probability sampling and must report its source coverage and limitations.

---

## 3. Research Aim

To develop and apply a reproducible data analytics framework for investigating the South African technology labour market through the systematic collection, processing and analysis of technology job advertisements, generating evidence-based insights into skills demand, qualifications, experience requirements, employment opportunities, salary transparency, geographic distribution and temporal trends.

---

## 4. Research Objectives

The twelve approved research objectives provide the foundation for the research questions.

| Objective ID | Research Objective |
|---|---|
| RO-01 | Establish research framework defining South African technology labour-market scope, research period, job families and analytical boundaries. |
| RO-02 | Identify, evaluate and document suitable job advertisement sources according to relevance, accessibility, reliability, coverage and permitted use. |
| RO-03 | Acquire a defensible sample using documented and reproducible collection procedures. |
| RO-04 | Design and implement a processing pipeline to clean, standardise, validate and deduplicate acquired records. |
| RO-05 | Develop structured classification framework for assigning advertisements to seven technology job families. |
| RO-06 | Extract and standardise technical/professional skills, qualifications, experience requirements, salary information, locations and employment characteristics. |
| RO-07 | Analyse frequency/distribution of advertised skills, differences between job families and commonly requested skill combinations. |
| RO-08 | Investigate qualification, experience and entry-level requirements across selected job families. |
| RO-09 | Examine geographic distribution and characteristics of advertised opportunities in South Africa. |
| RO-10 | Investigate salary transparency, available salary ranges and differences across relevant job characteristics. |
| RO-11 | Analyse changes/patterns in advertised technology requirements over the selected research period. |
| RO-12 | Develop interactive labour-market intelligence report and supporting research publication communicating findings, limitations and implications. |

---

## 5. Approved Research Questions

The research contains twelve approved research questions.

### RQ1 — Overall Technology Skills Demand

**Research question:**

Which technical and professional skills are most frequently requested in South African technology job advertisements during the selected research period?

**Research focus:**

- Most frequently advertised technical skills.
- Most frequently advertised professional skills.
- Skill categories and distributions.
- Required versus preferred skills.
- Frequency and proportion of advertisements containing each skill.

**Related objectives:** RO-06, RO-07.

**Required variables:**

- Standardised skill name.
- Skill category.
- Skill type.
- Skill requirement level.
- Advertisement identifier.
- Skill extraction confidence.
- Skill evidence and review status.

**Proposed analytical approach:**

Descriptive frequency analysis, proportions, rankings and skill-category comparisons.

---

### RQ2 — Skills Demand by Job Family

**Research question:**

How does demand for technical and professional skills differ across the seven approved technology job families?

**Research focus:**

- Skill frequency by job family.
- Differences in technical skill requirements.
- Differences in professional skill requirements.
- Family-specific skill profiles.
- Required versus preferred skill patterns.
- Differences in skill diversity and concentration.

**Related objectives:** RO-05, RO-06, RO-07.

**Required variables:**

- Advertisement identifier.
- Job-family code.
- Standardised skill.
- Skill category.
- Skill type.
- Skill requirement level.
- Job-family classification confidence.

**Proposed analytical approach:**

Cross-tabulations, proportions, chi-square tests where appropriate, suitable sparse-data alternatives, association measures and confidence intervals.

**Important safeguard:**

Advertisements may have multiple job-family assignments. Family-specific advertisement counts may overlap and must not be interpreted as independent samples without an appropriate analytical approach.

---

### RQ3 — Skills Combinations and Relationships

**Research question:**

Which skills commonly occur together in South African technology job advertisements, and how do these combinations differ across job families?

**Research focus:**

- Frequently co-occurring skill pairs.
- Common technical skill combinations.
- Technical and professional skill combinations.
- Family-specific skill relationships.
- Graduate and entry-level skill combinations.
- Relationships between individual skills.

**Related objectives:** RO-06, RO-07.

**Required variables:**

- Advertisement identifier.
- Standardised skill identifier.
- Skill category.
- Skill type.
- Job-family assignment.
- Graduate accessibility.
- Skill requirement level.

**Proposed analytical approach:**

- Pairwise co-occurrence.
- Support.
- Confidence.
- Jaccard similarity.
- Lift.
- Association-rule analysis where justified.
- Skill-network analysis.

**Important safeguard:**

Each advertisement-skill relationship must be counted once for frequency analysis, regardless of repeated mentions in the original advertisement.

Association does not establish causation.

---

### RQ4 — Qualification and Certification Requirements

**Research question:**

What educational qualifications and professional certifications are requested across the seven technology job families?

**Research focus:**

- Educational qualification levels.
- Qualification fields.
- Required versus preferred qualifications.
- Professional certifications.
- Certification providers.
- Degree and diploma requirements.
- Equivalent experience acceptance.
- Family-specific differences.

**Related objectives:** RO-06, RO-08.

**Required variables:**

- Qualification name and level.
- Qualification field.
- Qualification requirement level.
- Certification name.
- Certification provider.
- Certification requirement level.
- Equivalent experience accepted.
- Job-family assignment.

**Proposed analytical approach:**

Frequency distributions, proportions, cross-tabulations, chi-square tests, Fisher's exact test or suitable alternatives, Cramér's V and ordinal analysis where justified.

**Important safeguard:**

Not mentioning a qualification does not establish that no qualification is required. Educational qualifications and professional certifications must remain distinct analytical categories.

---

### RQ5 — Experience and Seniority Requirements

**Research question:**

How do advertised experience requirements differ across technology job families and seniority levels?

**Research focus:**

- Minimum advertised experience.
- Maximum advertised experience.
- Experience ranges.
- Seniority levels.
- Required versus preferred experience.
- Relevant domain experience.
- Acceptance of equivalent experience.
- Differences across job families.

**Related objectives:** RO-06, RO-08.

**Required variables:**

- Original experience wording.
- Minimum experience years.
- Maximum experience years.
- Experience category.
- Experience requirement level.
- Seniority level.
- Relevant domain.
- Equivalent experience acceptance.
- Job-family assignment.

**Proposed analytical approach:**

Frequency distributions, medians, IQR, percentiles, cross-tabulations, chi-square tests, Kruskal–Wallis and Mann–Whitney U tests where appropriate.

**Important safeguard:**

Vague experience descriptions must not be converted into invented numerical values. Seniority and years of experience must be analysed as distinct concepts.

---

### RQ6 — Graduate and Entry-Level Opportunities

**Research question:**

What proportion and characteristics of advertised opportunities are accessible to graduates and entry-level candidates, and what skills, qualifications and experience requirements are associated with these opportunities?

**Research focus:**

- Graduate-specific positions.
- Entry-level accessible positions.
- Graduate programmes.
- Internships.
- Learnerships.
- Apprenticeships.
- Required qualifications.
- Experience expectations.
- Skills associated with graduate-accessible opportunities.
- Family and geographic distribution.
- Advertised salary transparency for graduate opportunities.

**Related objectives:** RO-06, RO-08, RO-09, RO-10.

**Required variables:**

- Graduate accessibility.
- Graduate-specific flag.
- Entry-level accessible flag.
- Employment type.
- Experience category.
- Qualification requirements.
- Skills.
- Job-family assignment.
- Location.
- Salary disclosure.
- Salary values where comparable.

**Proposed analytical approach:**

Frequencies, proportions, cross-tabulations, categorical comparisons, descriptive numerical comparisons and regression where justified.

**Important safeguard:**

The following groups are distinct and may overlap:

1. Graduate-specific.
2. Entry-level accessible.
3. Other opportunities.

A graduate programme is not automatically evidence that no prior experience is required. A junior role is not automatically graduate-accessible.

---

### RQ7 — Geographic Distribution of Opportunities

**Research question:**

How are advertised technology opportunities distributed across South African provinces and major locations, and how do advertised requirements vary geographically?

**Research focus:**

- Provincial advertisement distribution.
- City-level distribution.
- Multiple-location advertisements.
- South African remote opportunities.
- Hybrid and on-site opportunities.
- International remote opportunities explicitly open to South African candidates.
- Family-specific geographic patterns.
- Graduate opportunities by location.
- Geographic variation in advertised requirements.

**Related objectives:** RO-09, RO-06, RO-08.

**Required variables:**

- Province.
- City.
- Location category.
- Employer country.
- Work country.
- Work arrangement.
- Remote eligibility.
- International remote flag.
- Job-family assignment.
- Skills.
- Experience.
- Qualification requirements.

**Proposed analytical approach:**

Frequency distributions, proportions, cross-tabulations, chi-square tests, suitable sparse-data alternatives, Cramér's V, geographic concentration summaries and maps where appropriate.

**Important safeguard:**

Two geographic perspectives must remain distinct:

- Opportunity-location view: where the candidate may perform the work.
- Employer-location view: where the advertising or hiring organisation is based.

International remote opportunities must be reported separately from domestic opportunities.

---

### RQ8 — Salary Disclosure

**Research question:**

To what extent do South African technology job advertisements disclose salary information, and how does salary disclosure vary across job family, experience and location?

**Research focus:**

- Overall salary disclosure rate.
- Disclosure by job family.
- Disclosure by experience category.
- Disclosure by geographic category.
- Disclosure by employment type.
- Graduate opportunity salary transparency.
- Types of salary disclosure.

**Related objectives:** RO-10, RO-06, RO-08, RO-09.

**Required variables:**

- Salary disclosure flag.
- Salary disclosure type.
- Salary text.
- Salary currency.
- Salary period.
- Salary type.
- Job-family assignment.
- Experience category.
- Location.
- Employment type.
- Graduate accessibility.

**Proposed analytical approach:**

Frequency distributions, disclosure proportions, cross-tabulations, chi-square tests, Fisher's exact or suitable alternatives, Cramér's V and confidence intervals.

**Important safeguard:**

Salary disclosure and salary amount are separate analytical dimensions.

An advertisement with no salary information must not be assigned a salary value of zero.

---

### RQ9 — Advertised Salary Patterns

**Research question:**

Among advertisements with usable salary information, how do advertised salary ranges differ across job family, experience and location?

**Research focus:**

- Advertised salary ranges.
- Salary by job family.
- Salary by experience category.
- Salary by location.
- Salary by work arrangement.
- Graduate opportunity remuneration.
- Salary distribution and variability.

**Related objectives:** RO-10, RO-06, RO-08, RO-09.

**Required variables:**

- Salary minimum.
- Salary maximum.
- Currency.
- Salary period.
- Gross/net status where disclosed.
- Salary type.
- Salary standardisation basis.
- Experience category.
- Job-family assignment.
- Geographic category.
- Work arrangement.

**Proposed analytical approach:**

Median, IQR, percentiles, distribution summaries, Mann–Whitney U, Kruskal–Wallis and regression where data comparability and assumptions justify them.

**Important safeguard:**

Only sufficiently comparable remuneration values may be included in common-basis salary comparisons.

The original salary wording and ranges must be preserved. A range must not automatically be reduced to its midpoint.

---

### RQ10 — Employment Arrangements and Working Conditions

**Research question:**

What employment arrangements and working conditions are advertised, and how do they vary across technology job families and geographic locations?

**Research focus:**

- Permanent employment.
- Fixed-term and temporary employment.
- Graduate programmes and positions.
- Internships.
- Learnerships.
- Apprenticeships.
- Part-time opportunities.
- Freelance and project-based contracts.
- Remote, hybrid and on-site arrangements.
- Contract duration.
- Working hours and shift requirements.
- Advertised benefits.
- Work-authorisation requirements.

**Related objectives:** RO-06, RO-09, RO-12.

**Required variables:**

- Employment type.
- Employment duration.
- Contract renewal.
- Graduate programme flag.
- Internship flag.
- Learnership flag.
- Apprenticeship flag.
- Part-time flag.
- Freelance flag.
- Project contract flag.
- Work arrangement.
- Working hours.
- Shift work.
- Benefits.
- Work-authorisation requirement.
- Location.
- Job-family assignment.

**Proposed analytical approach:**

Frequency distributions, proportions, cross-tabulations, chi-square tests, Fisher's exact or suitable alternatives, Cramér's V and numerical summaries for comparable contract durations.

**Important safeguard:**

Employment type, working hours, work arrangement and graduate accessibility must be treated as distinct concepts.

Benefits must be analysed individually rather than combined into a subjective employment-quality score.

---

### RQ11 — Temporal Patterns in Advertised Technology Requirements

**Research question:**

How do advertised technology skills, qualifications, experience requirements and opportunities change over the selected research period?

**Research focus:**

- Monthly advertisement volume.
- Monthly skills demand.
- Changes in skill categories.
- Qualification requirement trends.
- Experience and seniority patterns.
- Graduate opportunity patterns.
- Salary disclosure trends.
- Employment arrangement trends.
- Geographic changes.

**Related objectives:** RO-07, RO-08, RO-09, RO-10, RO-11.

**Required variables:**

- Publication date.
- Publication month.
- Publication quarter.
- Publication year.
- Skills.
- Qualifications.
- Experience.
- Job-family assignment.
- Graduate accessibility.
- Salary disclosure.
- Employment type.
- Location.
- Work arrangement.

**Proposed analytical approach:**

Monthly and quarterly frequency summaries, month-on-month changes, moving averages where useful, proportion trends, suitable regression and non-parametric trend methods where justified.

**Important safeguard:**

Temporal analysis must use original publication dates rather than collection dates.

Twelve monthly observations do not, by themselves, establish seasonality or justify complex forecasting.

---

### RQ12 — Multivariable Relationships Between Job Characteristics and Advertised Requirements

**Research question:**

What relationships exist between job family, experience, location and advertised skills, qualifications, salary information and employment requirements?

**Research focus:**

- Skill demand in relation to job characteristics.
- Qualification requirements in relation to job characteristics.
- Experience requirements in relation to job family and other characteristics.
- Salary disclosure in relation to job characteristics.
- Graduate accessibility in relation to job characteristics.
- Employment arrangements in relation to role and location.

**Related objectives:** RO-06, RO-07, RO-08, RO-09, RO-10, RO-11.

**Required variables:**

Potential explanatory variables:

- Job family.
- Experience category.
- Seniority.
- Location.
- Employer country.
- Work arrangement.
- Employment type.
- Qualification level.
- Graduate accessibility.
- Publication month or quarter.
- Employer characteristics where sufficiently complete.

Potential outcomes:

- Skill presence.
- Qualification requirement.
- Experience category.
- Salary disclosure.
- Advertised salary value.
- Graduate accessibility.
- Employment arrangement.

**Proposed analytical approach:**

Logistic regression, ordinal logistic regression, multinomial logistic regression and multiple regression or robust alternatives where appropriate.

**Important safeguard:**

Multivariable models must be selected according to variable types, sample adequacy, assumptions and interpretability.

Associations must not be interpreted as causal effects.

---

## 6. Approved Statistical Hypotheses

Seven hypotheses are approved for the project.

Each hypothesis contains a null hypothesis (H0) and an alternative hypothesis (H1).

The hypotheses are subject to statistical feasibility assessment before testing.

### H1 — Differences in Skill Distributions Across Job Families

**Related research question:** RQ2

**Research hypothesis:**

Skill distributions differ across the seven technology job families.

**Null hypothesis (H0):**

There is no statistically significant difference in the distribution of advertised skills across the seven technology job families.

**Alternative hypothesis (H1):**

There is a statistically significant difference in the distribution of advertised skills across the seven technology job families.

**Proposed analytical approach:**

- Cross-tabulations.
- Chi-square tests where appropriate.
- Suitable alternatives for sparse categorical data.
- Cramér's V.
- Confidence intervals where appropriate.

**Variables:**

- Job-family assignment.
- Standardised skill.
- Skill category.
- Skill requirement level.

**Interpretation boundary:**

The analysis investigates differences in advertised skill patterns, not differences in the competence of employees or applicants.

---

### H2 — Association Between Job Family and Qualification Requirements

**Related research question:** RQ4

**Research hypothesis:**

Qualification requirements are associated with technology job family.

**Null hypothesis (H0):**

Qualification requirements and job-family classification are statistically independent.

**Alternative hypothesis (H1):**

Qualification requirements and job-family classification are statistically associated.

**Proposed analytical approach:**

- Cross-tabulations.
- Chi-square test of independence.
- Fisher's exact or suitable alternatives for sparse data.
- Cramér's V.
- Ordinal methods where defensible.

**Variables:**

- Job-family assignment.
- Qualification level.
- Qualification requirement level.
- Qualification field.
- Formal qualification requirement status.

**Interpretation boundary:**

An association does not demonstrate that a particular job family causes a qualification requirement.

---

### H3 — Association Between Job Family and Experience Requirements

**Related research question:** RQ5

**Research hypothesis:**

Experience requirements are associated with technology job family.

**Null hypothesis (H0):**

Experience requirements and job-family classification are statistically independent.

**Alternative hypothesis (H1):**

Experience requirements and job-family classification are statistically associated.

**Proposed analytical approach:**

- Cross-tabulations.
- Chi-square test of independence.
- Suitable sparse-data alternatives.
- Cramér's V.
- Ordinal methods where justified.

**Variables:**

- Job-family assignment.
- Experience category.
- Experience requirement level.
- Seniority level.
- Minimum experience years.
- Maximum experience years.

**Interpretation boundary:**

Experience categories and seniority classifications must remain distinct.

---

### H4 — Geographic Distribution of Advertised Opportunities

**Related research question:** RQ7

**Research hypothesis:**

Advertised technology opportunities are not uniformly distributed across South African provinces.

**Null hypothesis (H0):**

The distribution of qualifying advertised opportunities is uniform across the nine South African provinces.

**Alternative hypothesis (H1):**

The distribution of qualifying advertised opportunities is not uniform across the nine South African provinces.

**Proposed analytical approach:**

- Provincial frequency distributions.
- Chi-square goodness-of-fit test where expected frequencies are appropriate.
- Suitable alternatives where assumptions are not satisfied.
- Geographic concentration summaries.
- Sensitivity analysis where source coverage differs materially.

**Variables:**

- Province.
- City.
- Location category.
- Advertisement identifier.
- Geographic eligibility.
- Work arrangement.

**Interpretation boundary:**

The test concerns the distribution within the accessible research dataset. It does not establish the distribution of all South African technology vacancies.

The uniformity benchmark is a statistical comparison, not an assumption that provinces should have equal labour-market opportunity.

Advertisements with multiple qualifying locations require documented counting rules to avoid double-counting unique opportunities.

---

### H5 — Differences in Salary Disclosure Rates Across Job Families

**Related research question:** RQ8

**Research hypothesis:**

Salary disclosure rates differ across technology job families.

**Null hypothesis (H0):**

Salary disclosure rates are equal across the seven technology job families.

**Alternative hypothesis (H1):**

At least one technology job family has a salary disclosure rate that differs from another.

**Proposed analytical approach:**

- Disclosure proportions.
- Cross-tabulations.
- Chi-square tests.
- Fisher's exact or suitable alternatives for sparse data.
- Cramér's V.
- Confidence intervals.

**Variables:**

- Salary disclosure flag.
- Salary disclosure type.
- Job-family assignment.
- Advertisement identifier.

**Interpretation boundary:**

Salary disclosure refers to whether remuneration information is advertised, not the amount employees actually receive.

---

### H6 — Differences in Advertised Salary Distributions

**Related research question:** RQ9

**Research hypothesis:**

Advertised salary distributions differ across job-family and experience groups.

**Null hypothesis (H0):**

There is no statistically significant difference in advertised salary distributions across the relevant job-family and experience groups being compared.

**Alternative hypothesis (H1):**

At least some relevant job-family and experience groups have statistically different advertised salary distributions.

**Proposed analytical approach:**

- Median and IQR comparisons.
- Percentile analysis.
- Mann–Whitney U for suitable two-group comparisons.
- Kruskal–Wallis for suitable multi-group comparisons.
- Regression where appropriate.
- Effect sizes and confidence intervals.

**Variables:**

- Standardised salary minimum.
- Standardised salary maximum.
- Salary currency.
- Salary period.
- Salary type.
- Experience category.
- Job-family assignment.

**Interpretation boundary:**

Only comparable salary observations may be used for common-basis comparisons.

Salary ranges, currency and remuneration periods must be handled consistently.

---

### H7 — Relationships Between Advertised Skills and Job Characteristics

**Related research question:** RQ12

**Research hypothesis:**

Advertised skills demand is associated with job characteristics, including job family, experience and location.

**Null hypothesis (H0):**

Advertised skills demand has no statistically significant association with the selected job characteristics.

**Alternative hypothesis (H1):**

Advertised skills demand has a statistically significant association with at least one selected job characteristic.

**Proposed analytical approach:**

- Cross-tabulations and association measures.
- Logistic regression for suitable skill-presence outcomes.
- Multivariable analysis where justified.
- Appropriate model diagnostics.
- Effect sizes and confidence intervals.

**Variables:**

- Skill presence.
- Job-family assignment.
- Experience category.
- Location.
- Work arrangement.
- Employment type.
- Other relevant job characteristics.

**Interpretation boundary:**

The analysis investigates associations in advertised requirements. It does not establish that job characteristics cause a particular skill to be requested.

---

## 7. Hypothesis Testing Standards

All seven hypotheses must follow the approved statistical methodology.

### 7.1 Significance Level

The approved significance level is:

**α = 0.05**

Tests will generally be two-sided unless a directional hypothesis has been explicitly justified in advance.

### 7.2 Reporting Requirements

Where appropriate, report:

- Test name.
- Test statistic.
- Degrees of freedom.
- Exact p-value.
- Adjusted p-value.
- Effect size.
- Confidence interval.
- Sample size.
- Relevant group sizes.
- Assumption and diagnostic results.
- Interpretation and limitations.

### 7.3 Multiple Testing

The Benjamini–Hochberg false discovery rate procedure is approved for suitable families of multiple exploratory tests.

Testing families must be defined and documented.

Both raw and adjusted p-values should be reported where applicable.

### 7.4 Effect Sizes

Effect sizes must accompany inferential results where appropriate.

Candidate measures include:

- Cramér's V.
- Cohen's d.
- Rank-based effect sizes.
- Eta-squared or suitable alternatives.
- Odds ratios.
- Pearson's r or Spearman's rho.
- Other method-appropriate measures.

### 7.5 Statistical and Practical Significance

Findings must distinguish between:

1. Statistical significance.
2. Magnitude of the observed difference or association.
3. Practical relevance to the research context.

A statistically significant result must not automatically be described as practically important.

### 7.6 Multi-Family Assignment Dependence

Because advertisements may belong to multiple job families, analyses comparing families must consider overlapping observations.

A conventional test must not treat expanded family-assignment rows as independent observations without justification.

Appropriate analytical approaches may include advertisement-level modelling, methods accounting for overlapping observations and sensitivity analyses.

The final method depends on the dataset and will be documented in the statistical methodology.

---

## 8. Research Question and Hypothesis Mapping

| Research Question | Related Objectives | Hypothesis |
|---|---|---|
| RQ1 — Overall skills demand | RO-06, RO-07 | Descriptive |
| RQ2 — Skills by job family | RO-05, RO-06, RO-07 | H1 |
| RQ3 — Skills relationships | RO-06, RO-07 | Descriptive / exploratory |
| RQ4 — Qualifications and certifications | RO-06, RO-08 | H2 |
| RQ5 — Experience and seniority | RO-06, RO-08 | H3 |
| RQ6 — Graduate opportunities | RO-06, RO-08, RO-09, RO-10 | Descriptive / exploratory |
| RQ7 — Geographic distribution | RO-09 | H4 |
| RQ8 — Salary disclosure | RO-10 | H5 |
| RQ9 — Advertised salary patterns | RO-10 | H6 |
| RQ10 — Employment arrangements | RO-06, RO-09, RO-12 | Descriptive / exploratory |
| RQ11 — Temporal patterns | RO-07, RO-08, RO-09, RO-10, RO-11 | Descriptive / exploratory |
| RQ12 — Multivariable relationships | RO-06, RO-07, RO-08, RO-09, RO-10, RO-11 | H7 |

Not every research question requires a formal hypothesis.

Descriptive and exploratory questions remain important research components and must not be forced into hypothesis testing.

---

## 9. Research Question Prioritisation

The approved research questions collectively define the project's analytical scope.

The following prioritisation is a proposed implementation aid and does not change their approved status.

### 9.1 Core Descriptive Analysis

- RQ1 — Overall skills demand.
- RQ2 — Skills by job family.
- RQ4 — Qualifications and certifications.
- RQ5 — Experience and seniority.
- RQ7 — Geographic distribution.
- RQ8 — Salary disclosure.
- RQ10 — Employment arrangements.

### 9.2 Comparative and Relationship Analysis

- RQ3 — Skills combinations.
- RQ6 — Graduate accessibility.
- RQ9 — Advertised salary patterns.

### 9.3 Advanced Analytical Investigation

- RQ11 — Temporal patterns.
- RQ12 — Multivariable relationships.

All questions remain part of the approved research design. The actual depth of analysis will depend on data adequacy and the relevant statistical assumptions.

---

## 10. Research Question Feasibility and Data Adequacy

Each research question must undergo a feasibility assessment before analysis.

Assessment should consider:

- Number of eligible unique advertisements.
- Completeness of required variables.
- Number of observations in relevant groups.
- Quality of classification and extraction.
- Source coverage.
- Duplicate handling.
- Missingness.
- Statistical assumptions.
- Independence and overlap.
- Suitability of the proposed analytical method.

### 10.1 Analysis Statuses

Each planned analysis must receive one of the following statuses:

| Status | Meaning |
|---|---|
| Completed | Analysis successfully performed. |
| Completed with limitations | Analysis performed, but limitations affect interpretation. |
| Descriptive only | Inferential analysis was not justified. |
| Modified | Original method replaced by a suitable alternative. |
| Not performed — insufficient data | Available data cannot support the analysis. |
| Not performed — assumption failure | Required assumptions could not be adequately addressed. |
| Pending review | Data or classification requires further validation. |

A non-significant statistical result must not be confused with insufficient data.

### 10.2 No Forced Hypothesis Testing

If the available dataset cannot support a planned test:

- Document the reason.
- Use a suitable descriptive alternative where useful.
- Identify the affected hypothesis.
- Explain any change in methodology.
- Avoid unsupported conclusions.

No artificial observations or fabricated findings may be introduced.

---

## 11. Research Interpretation and Reporting Rules

All findings must follow these principles:

1. Findings describe the accessible sample of qualifying job advertisements.
2. Non-probability sampling limitations must be disclosed.
3. Statistical association must not be interpreted as causation.
4. Advertisement volume must not be interpreted as actual hiring volume.
5. Advertised salary must not be interpreted as actual employee earnings.
6. Missing information must not be interpreted as absence.
7. Job-family overlap must be disclosed.
8. Denominators must accompany reported percentages.
9. Group sample sizes must accompany comparisons.
10. Statistical uncertainty and effect sizes must be reported where appropriate.
11. Exploratory findings must be labelled.
12. Negative, inconclusive and unsupported findings must be reported transparently.

---

## 12. Relationship to Other Project Documents

This document must be read alongside:

| Document | Relationship |
|---|---|
| Research Design | Defines the overall research framework, problem, aim, scope and period. |
| Sampling Strategy | Defines population, accessible population, sampling frame and sample construction. |
| Data Dictionary | Defines variables and their operationalisation. |
| Statistical Methodology | Defines statistical methods, assumptions, diagnostics and reporting. |
| Data Governance Plan | Defines data handling, permissions, privacy and publication rules. |

The research questions define what must be investigated. The data dictionary defines what information is required. The statistical methodology defines how the research questions will be analysed.

---

## 13. Confirmed Decisions and Unresolved Implementation Matters

### 13.1 Confirmed Decisions

The following are approved:

- Twelve research questions.
- Seven statistical hypotheses.
- Null and alternative formulations for all seven hypotheses.
- Dedicated graduate and entry-level research question.
- Advanced but defensible statistical ambition.
- Descriptive, comparative and multivariable research coverage.
- Significance level of 0.05.
- Two-sided testing unless justified otherwise.
- Benjamini–Hochberg FDR for appropriate multiple-testing families.
- Effect sizes and confidence intervals where appropriate.
- Analysis-specific adequacy.
- Explicit handling of multi-family assignment overlap.
- No compulsory predictive modelling.
- No fabricated results.

### 13.2 Unresolved Implementation Matters

The following remain subject to later approval or actual dataset assessment:

- Exact statistical tests for individual comparisons.
- Final variable grouping and category boundaries.
- Final regression specifications.
- Minimum adequacy criteria for individual analyses.
- Exact model diagnostics and parameters.
- Final technical libraries and versions.
- Final extraction and classification methods.

These matters must not be treated as final technical decisions merely because candidate methods are listed in this document.

---

## 14. Acceptance Criteria

| ID | Acceptance Criterion |
|---|---|
| RQH-AC-01 | All twelve approved research questions are included. |
| RQH-AC-02 | All seven approved hypotheses are included. |
| RQH-AC-03 | Every hypothesis includes a null and alternative formulation. |
| RQH-AC-04 | Each research question is linked to relevant research objectives. |
| RQH-AC-05 | Required variables are identified for every research question. |
| RQH-AC-06 | Proposed analytical approaches are documented without being treated as unconditional implementation decisions. |
| RQH-AC-07 | Multi-family advertisement overlap is explicitly addressed. |
| RQH-AC-08 | Graduate and entry-level accessibility are treated as distinct analytical concepts. |
| RQH-AC-09 | Salary disclosure and advertised remuneration are treated separately. |
| RQH-AC-10 | Geographic and international remote eligibility boundaries are preserved. |
| RQH-AC-11 | Temporal analysis uses the approved research period and publication-date rules. |
| RQH-AC-12 | Hypothesis-testing standards align with the approved Statistical Methodology. |
| RQH-AC-13 | Data adequacy and analysis-status rules are documented. |
| RQH-AC-14 | Non-probability sampling limitations and interpretation safeguards are included. |
| RQH-AC-15 | Confirmed decisions are distinguished from unresolved implementation matters. |
| RQH-AC-16 | Related methodology and governance documents are cross-referenced. |

---

## 15. Approval and Document Control

This document consolidates the approved B3 research questions and hypotheses for SkillSignal SA.

The research questions and hypotheses are fixed components of the approved research design unless formally amended through project change management.

The existence of an approved hypothesis does not guarantee that the available data will support statistical testing.

All findings must be determined from validated research evidence.

**Approval Status:** Approved — Section B Finalised

**Document Status:** Ready for incorporation into the SkillSignal SA repository following review and acceptance.