# SkillSignal SA — Statistical Methodology

| Document Attribute | Details |
|---|---|
| Project Name | SkillSignal SA |
| Project ID | SSA-001 |
| Document | Statistical Methodology |
| Document Location | `docs/02_Research_Methodology/Statistical_Methodology.md` |
| Version | 2.0 |
| Status | Approved — Section B Finalised |
| Research Orientation | Applied, quantitative and analytical |
| Research Period | 1 November 2025 – 31 October 2026 inclusive |
| Unit of Analysis | One unique job advertisement representing one advertised opportunity |
| Primary Analytical Focus | Descriptive, comparative, inferential and multivariable analysis where justified |
| Related Documents | Research Design; Research Questions and Hypotheses; Sampling Strategy; Data Dictionary; Data Governance Plan |

---

## 1. Purpose

This document defines the statistical methodology for analysing the SkillSignal SA job advertisement dataset.

It establishes the approved analytical principles, descriptive measures, comparative methods, hypothesis-testing standards, potential multivariable techniques, diagnostic procedures, effect-size reporting, sample-adequacy requirements and reproducibility standards.

The methodology supports the investigation of:

- Advertised technical and professional skills.
- Differences across technology job families.
- Skills that commonly occur together.
- Educational qualification and certification requirements.
- Experience and seniority requirements.
- Graduate and entry-level accessibility.
- Geographic distribution of opportunities.
- Salary disclosure and advertised remuneration.
- Employment types and working arrangements.
- Temporal patterns in advertised requirements.
- Relationships between job characteristics and advertised requirements.

The purpose is to generate evidence-based labour-market intelligence from job advertisements, not to infer actual hiring outcomes or claim complete coverage of the South African technology labour market.

---

## 2. Statistical Analysis Principles

All statistical analysis must follow these principles.

### 2.1 Descriptive analysis first

The dataset must be understood before inferential or multivariable analysis is attempted.

Descriptive analysis establishes:

- Sample composition.
- Variable distributions.
- Missingness.
- Category representation.
- Potential outliers.
- Data-quality concerns.
- Suitability for further analysis.

### 2.2 Research-question alignment

Every analysis must support an approved research question, objective or hypothesis.

Analysis must not be conducted solely to produce complex statistics or visually impressive results.

### 2.3 Method suitability

Methods must be selected according to:

- Variable types.
- Data distributions.
- Sample size.
- Group sizes.
- Missingness.
- Independence assumptions.
- Statistical assumptions.
- Data quality.
- Practical interpretability.

### 2.4 Statistical integrity

The project must:

- Report actual results only.
- Avoid fabricated findings.
- Avoid unsupported population-level claims.
- Distinguish statistical significance from practical significance.
- Report uncertainty where appropriate.
- Disclose limitations.
- Avoid interpreting association as causation.

### 2.5 Reproducibility

All material analytical transformations, calculations, statistical tests and reporting outputs must be reproducible through documented procedures.

### 2.6 Analysis-specific adequacy

A dataset may support descriptive analysis but not a particular inferential test or multivariable model.

No single global sample-size threshold will determine whether every analysis is permitted.

### 2.7 Analytical workflow

The approved analytical workflow is:

1. Data-quality assessment.
2. Descriptive analysis.
3. Comparative analysis.
4. Inferential analysis where justified.
5. Multivariable analysis where justified.
6. Interpretation and limitation assessment.
7. Reproducibility and reporting review.

---

## 3. Data Preparation for Statistical Analysis

### 3.1 Analytical dataset

The analytical dataset must be derived from the canonical advertisement records established through the approved sampling strategy.

Duplicate publication instances must not inflate unique advertisement counts.

### 3.2 Data preparation requirements

Before analysis:

- Validate advertisement eligibility.
- Confirm canonical-record status.
- Review job-family assignments.
- Standardise relevant categories.
- Validate numeric values.
- Review date fields.
- Assess missingness.
- Identify conflicting evidence.
- Check duplicate relationships.
- Confirm variable definitions.
- Record dataset and taxonomy versions.

### 3.3 Multi-family assignment

Advertisements may belong to multiple job families.

Consequently:

- Family-specific groups may overlap.
- Family counts may exceed the total number of unique advertisements.
- Family-level percentages may use different denominators.
- Comparisons must disclose the overlap.
- Statistical independence assumptions must be considered.

Where a test requires independent observations, the analysis must assess whether overlapping family assignments invalidate that assumption.

### 3.4 Missing data

Missing information must not be converted into a negative response.

Examples:

- Missing salary is not zero salary.
- Missing experience is not zero experience.
- Missing qualification information does not indicate no qualification requirement.
- Missing location information does not establish remote work.

Each analysis must define how missing, unclear, conflicting and unassessed observations are handled.

### 3.5 Analytical eligibility

A record may be eligible for the overall dataset but unsuitable for a specific analysis because the required variable is missing or unreliable.

Analysis-specific denominators must reflect this distinction.

---

## 4. Descriptive Statistical Methods

### 4.1 Approved measures

The following descriptive measures may be used where appropriate:

| Measure | Application |
|---|---|
| Frequency | Number of advertisements or relationships in a category. |
| Percentage | Proportion relative to a stated denominator. |
| Proportion | Share of observations meeting a defined condition. |
| Mean | Arithmetic average for suitable numeric variables. |
| Median | Central observation, particularly useful for skewed distributions. |
| Mode | Most frequently occurring value or category. |
| Minimum and maximum | Observed range. |
| Standard deviation | Dispersion around the mean. |
| Interquartile range | Dispersion around the median. |
| Percentiles | Distributional position. |
| Cross-tabulation | Comparison across categorical variables. |
| Missingness analysis | Proportion and pattern of unavailable information. |
| Unique counts | Distinct advertisements, employers or relationships. |

### 4.2 Application areas

Descriptive statistics will be applied to:

- Overall advertisement composition.
- Job-family distribution.
- Technical and professional skills.
- Skill requirement levels.
- Qualification and certification requirements.
- Experience and seniority.
- Graduate accessibility.
- Geographic distribution.
- Salary disclosure.
- Advertised remuneration.
- Employment type.
- Work arrangement.
- Temporal distribution.

### 4.3 Denominator requirements

Every reported percentage must state or clearly identify its denominator.

For example:

\[
\text{Skill prevalence} =
\frac{\text{Unique eligible advertisements containing the skill}}
{\text{Eligible unique advertisements in the relevant group}}
\times 100
\]

\[
\text{Salary disclosure rate} =
\frac{\text{Advertisements with disclosed remuneration}}
{\text{Advertisements assessed for salary disclosure}}
\times 100
\]

\[
\text{Graduate accessibility proportion} =
\frac{\text{Graduate-specific or entry-level accessible advertisements}}
{\text{Advertisements assessed for graduate accessibility}}
\times 100
\]

### 4.4 Interpretation safeguards

- Report observation counts alongside percentages.
- Use medians and interquartile ranges for skewed numerical distributions where appropriate.
- Distinguish zero values from missing values.
- Avoid comparing raw counts without considering group sizes.
- Disclose overlapping categories.
- Do not interpret descriptive patterns as proof of causation.

---

## 5. Skills Demand Analysis

**Related research questions:** RQ1, RQ2, RQ3, RQ6 and RQ12.

### 5.1 Analysis objectives

Investigate:

- Most frequently advertised technical skills.
- Most frequently advertised professional skills.
- Skill demand across seven job families.
- Required versus preferred skills.
- Skill-category distributions.
- Skills requested in graduate and entry-level opportunities.
- Commonly co-occurring skill combinations.
- Associations between skills and job characteristics.

### 5.2 Descriptive measures

Use:

- Advertisement-level skill frequencies.
- Skill prevalence percentages.
- Family-level skill distributions.
- Technical versus professional skill comparisons.
- Requirement-level distributions.
- Skill-category frequencies.
- Graduate versus non-graduate accessible skill profiles.

Top 10, top 20 or top 30 skills may be reported where the available data supports a meaningful ranking.

The number of displayed skills must not be treated as a predetermined research finding.

### 5.3 Comparative analysis

Potential comparisons include:

- Skills across job families.
- Technical versus professional skill requirements.
- Required versus preferred skills.
- Graduate-specific versus other opportunities.
- Skills across seniority categories.

Potential statistical methods:

- Chi-square test of independence.
- Fisher's exact test where expected frequencies are insufficient for a suitable chi-square approximation.
- Cramér's V for association strength.
- Confidence intervals for relevant proportions.

The suitability of each method must be assessed against the actual data structure.

### 5.4 Skill counting

Each unique standardised skill counts once per canonical advertisement for advertisement-level prevalence.

Repeated mentions within one advertisement must not inflate the frequency.

### 5.5 Multi-family interpretation

Family-level comparisons must account for advertisements assigned to multiple families.

Results must not imply that job-family groups are mutually exclusive where they are not.

### 5.6 Interpretation

Skill frequency indicates what employers advertise as requirements or preferences.

It does not directly measure:

- Actual employee capability.
- Actual hiring demand.
- Skill shortages.
- Candidate supply.
- Employer satisfaction.
- Employment outcomes.

---

## 6. Skill Co-occurrence Analysis

**Related research question:** RQ3.

### 6.1 Purpose

Identify skills that commonly appear together in the same advertisement.

### 6.2 Candidate measures

| Measure | Definition |
|---|---|
| Pair frequency | Number of unique advertisements containing both skills. |
| Support | Proportion of eligible advertisements containing both skills. |
| Confidence | Proportion of advertisements containing skill A that also contain skill B. |
| Jaccard similarity | Intersection of advertisements containing both skills divided by the union of advertisements containing either skill. |
| Lift | Observed co-occurrence relative to the expected co-occurrence under independence. |

### 6.3 Formulas

For skills A and B:

\[
\text{Support}(A,B)=P(A\cap B)
\]

\[
\text{Confidence}(A\rightarrow B)=
\frac{P(A\cap B)}{P(A)}
\]

\[
\text{Lift}(A,B)=
\frac{P(A\cap B)}{P(A)P(B)}
\]

\[
\text{Jaccard}(A,B)=
\frac{|A\cap B|}{|A\cup B|}
\]

### 6.4 Interpretation

- Lift greater than 1 indicates positive co-occurrence relative to independence.
- Lift equal to 1 indicates the independence benchmark under the measure's assumptions.
- Lift below 1 indicates lower co-occurrence than expected under independence.

### 6.5 Potential outputs

- Skill-pair frequency tables.
- Co-occurrence matrices.
- Job-family-specific skill combinations.
- Association-rule summaries.
- Skill network visualisations.

### 6.6 Safeguards

- Use unique advertisement-skill relationships.
- Establish support and confidence thresholds after inspecting the pilot data.
- Avoid overemphasising rare combinations with high lift.
- Report the underlying observation counts.
- Do not interpret co-occurrence as causation.
- Consider the effect of job-family overlap.
- Document the denominator used for each measure.

---

## 7. Qualification and Certification Analysis

**Related research question:** RQ4.

### 7.1 Analysis objectives

Investigate:

- Educational qualification levels requested.
- Qualification fields.
- Required versus preferred qualifications.
- Professional certification requirements.
- Certification providers and types.
- Acceptance of equivalent experience.
- Differences across job families.
- Qualification patterns in graduate and entry-level opportunities.

### 7.2 Descriptive methods

Use:

- Frequency distributions.
- Percentages.
- Qualification-level comparisons.
- Certification-category summaries.
- Required/preferred distributions.
- Cross-tabulations.

### 7.3 Comparative methods

Potential methods include:

- Chi-square test of independence.
- Fisher's exact test.
- Cramér's V.
- Confidence intervals for relevant proportions.
- Ordinal methods where the qualification categories have a defensible ordering.

### 7.4 Interpretation safeguards

- Distinguish qualifications from certifications.
- Distinguish required from preferred.
- Preserve alternative qualification pathways.
- Missing information must not be interpreted as no requirement.
- Avoid implying that an advertised qualification is universally required across the profession.
- Consider the impact of missing and unclear qualification wording.

---

## 8. Experience and Graduate Accessibility Analysis

**Related research questions:** RQ5 and RQ6.

### 8.1 Analysis objectives

Investigate:

- Experience requirements across job families.
- Experience requirements by seniority.
- Entry-level and graduate accessibility.
- Internship and equivalent-experience acceptance.
- Graduate skill requirements.
- Qualification and experience expectations in graduate opportunities.
- Relationships between experience and other advertised characteristics.

### 8.2 Descriptive methods

Use:

- Experience-category frequencies.
- Numeric experience summaries where reliable.
- Median and interquartile range.
- Minimum and maximum where meaningful.
- Seniority distributions.
- Graduate accessibility proportions.
- Cross-tabulations.

### 8.3 Comparative methods

Potential methods include:

- Chi-square test of independence.
- Fisher's exact test.
- Mann–Whitney U test.
- Kruskal–Wallis test.
- Ordinal analysis where defensible.
- Confidence intervals.
- Suitable effect-size measures.

### 8.4 Graduate accessibility definitions

Maintain the distinction between:

- Graduate-specific.
- Entry-level accessible.
- Experience required.
- Not established.

Graduate-specific and entry-level accessible opportunities may overlap with other employment or experience classifications.

### 8.5 Interpretation safeguards

- Missing experience does not mean zero experience.
- Vague wording must not be converted into unsupported numeric values.
- Seniority is not interchangeable with years of experience.
- Internship acceptance must be distinguished from general professional experience.
- Graduate programmes must not automatically be classified as accessible to every graduate.
- Comparisons must disclose overlapping classifications.

---

## 9. Geographic Analysis

**Related research question:** RQ7.

### 9.1 Analysis objectives

Investigate:

- Advertisement distribution across nine provinces.
- Major cities and other locations.
- Geographic variation in job-family demand.
- Graduate accessibility by location.
- Work arrangement by location.
- Skill requirements by location.
- Advertised remuneration by location where comparable.
- Domestic opportunities versus qualifying international remote opportunities.

### 9.2 Descriptive methods

Use:

- Frequency distributions.
- Proportions.
- Provincial rankings.
- City-level summaries where adequate.
- Geographic concentration summaries.
- Cross-tabulations.
- Maps where geographic information is sufficiently reliable.

### 9.3 Comparative methods

Potential methods include:

- Chi-square test of independence.
- Fisher's exact test.
- Cramér's V.
- Median and interquartile range.
- Kruskal–Wallis test for suitable numerical comparisons.
- Confidence intervals for proportions.

### 9.4 Two geographic views

The analysis must distinguish:

1. **Opportunity geography:** Where the work is advertised or performed.
2. **Employer geography:** Where the employer is based.

These are not interchangeable.

### 9.5 Geographic safeguards

- Do not infer province from employer headquarters.
- Preserve multi-location advertisements.
- Avoid assigning remote opportunities to an unsupported physical location.
- Keep qualifying international remote opportunities separate.
- Do not assume all remote opportunities are available to South African candidates.
- Report missing and unspecified geographic information.
- Avoid detailed comparisons where group counts are insufficient.

---

## 10. Salary Transparency and Remuneration Analysis

**Related research questions:** RQ8 and RQ9.

### 10.1 Two-track analytical approach

Salary analysis must be divided into two distinct tracks.

**Track A — Salary transparency**

Investigates whether and how advertisements disclose remuneration.

**Track B — Advertised remuneration**

Investigates the remuneration amounts and ranges where sufficiently comparable numeric information is available.

### 10.2 Track A: Salary transparency

Analyse:

- Overall salary disclosure rate.
- Exact amount disclosure.
- Salary-range disclosure.
- Starting or maximum amount disclosure.
- Negotiable salary without an amount.
- Commission disclosure.
- Stipend or allowance disclosure.
- Benefits-only disclosure.
- Non-disclosure.

Potential comparisons:

- Job family.
- Experience category.
- Seniority.
- Location.
- Employment type.
- Graduate accessibility.

Potential methods:

- Frequencies and proportions.
- Cross-tabulations.
- Chi-square test of independence.
- Fisher's exact test.
- Cramér's V.
- Confidence intervals for proportions.

### 10.3 Track B: Advertised remuneration

Where comparable numeric values are available, analyse:

- Median remuneration.
- Interquartile range.
- Percentiles.
- Minimum and maximum.
- Distribution across job families.
- Differences by experience.
- Differences by geography.
- Differences by employment type.

Potential methods:

- Descriptive distribution summaries.
- Mann–Whitney U test.
- Kruskal–Wallis test.
- Regression where justified by data quality and assumptions.
- Suitable effect sizes and confidence intervals.

### 10.4 Salary data safeguards

- Preserve original wording.
- Preserve original currency and period.
- Distinguish gross and net values where stated.
- Do not replace ranges with midpoints.
- Do not mix hourly, daily, monthly and annual amounts without a defensible conversion.
- Do not mix salary and commission or benefits as equivalent numerical measures.
- Do not infer undisclosed remuneration.
- Do not convert currency without a documented exchange-rate source, rate and reference date.
- Annualisation to ZAR may only occur where the original remuneration basis and conversion method are defensible.
- Exclude incomparable values from numerical comparisons while retaining them for transparency analysis where appropriate.

### 10.5 Interpretation

Salary disclosure rates and advertised salary distributions measure different things.

A high disclosure rate does not necessarily imply higher remuneration.

A lack of numerical salary information must not be interpreted as evidence of low remuneration.

---

## 11. Employment Type and Working-Condition Analysis

**Related research question:** RQ10.

### 11.1 Analysis objectives

Investigate:

- Employment-type distribution.
- Permanent versus non-permanent opportunities.
- Graduate programmes and internships.
- Learnerships and apprenticeships.
- Part-time and freelance opportunities.
- Project-based contracts.
- Remote, hybrid and on-site arrangements.
- Contract duration.
- Working hours and shifts.
- Advertised benefits.
- Work-authorisation requirements.

### 11.2 Descriptive methods

Use:

- Frequency distributions.
- Percentages.
- Cross-tabulations.
- Contract-duration summaries.
- Work-arrangement distributions.
- Benefits-category frequencies.

### 11.3 Comparative methods

Potential methods include:

- Chi-square test of independence.
- Fisher's exact test.
- Cramér's V.
- Median and interquartile range for suitable duration variables.
- Non-parametric comparisons where justified.

### 11.4 Interpretation safeguards

- Employment type and work arrangement must remain separate.
- Benefits must be analysed individually or by documented categories.
- Missing benefits information does not mean no benefits.
- No composite employment-quality score is approved.
- Do not infer job security or employment quality from contract labels alone.

---

## 12. Hypothesis Testing Framework

### 12.1 Approved significance standard

The default significance level is:

\[
\alpha = 0.05
\]

Tests will be two-sided unless a directional test is separately justified and documented.

### 12.2 Reporting requirements

Where inferential testing is performed, report:

- Null hypothesis.
- Alternative hypothesis.
- Statistical method.
- Sample size.
- Group sizes.
- Test statistic.
- Exact p-value where available.
- Effect size.
- Confidence interval where appropriate.
- Assumption assessment.
- Interpretation.
- Analytical limitations.

### 12.3 Multiple testing

For suitable families of exploratory tests, apply the Benjamini–Hochberg false discovery rate procedure.

Report both:

- Raw p-values.
- Adjusted p-values.

The relevant test family and adjustment procedure must be documented.

Multiple-testing correction must not be applied mechanically to unrelated tests without a reasoned definition of the test family.

### 12.4 Overlapping observations

The analysis must assess whether advertisements assigned to multiple job families violate independence assumptions.

Where appropriate, use an alternative method or restrict the analysis to a defensible subset.

### 12.5 Approved hypotheses

| ID | Research Focus | Null Hypothesis (H0) | Alternative Hypothesis (H1) |
|---|---|---|---|
| H1 | Skills across job families | Advertised skill distributions do not differ across job families. | Advertised skill distributions differ across job families. |
| H2 | Qualifications and job family | Qualification requirements are independent of job family. | Qualification requirements are associated with job family. |
| H3 | Experience and job family | Experience requirements are independent of job family. | Experience requirements are associated with job family. |
| H4 | Provincial distribution | The distribution of qualifying advertised opportunities across provinces is uniform. | The distribution is not uniform. |
| H5 | Salary disclosure | Salary disclosure rates are equal across job families. | Salary disclosure rates differ across job families. |
| H6 | Salary distributions | Advertised salary distributions do not differ across job-family and experience groups. | At least some comparable salary distributions differ across these groups. |
| H7 | Skills and job characteristics | Advertised skills demand is not associated with job characteristics. | Advertised skills demand is associated with one or more job characteristics. |

### 12.6 Hypothesis-specific safeguards

- H1: Account for overlapping job-family assignments.
- H2: Preserve required, preferred and unspecified qualification categories.
- H3: Distinguish missing experience from no experience required.
- H4: The uniform distribution is a statistical benchmark, not an assumption that each province should have equal labour-market demand.
- H5: Use advertisements assessed for salary disclosure and disclose denominators.
- H6: Include only sufficiently comparable remuneration values and groups.
- H7: Interpret association as association, not causation.

Failure to reject a null hypothesis must not be reported as proof that no relationship or difference exists.

---

## 13. Multivariable Analysis

**Related research question:** RQ12.

### 13.1 Purpose

Multivariable analysis may be used to investigate relationships between job characteristics and advertised requirements while accounting for multiple variables.

It is intended to support explanatory statistical analysis where appropriate.

Predictive modelling is not mandatory.

### 13.2 Candidate outcome variables

Potential outcomes include:

- Presence of a selected advertised skill.
- Qualification requirement category.
- Experience requirement category.
- Salary disclosure.
- Comparable advertised salary value.
- Graduate accessibility.
- Employment type.

### 13.3 Candidate explanatory variables

Potential predictors include:

- Job family.
- Experience.
- Seniority.
- Province.
- Employer country.
- Work arrangement.
- Employment type.
- Qualification category.
- Graduate accessibility.
- Publication month or quarter.
- Employer characteristics where reliable.

Only variables with adequate data quality and a defensible analytical relationship should be included.

### 13.4 Candidate methods

| Method | Potential application |
|---|---|
| Binary logistic regression | Binary outcomes such as salary disclosed or a selected skill present. |
| Ordinal logistic regression | Outcomes with a defensible ordered structure. |
| Multinomial logistic regression | Outcomes with multiple unordered categories. |
| Multiple linear regression | Suitable continuous outcomes where assumptions can be supported. |
| Robust alternatives | Where ordinary model assumptions are not sufficiently supported. |

### 13.5 Model evaluation

Where a model is fitted, evaluate as appropriate:

- Coefficients.
- Odds ratios.
- Confidence intervals.
- Model fit.
- Multicollinearity.
- Residual behaviour.
- Linearity assumptions.
- Heteroscedasticity.
- Influential observations.
- Separation.
- Calibration.
- Discrimination.
- ROC-AUC where appropriate.

### 13.6 Model development hierarchy

Where justified, structure analysis into:

1. Core model.
2. Adjusted model.
3. Exploratory model.

Each additional model must have a clear analytical reason.

### 13.7 Safeguards

- Do not fit a model merely because the dataset contains multiple variables.
- Avoid excessive predictors relative to available observations.
- Consider sparse categories.
- Consider overlap between job-family assignments.
- Avoid interpreting model coefficients causally.
- Report model limitations.
- Do not claim predictive performance from training results alone.
- Predictive modelling remains optional and is not an acceptance requirement.

---

## 14. Temporal Analysis

**Related research question:** RQ11.

### 14.1 Analysis objectives

Investigate changes or patterns in:

- Advertised skills.
- Qualification requirements.
- Experience requirements.
- Job-family distributions.
- Graduate accessibility.
- Salary disclosure.
- Employment arrangements.
- Geographic distribution.

### 14.2 Time basis

Publication date is the controlling date for temporal analysis.

Collection date must not be substituted for publication date.

### 14.3 Candidate methods

- Monthly frequencies.
- Quarterly summaries.
- Month-on-month comparisons.
- Monthly proportions.
- Moving averages where appropriate.
- Regression-based trend analysis where justified.
- Mann–Kendall trend testing where its assumptions and data structure are appropriate.

### 14.4 Temporal safeguards

- The approved research period contains twelve monthly periods.
- Twelve monthly observations do not automatically establish seasonality.
- Twelve monthly observations do not automatically justify complex forecasting.
- Small monthly counts must be reported with appropriate caution.
- Missing historical advertisements must be acknowledged.
- Changes in source availability may influence observed patterns.
- Reposts must not inflate opportunity counts.
- Do not infer long-term labour-market trends from a single twelve-month research window.

---

## 15. Statistical Assumptions and Diagnostics

### 15.1 Purpose

Before applying inferential or multivariable methods, assess whether the data supports the selected method.

### 15.2 Categorical-data diagnostics

Assess:

- Expected cell frequencies.
- Sparse categories.
- Independence of observations.
- Overlapping group membership.
- Missingness.
- Category definitions.
- Adequacy of contingency tables.

Where chi-square assumptions are unsuitable, consider Fisher's exact test or another justified alternative.

### 15.3 Numerical-data diagnostics

Assess:

- Distribution shape.
- Skewness.
- Outliers.
- Variance.
- Independence.
- Measurement reliability.
- Comparability of units.

Use non-parametric alternatives where justified.

### 15.4 Regression diagnostics

Where regression is performed, assess relevant assumptions, including:

- Multicollinearity.
- Residual behaviour.
- Linearity where applicable.
- Heteroscedasticity.
- Influential observations.
- Model specification.
- Separation in categorical models.
- Calibration where appropriate.

### 15.5 Diagnostic failure

If assumptions cannot be adequately addressed:

- Document the failure.
- Consider a suitable alternative.
- Simplify the analysis only where justified.
- Use descriptive analysis if necessary.
- Mark the original analysis as modified or not performed.

A method must not be changed merely to obtain a statistically significant result.

---

## 16. Effect Sizes and Confidence Intervals

### 16.1 Purpose

Statistical significance alone does not describe the magnitude or practical importance of a result.

Effect sizes and confidence intervals must be reported where appropriate.

### 16.2 Candidate effect-size measures

| Measure | Potential application |
|---|---|
| Cramér's V | Association between categorical variables. |
| Cohen's d | Standardised difference between suitable numerical groups. |
| Rank-based effect measures | Non-parametric group comparisons. |
| Eta-squared | Suitable variance-based comparisons. |
| Odds ratio | Logistic regression and related comparisons. |
| Pearson correlation | Suitable linear relationships between numerical variables. |
| Spearman correlation | Rank-based or monotonic relationships. |
| Jaccard similarity | Skill-set overlap. |
| Lift | Skill co-occurrence association. |
| Proportion difference | Differences between relevant proportions. |

### 16.3 Confidence intervals

Use 95% confidence intervals where appropriate.

The interval method must be suitable for the statistic and data structure.

### 16.4 Interpretation

- Report effect sizes alongside p-values.
- Interpret magnitude in context.
- Distinguish statistical significance from practical significance.
- Avoid arbitrary universal effect-size thresholds.
- A statistically significant result may have limited practical importance.
- A non-significant result may still have an uncertain or meaningful estimated effect.

---

## 17. Sample Adequacy and Method Selection

### 17.1 Approved principle

There is no single global minimum sample size for all analyses.

Each analysis must be assessed independently.

### 17.2 Adequacy considerations

Consider:

- Total eligible observations.
- Group sizes.
- Missingness.
- Category distribution.
- Data quality.
- Measurement reliability.
- Statistical assumptions.
- Independence.
- Number of explanatory variables.
- Practical interpretability.

### 17.3 Alternative methods

When data is insufficient, possible responses include:

1. Retain descriptive analysis only.
2. Use an appropriate exact test.
3. Reduce model complexity.
4. Combine categories only when conceptually justified.
5. Conduct sensitivity analysis.
6. Suppress unsupported comparisons.
7. Mark the analysis as not performed.

Categories must never be combined solely to obtain statistical significance.

### 17.4 Analysis status framework

| Status | Definition |
|---|---|
| Completed | Analysis performed using an appropriate method. |
| Completed with limitations | Analysis performed with material limitations. |
| Descriptive only | Inferential analysis was not justified. |
| Modified | Original method replaced with a suitable alternative. |
| Not performed — insufficient data | Available observations do not support the analysis. |
| Not performed — assumption failure | Required assumptions could not be adequately addressed. |
| Pending review | Data or classification requires additional validation. |

### 17.5 Sensitivity analysis

Where meaningful, perform sensitivity analysis to determine whether findings materially change under reasonable alternative assumptions or data-handling decisions.

Document the assumptions and results.

---

## 18. Reporting and Reproducibility

### 18.1 Minimum reporting requirements

Each material analysis must document:

- Research question or hypothesis.
- Dataset version.
- Relevant variables.
- Eligibility criteria.
- Total and group sample sizes.
- Missing-data handling.
- Statistical method.
- Assumption checks.
- Test parameters.
- Statistical results.
- Effect size.
- Confidence interval where appropriate.
- Interpretation.
- Limitations.
- Analysis status.

### 18.2 Reproducibility requirements

Maintain:

- Version-controlled analysis scripts or notebooks.
- Documented data transformations.
- Dataset version references.
- Taxonomy versions.
- Package and dependency versions.
- Random seeds where stochastic methods are used.
- Reproducible statistical outputs.
- Traceable reporting calculations.

### 18.3 Output categories

Analytical outputs may include:

**Intermediate outputs**
- Cleaned analytical datasets.
- Validation summaries.
- Classification summaries.
- Missingness reports.

**Statistical outputs**
- Frequency tables.
- Cross-tabulations.
- Test results.
- Regression summaries.
- Effect-size summaries.
- Confidence intervals.

**Visual outputs**
- Bar charts.
- Stacked charts.
- Distribution plots.
- Heatmaps.
- Skill co-occurrence networks.
- Geographic maps.
- Temporal trend charts.

**Publication outputs**
- Research findings.
- Dashboard indicators.
- Methodological explanations.
- Limitations.
- Aggregate labour-market insights.

### 18.4 Consistency across outputs

The research publication, statistical summaries and interactive dashboard must use consistent definitions, denominators and dataset versions.

Differences must be documented rather than silently reconciled.

### 18.5 Restricted data

Public outputs must not expose restricted raw advertisements or personal information.

Synthetic demonstration data, if used, must be clearly identified as synthetic.

---

## 19. Research Question and Method Mapping

The following table links each approved research question to its primary analytical approach.

| Research Question | Analytical Focus | Primary Methods |
|---|---|---|
| RQ1 | Most frequently advertised skills | Frequencies, proportions, rankings, confidence intervals |
| RQ2 | Skill demand across job families | Cross-tabulations, chi-square/Fisher's exact, Cramér's V |
| RQ3 | Skills commonly occurring together | Pair frequencies, support, confidence, lift, Jaccard, networks |
| RQ4 | Qualifications and certifications | Frequencies, proportions, cross-tabulations, chi-square/Fisher's exact |
| RQ5 | Experience and seniority requirements | Distributions, medians, cross-tabulations, non-parametric comparisons |
| RQ6 | Graduate and entry-level accessibility | Proportions, skill profiles, cross-tabulations, suitable association tests |
| RQ7 | Geographic distribution | Frequencies, proportions, maps, cross-tabulations, suitable comparisons |
| RQ8 | Salary disclosure | Disclosure rates, proportions, cross-tabulations, chi-square/Fisher's exact |
| RQ9 | Advertised salary patterns | Medians, IQR, percentiles, non-parametric comparisons, regression where justified |
| RQ10 | Employment types and conditions | Frequencies, proportions, cross-tabulations, suitable comparisons |
| RQ11 | Temporal patterns | Monthly/quarterly summaries, proportions, trend analysis where justified |
| RQ12 | Relationships between job characteristics and requirements | Multivariable methods where justified |

This mapping is a methodological framework, not a commitment to perform every candidate test.

---

## 20. Confirmed Decisions and Unresolved Implementation Matters

### 20.1 Confirmed decisions

The following are approved:

- Descriptive analysis before inferential analysis.
- Research-question-aligned statistical methods.
- Method selection based on variable types and assumptions.
- Analysis-specific sample adequacy.
- Descriptive and comparative methods.
- Skills and co-occurrence analysis.
- Qualification and experience analysis.
- Geographic analysis.
- Two-track salary analysis.
- Employment-condition analysis.
- Alpha level of 0.05.
- Two-sided tests unless justified otherwise.
- Effect-size and confidence-interval reporting.
- Benjamini–Hochberg adjustment for suitable exploratory test families.
- Candidate multivariable methods.
- Temporal analysis safeguards.
- Statistical diagnostic requirements.
- Sensitivity analysis where meaningful.
- Reproducibility and reporting requirements.
- No mandatory predictive modelling.

### 20.2 Unresolved implementation matters

The following remain subject to data assessment and later implementation decisions:

- Exact statistical tests for individual final comparisons.
- Numerical sample-adequacy thresholds.
- Final regression specifications.
- Salary standardisation and currency-conversion implementation.
- Co-occurrence support and confidence thresholds.
- Final grouping and category-consolidation rules.
- Statistical software and library selection.
- Dashboard and BI implementation.
- Final visualisation specifications.

These decisions must be based on the actual dataset, variable quality and statistical suitability.

---

## 21. Acceptance Criteria

| ID | Acceptance Criterion |
|---|---|
| SM-AC-01 | Statistical principles and analytical workflow are documented. |
| SM-AC-02 | Descriptive statistical methods are defined. |
| SM-AC-03 | Denominator and missing-data rules are explicit. |
| SM-AC-04 | Skills demand analysis is documented. |
| SM-AC-05 | Skill co-occurrence measures and formulas are included. |
| SM-AC-06 | Qualification and certification analysis is documented. |
| SM-AC-07 | Experience and graduate accessibility analysis is documented. |
| SM-AC-08 | Geographic analysis is documented. |
| SM-AC-09 | Salary transparency and remuneration are treated separately. |
| SM-AC-10 | Employment and working-condition analysis is documented. |
| SM-AC-11 | All seven approved hypotheses and H0/H1 statements are included. |
| SM-AC-12 | Significance level and multiple-testing requirements are defined. |
| SM-AC-13 | Multivariable methods are conditional on suitability. |
| SM-AC-14 | Predictive modelling is not mandatory. |
| SM-AC-15 | Temporal analysis limitations are explicit. |
| SM-AC-16 | Statistical assumptions and diagnostics are documented. |
| SM-AC-17 | Effect sizes and confidence intervals are addressed. |
| SM-AC-18 | Analysis-specific adequacy and alternative approaches are defined. |
| SM-AC-19 | Reporting and reproducibility requirements are included. |
| SM-AC-20 | All twelve research questions are mapped to analytical approaches. |
| SM-AC-21 | Confirmed decisions are distinguished from unresolved implementation matters. |

---

## 22. Approval and Document Control

This document consolidates the approved B8.1–B8.17 statistical methodology decisions.

It is the controlling analytical framework for SkillSignal SA.

The actual statistical methods applied must be selected and documented after data acquisition and quality assessment.

No statistical result, relationship, trend or hypothesis outcome may be presented as established until supported by the collected and validated dataset.

**Approval Status:** Approved — Section B Finalised

**Document Status:** Ready for incorporation into the SkillSignal SA repository following review and acceptance.