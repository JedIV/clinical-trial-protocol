# 9 STATISTICAL CONSIDERATIONS

## 9.1 Statistical Hypotheses

### Primary Hypothesis (Continuous Co-Primary Endpoint)

- **Null Hypothesis (H₀):** There is no difference between SkeetSteph and placebo in mean percent change in body weight from baseline to Week 72 (μ_SkeetSteph - μ_Placebo = 0).
- **Alternative Hypothesis (H₁):** SkeetSteph is superior to placebo in mean percent change in body weight from baseline to Week 72 (μ_SkeetSteph - μ_Placebo ≠ 0).
- **Testing:** Two-sided test at alpha = 0.05 (adjusted per hierarchical testing procedure below).

### Co-Primary Hypothesis (Binary Co-Primary Endpoint)

- **Null Hypothesis (H₀):** There is no difference between SkeetSteph and placebo in the proportion of participants achieving ≥5% body weight reduction at Week 72 (π_SkeetSteph - π_Placebo = 0).
- **Alternative Hypothesis (H₁):** SkeetSteph is superior to placebo in the proportion achieving ≥5% weight reduction at Week 72 (π_SkeetSteph - π_Placebo ≠ 0).
- **Testing:** Two-sided test at alpha = 0.05.

### Multiplicity Adjustment for Co-Primary Endpoints

Both co-primary endpoints must be statistically significant (p < 0.05) for the study to be declared positive. This intersection-union testing approach controls the overall Type I error rate at 0.05 without requiring further alpha adjustment, as both hypotheses must be rejected for success.

### Key Secondary Hypotheses (Hierarchical Testing)

If both co-primary endpoints are statistically significant, the following secondary endpoints will be tested in a pre-specified hierarchical (fixed-sequence) order at alpha = 0.05:

1. Proportion achieving ≥10% weight reduction at Week 72
2. Proportion achieving ≥15% weight reduction at Week 72
3. Change in waist circumference from baseline to Week 72
4. Change in systolic blood pressure from baseline to Week 72
5. Change in IWQOL-Lite total score from baseline to Week 72

Testing proceeds sequentially; if any test in the sequence fails (p ≥ 0.05), all subsequent endpoints are considered exploratory (descriptive only). This hierarchical procedure controls the familywise Type I error rate at 0.05.

## 9.2 Sample Size Determination

### Primary Endpoint for Sample Size Calculation

The sample size is based on the continuous co-primary endpoint: percent change in body weight from baseline to Week 72. The continuous endpoint was selected as the basis for powering because it provides greater sensitivity to detect treatment differences than the binary responder endpoint.

### Assumptions

**Effect Size:**
- Expected mean percent change in body weight with SkeetSteph: -12.0%
- Expected mean percent change in body weight with placebo: -2.5%
- Expected treatment difference: 9.5 percentage points
- Basis: Conservative estimate informed by STEP 1 (semaglutide: -14.9% vs placebo: -2.4%, NCT03548935), SURMOUNT-1 (tirzepatide: -15.0% to -20.9% vs placebo: -3.1%, NCT04184622), and ATTAIN-1 (orforglipron: -7.5% to -11.2% vs placebo: -2.1%, NCT05869903). A conservative 12% weight loss assumption for SkeetSteph accounts for the possibility of lower efficacy compared to established agents.

**Standard Deviation:**
- Common standard deviation: 8.5%
- Basis: Standard deviations observed in STEP 1 (~7-9%) and SURMOUNT-1 (~8-10%) for the primary weight change endpoint.

**Statistical Parameters:**
- Statistical test: Mixed Model for Repeated Measures (MMRM) with ANCOVA at Week 72 as confirmatory
- Significance level: Two-sided alpha = 0.05 (no adjustment required for co-primary intersection-union test)
- Power: 90%
- Allocation ratio: 2:1 (SkeetSteph : Placebo)

### Sample Size Calculation

Using a two-sample t-test approximation (conservative relative to MMRM/ANCOVA which provides higher power by leveraging repeated measures):

- **Unadjusted sample size:** Approximately 2,400 (SkeetSteph) and 1,200 (Placebo) = 3,600 total
- **Dropout adjustment:** 20% expected dropout rate based on similar trials (STEP 1: ~14%, SURMOUNT-1: ~15%, with conservative margin for a novel agent)
- **Adjusted sample size:** 3,600 / (1 - 0.20) = 4,500
- **Final enrollment target:** N = 4,500 (3,000 SkeetSteph : 1,500 Placebo)

This enrollment target also meets the FDA 2025 draft guidance requirements of ≥3,000 subjects randomized to the investigational drug and ≥1,500 subjects on placebo for ≥1 year of maintenance treatment.

### Sensitivity Analyses for Sample Size

| Scenario | Effect Size | SD | Power | N Total (Adjusted) | Conclusion |
|----------|------------|-----|-------|-------------------|------------|
| **Base case** | 9.5% | 8.5% | 90% | 4,500 | Adequately powered |
| **Conservative effect** (20% lower) | 7.6% | 8.5% | ~85% | 4,500 | Adequately powered |
| **Higher variance** (20% higher SD) | 9.5% | 10.2% | ~82% | 4,500 | Adequately powered |
| **Both conservative** | 7.6% | 10.2% | ~75% | 4,500 | Borderline; may require sample increase |

The proposed sample size of 4,500 provides robust power (≥80%) under moderately conservative assumptions. If actual effect size is smaller than anticipated, the interim analysis (Section 9.4.6) will provide an opportunity for sample size re-estimation.

### Power for Co-Primary Binary Endpoint

- Expected proportion achieving ≥5% weight loss: ~85% (SkeetSteph) vs ~35% (Placebo)
- At N = 4,500 (2:1), power exceeds 99% for the binary endpoint using Chi-square test
- The binary co-primary endpoint is not the power-limiting endpoint

### Power for Key Secondary Endpoints

The study is formally powered for the continuous co-primary endpoint. Key secondary endpoints are expected to have sufficient power (>80%) based on effect sizes observed in similar trials, though formal power calculations for each secondary endpoint are not presented. Analyses of secondary endpoints that do not achieve statistical significance in the hierarchical testing procedure will be considered exploratory.

**IMPORTANT DISCLAIMER:** Sample size calculations are preliminary estimates based on pattern analysis of similar trials. Formal sample size calculation using validated statistical software (nQuery, PASS, or SAS PROC POWER) and review by a qualified biostatistician is required before study initiation. Final sample size may be adjusted based on updated assumptions, Phase 2 data, or regulatory feedback from the Pre-IND meeting.

## 9.3 Populations for Analyses

| Population | Definition | Primary Use |
|-----------|------------|-------------|
| **Intent-to-Treat (ITT)** | All randomized participants, analyzed per randomization assignment regardless of treatment received | Primary population for all efficacy analyses |
| **Modified ITT (mITT)** | All randomized participants who received ≥1 dose of study drug and had ≥1 post-baseline body weight measurement | Supportive efficacy analysis |
| **Per-Protocol (PP)** | All mITT participants who completed ≥52 weeks of treatment (maintenance period), had ≥80% compliance with study drug, had body weight measured at Week 72 (±14 days), and had no major protocol deviations | Supportive efficacy analysis; sensitivity analysis |
| **Safety** | All participants who received ≥1 dose (or partial dose) of study drug, analyzed per treatment actually received | All safety analyses |
| **DXA Substudy** | All randomized participants at DXA-qualified sites who consented to DXA substudy and completed baseline DXA | Exploratory body composition analyses |

**Major Protocol Deviations (excluding from PP):**
- Enrollment of participant not meeting inclusion/exclusion criteria (eligibility violation)
- Use of prohibited concomitant medication (other GLP-1 RA, other prescription weight loss medication)
- Study drug compliance <80%
- Missing primary endpoint assessment (no body weight at Week 72 ± 14 days)

## 9.4 Statistical Analyses

### 9.4.1 General Approach

All statistical analyses will be conducted using SAS version 9.4 or later (SAS Institute, Cary, NC) and/or R version 4.0 or later (R Foundation for Statistical Computing). A detailed Statistical Analysis Plan (SAP) will be finalized prior to database lock.

**Descriptive Statistics:**
- Continuous variables: N, mean, standard deviation, median, Q1, Q3, minimum, maximum
- Categorical variables: N, n (frequency), percentage (%)

**Inferential Statistics:**
- Two-sided tests at alpha = 0.05 unless otherwise specified
- 95% confidence intervals for treatment effects
- P-values reported to 4 decimal places

**Pre-Specified Covariates for Primary Analyses:**
- Baseline body weight (continuous)
- Stratification factors: BMI category, sex, race/ethnicity, glycemic status
- Age (continuous)

**Estimand Framework (per FDA 2025 Guidance and ICH E9(R1)):**

The primary estimand is the **treatment policy estimand**, which estimates the treatment effect regardless of adherence to study drug (intent-to-treat principle). This includes all data regardless of treatment discontinuation, use of rescue medication, or initiation of prohibited concomitant medications.

| Attribute | Definition |
|-----------|-----------|
| **Population** | Adults aged 30-39 with BMI ≥30 without T2DM |
| **Treatment** | SkeetSteph SC QW vs. Placebo SC QW + lifestyle intervention |
| **Endpoint** | Percent change in body weight from baseline to Week 72 |
| **Intercurrent Events** | Treatment discontinuation: included under treatment policy; Initiation of prohibited weight loss medication: included under treatment policy; Bariatric surgery: composite strategy (treatment failure) |
| **Summary Measure** | Difference in means between treatment groups |

A **supplementary estimand** (hypothetical estimand) will estimate the treatment effect assuming all participants adhered to study drug for the full 72 weeks, using MMRM under the MAR assumption.

### 9.4.2 Analysis of the Primary Efficacy Endpoint(s)

**Co-Primary Endpoint 1: Percent Change in Body Weight from Baseline to Week 72**

- **Population:** ITT
- **Statistical Model:** Mixed Model for Repeated Measures (MMRM)
  - Model: % Change from Baseline = Treatment + Visit + Treatment × Visit + Baseline Weight + BMI Category + Sex + Race/Ethnicity + Glycemic Status
  - Covariance structure: Unstructured (selected based on model fit criteria; compound symmetry and AR(1) as sensitivity)
  - Visits included: Weeks 4, 8, 12, 16, 20, 24, 36, 48, 60, 72
  - Primary inference: Least squares mean difference at Week 72 (SkeetSteph minus Placebo) with 95% CI and p-value
- **Confirmatory Analysis:** ANCOVA at Week 72 with multiple imputation for missing data (treatment policy estimand)
  - Multiple imputation: 50 imputations using Markov Chain Monte Carlo (MCMC) method under MAR assumption
  - Imputation model includes: treatment, baseline weight, all observed post-baseline weights, stratification factors
  - Combined using Rubin's rules
- **Sensitivity Analyses:**
  - Per-protocol population
  - Complete case analysis (participants with observed Week 72 weight)
  - Tipping point analysis: Determine what imputed values for missing data in the SkeetSteph arm would change the conclusion
  - Pattern-mixture model: Impute missing data using reference-based imputation (placebo-based pattern for SkeetSteph dropouts)
  - Delta-adjusted analysis: Add progressively larger penalties (delta = 0, 1, 2, 3, 4 percentage points) to imputed values in the SkeetSteph arm

**Co-Primary Endpoint 2: Proportion Achieving ≥5% Weight Reduction at Week 72**

- **Population:** ITT
- **Statistical Model:** Logistic regression
  - Model: logit(P[≥5% reduction]) = Treatment + Baseline Weight + BMI Category + Sex + Race/Ethnicity + Glycemic Status
  - Primary inference: Odds ratio (SkeetSteph vs. Placebo) with 95% CI, p-value, and estimated proportions with 95% CI for each arm
  - Risk difference and relative risk also reported
- **Missing Data:** Participants with missing Week 72 weight are classified as non-responders (conservative, aligned with FDA 2025 guidance treatment policy estimand)
- **Sensitivity Analysis:** Multiple imputation approach (impute missing weight, then classify responder status)

### 9.4.3 Analysis of the Secondary Endpoint(s)

Secondary endpoints tested in hierarchical order (Section 9.1) at alpha = 0.05:

| # | Secondary Endpoint | Statistical Method |
|---|-------------------|-------------------|
| 1 | Proportion achieving ≥10% weight reduction at Week 72 | Logistic regression (same covariates as co-primary); non-responder imputation for missing data |
| 2 | Proportion achieving ≥15% weight reduction at Week 72 | Logistic regression; non-responder imputation |
| 3 | Change in waist circumference baseline to Week 72 | MMRM (same structure as primary); LS mean difference with 95% CI |
| 4 | Change in systolic blood pressure baseline to Week 72 | MMRM; LS mean difference with 95% CI |
| 5 | Change in IWQOL-Lite total score baseline to Week 72 | MMRM; LS mean difference with 95% CI; MCID = 7.7 points |

Additional secondary endpoints (not in hierarchical gate, reported as descriptive):
- Change in fasting plasma glucose and HbA1c from baseline to Week 72
- Change in lipid panel (LDL-C, HDL-C, triglycerides) from baseline to Week 72
- Incidence and severity of alopecia through Week 72 (see Safety Analyses)
- Hairdex questionnaire change from baseline to Week 72

### 9.4.4 Safety Analyses

**Population:** Safety population (all participants receiving ≥1 dose)

**Adverse Events:**
- Treatment-emergent AEs (TEAEs): Events with onset after first dose or worsening of pre-existing condition after first dose
- Summary tables by System Organ Class (SOC) and Preferred Term (PT), sorted by decreasing frequency in the SkeetSteph arm:
  - Any TEAE
  - Treatment-related TEAEs (investigator-assessed possible, probable, or definite relationship)
  - TEAEs by maximum severity (CTCAE Grade 1-5)
  - Serious TEAEs
  - TEAEs leading to dose reduction
  - TEAEs leading to study drug discontinuation
  - Fatal TEAEs
- Denominators: Number of participants in the safety population per treatment arm
- Between-group comparison: Descriptive (no formal statistical testing); risk differences with 95% CI may be calculated for key AEs

**Adverse Events of Special Interest (AESI):**
- Dedicated summary tables for each AESI category (alopecia, pancreatitis, thyroid neoplasm/calcitonin elevation, gallbladder events, severe GI events, acute kidney injury, suicidal ideation/behavior, severe injection site reactions)
- For alopecia specifically:
  - Incidence by CTCAE grade (1, 2, protocol-defined Grade 3)
  - Time to onset (Kaplan-Meier estimate)
  - SALT score over time (mean, median, range)
  - Association between rate of weight loss and alopecia (logistic regression: alopecia yes/no ~ rate of weight loss per month, adjusting for baseline covariates)
  - Nutritional biomarker levels at time of alopecia onset vs. non-alopecia participants (descriptive)
  - Resolution/persistence at end of follow-up (Week 80)

**Serious Adverse Events:**
- Separate detailed table by SOC and PT
- Individual participant narratives for all SAEs

**Laboratory Data:**
- Shift tables: Baseline CTCAE grade to worst post-baseline CTCAE grade for amylase, lipase, ALT, AST, bilirubin, calcitonin, eGFR
- Potentially clinically significant (PCS) values: frequency by treatment arm (e.g., amylase >3× ULN, lipase >3× ULN, ALT >3× ULN, calcitonin ≥50 pg/mL)
- Nutritional panel parameters (ferritin, zinc, biotin, vitamin D): mean change from baseline over time by treatment arm

**Vital Signs:**
- Mean change from baseline in SBP, DBP, and heart rate at each visit
- Frequency of clinically notable values (SBP >160, HR >100 bpm)

**ECG:**
- Mean change from baseline in QTcF; frequency of QTcF >480 ms or >500 ms or increase >60 ms

**C-SSRS:**
- Shift from baseline in suicidal ideation category; frequency of any positive ideation or behavior

### 9.4.5 Baseline Descriptive Statistics

**Table 1: Baseline Characteristics by Treatment Arm (ITT Population)**

Three columns: SkeetSteph (N=3,000), Placebo (N=1,500), Total (N=4,500)

Variables:
- Demographics: Age (mean ± SD, range), Sex (n, %), Race (n, %), Ethnicity (n, %), Region (US, Canada, Europe; n, %)
- Anthropometric: Body weight (kg; mean ± SD), BMI (kg/m²; mean ± SD), BMI category (30-34.9, 35-39.9, ≥40; n, %), Waist circumference (cm; mean ± SD)
- Glycemic status: Normoglycemia vs prediabetes (n, %), FPG (mg/dL; mean ± SD), HbA1c (%; mean ± SD)
- Cardiometabolic: SBP, DBP (mmHg; mean ± SD), Total cholesterol, LDL-C, HDL-C, triglycerides (mg/dL; mean ± SD)
- Hair baseline: Hair density (hairs/cm²; mean ± SD), SALT score (mean ± SD), Hair pull test positive (n, %)
- Nutritional biomarkers: Ferritin, zinc, vitamin D, biotin (mean ± SD; n (%) below normal)
- Prior weight management: Prior diet attempts (n, %), Prior pharmacotherapy (n, %)
- Medical history: Hypertension (n, %), Dyslipidemia (n, %), Obstructive sleep apnea (n, %), NAFLD (n, %)

**No statistical testing between arms.** Baseline comparisons are descriptive only. Randomization ensures balance; hypothesis testing at baseline is methodologically inappropriate.

### 9.4.6 Planned Interim Analyses

**One planned interim analysis** will be conducted when approximately 50% of participants (N ≈ 2,250) have completed the Week 72 assessment.

**Purpose:** Efficacy and futility assessment

**Conduct:** The independent Data Safety Monitoring Board (DSMB) will conduct the interim analysis. The DSMB biostatistician will prepare unblinded analyses. The sponsor, investigators, and study team will remain blinded.

**Methods:**

| Parameter | Detail |
|-----------|--------|
| **Alpha spending function** | Lan-DeMets (O'Brien-Fleming type) |
| **Information fraction** | 0.50 |
| **Efficacy boundary** | z = 2.96 (approximately p = 0.003) at interim; z = 2.01 (approximately p = 0.044) at final |
| **Futility boundary** | Conditional power < 20% under the current trend |
| **Overall alpha preserved** | 0.05 (two-sided) |

**DSMB Recommendations:**
- Continue as planned
- Continue with sample size re-estimation (increase enrollment if effect size smaller than expected)
- Stop for efficacy (crosses efficacy boundary)
- Stop for futility (conditional power < 20%)
- Stop for safety (unacceptable risk-benefit ratio)

**Safety Reviews:** The DSMB will also conduct safety reviews approximately every 6 months (independent of the efficacy interim). Safety reviews will assess overall AE/SAE rates, mortality, alopecia incidence, and any emerging safety signals.

**Impact on Final Analysis:** Final analysis p-value boundary adjusted per the alpha spending function. All CIs adjusted accordingly.

### 9.4.7 Sub-Group Analyses

**Pre-specified subgroups** (exploratory, not adjusted for multiplicity):

1. **Age:** 30-34 vs 35-39 years
2. **Sex:** Male vs Female
3. **Race:** White vs Black/African American vs Asian vs Other
4. **Ethnicity:** Hispanic/Latino vs Not Hispanic/Latino
5. **BMI category:** 30-34.9 vs 35-39.9 vs ≥40 kg/m²
6. **Glycemic status:** Normoglycemia vs Prediabetes
7. **Baseline waist circumference:** Below vs above median
8. **Region:** US vs Canada vs Europe

**Analysis Method:**
- Treatment × subgroup interaction test in MMRM model (or logistic regression for binary endpoints)
- Interaction p < 0.10 considered suggestive of heterogeneity (given limited power)
- Forest plots: Treatment effect (LS mean difference or OR) with 95% CI for each subgroup level, with overall effect for reference
- Consistency assessment: Visual and qualitative evaluation of whether treatment benefit is maintained across subgroups

**Interpretation:** Subgroup analyses are hypothesis-generating. Results are reported descriptively and are not used for confirmatory inference. Risk of false-positive and false-negative findings due to multiplicity and low power is acknowledged.

### 9.4.8 Tabulation of Individual Participant Data

Individual participant data listings will be provided in appendices:
1. **Demographics and baseline characteristics** (all randomized participants)
2. **Adverse event listings** (all AEs, SAEs, AEs leading to discontinuation, deaths — with individual narratives for SAEs and deaths)
3. **Concomitant medication listings** (all medications during study)
4. **Laboratory data listings** (all values at all timepoints)
5. **Body weight over time** (all measurements for each participant)
6. **Alopecia event listings** (all alopecia AESIs with SALT scores, CTCAE grades, hair pull test results, nutritional biomarker values, onset timing, resolution status)
7. **Protocol deviation listings** (all deviations with impact assessment)
8. **Study drug exposure and compliance** (doses received, compliance percentage)

Listings sorted by treatment arm, then participant ID, then visit/date.

### 9.4.9 Exploratory Analyses

1. **Body Composition (DXA Substudy, N ≈ 500):**
   - Change in total fat mass (kg), lean body mass (kg), percentage body fat from baseline to Week 72
   - ANCOVA adjusted for baseline, sex, and treatment
   - Ratio of fat mass loss to lean mass loss (fat:lean ratio) by treatment arm
   - Descriptive statistics and treatment comparisons

2. **Alopecia — Weight Loss Rate Correlation:**
   - Logistic regression: Alopecia (yes/no) ~ average monthly % weight loss + baseline BMI + age + sex + nutritional biomarkers
   - Cox regression: Time to alopecia onset ~ rate of weight loss (time-varying covariate)
   - Threshold analysis: Identify rate-of-weight-loss threshold associated with increased alopecia risk

3. **Nutritional Biomarker Predictors of Alopecia:**
   - Comparison of baseline and time-varying nutritional biomarker levels (ferritin, zinc, biotin, vitamin D) between participants who develop alopecia and those who do not
   - ROC analysis for baseline biomarker values predicting alopecia development
   - Mixed model: Nutritional biomarker trajectory over time by alopecia status

4. **Responder Analyses:**
   - Proportion achieving ≥20% weight reduction at Week 72
   - Time to achieve ≥5% weight reduction (Kaplan-Meier, log-rank)
   - Characteristics of "super-responders" (≥20% loss) vs "non-responders" (<5% loss): descriptive comparison of demographics, baseline characteristics, and alopecia incidence

5. **Weight Loss Trajectory:**
   - Growth curve modeling of weight change over time
   - Latent class analysis to identify distinct trajectory subgroups (e.g., early responders, gradual responders, non-responders)
   - Characterization of trajectory classes by baseline factors

6. **Weight Regain After Treatment Discontinuation:**
   - Descriptive analysis of weight change from Week 72 to Week 80 (follow-up period)
   - Comparison of weight regain trajectory between SkeetSteph and placebo arms

### 9.4.10 Missing Data Handling (per FDA 2025 Guidance)

**Primary Approach: Treatment Policy Estimand with Multiple Imputation**

Consistent with FDA 2025 draft guidance, the primary analysis uses a treatment policy estimand that includes all data regardless of treatment adherence. Missing data are handled using multiple imputation:

- **Method:** Multiple imputation by chained equations (MICE) under the missing-at-random (MAR) assumption
- **Number of imputations:** 50
- **Imputation model variables:** Treatment arm, baseline weight, all observed post-baseline weights, age, sex, BMI category, glycemic status, race/ethnicity
- **Combination:** Rubin's rules for combining estimates across imputations
- **Software:** SAS PROC MI and PROC MIANALYZE (or R mice package)

**Sensitivity Analyses for Missing Data:**

1. **Complete case analysis:** Only participants with observed Week 72 weight (MCAR assumption)
2. **Reference-based imputation (jump-to-reference):** Missing SkeetSteph data imputed from placebo distribution (conservative for treatment policy estimand)
3. **Copy increments in reference (CIR):** Missing SkeetSteph data imputed assuming post-discontinuation trajectory matches placebo trajectory
4. **Tipping point analysis:** Progressively increase imputed values for SkeetSteph missing data (delta = 0, 1, 2, 3, 4 percentage points added) to identify assumptions that would change the primary conclusion
5. **Pattern-mixture model:** Model missing data patterns and assess sensitivity to the MAR assumption

**Missing Data Monitoring:**
- Missing data rates monitored quarterly by the sponsor data management team
- If missing data rate exceeds 25% in either arm, the DSMB will be notified and retention strategies intensified
- Missing data reasons (withdrawal of consent, LTFU, AE-related discontinuation) will be tabulated by treatment arm and compared descriptively

---

# 10 SUPPORTING DOCUMENTATION AND OPERATIONAL CONSIDERATIONS

## 10.1 Regulatory, Ethical, and Study Oversight Considerations

### 10.1.1 Informed Consent Process

The informed consent process will be conducted in accordance with 21 CFR Part 50, ICH E6(R2), and applicable local regulations. The informed consent form (ICF) will be written at an appropriate reading level (8th grade or lower) in the participant's primary language.

**Process:**
- The Principal Investigator or a qualified, trained designee will explain the study to potential participants
- Participants will be given adequate time (at least 24 hours recommended) to review the ICF and discuss with family members or personal physicians
- All questions will be answered to the participant's satisfaction before consent is obtained
- The voluntary nature of participation, the right to withdraw at any time without penalty, and the alternatives to study participation will be emphasized
- The ICF will describe all known risks, including the alopecia safety signal, in clear language

**Documentation:**
- The ICF is signed and dated by the participant (or legally authorized representative) and the person obtaining consent
- The original signed ICF is maintained in the study regulatory file
- A copy is provided to the participant
- The consent process is documented in the participant's medical record

**Re-Consent:** If the protocol is amended with changes that materially affect participant risk or benefit, a revised ICF will be submitted to the IRB for approval. Currently enrolled participants will be re-consented with the updated ICF.

**Special Consents:**
- DXA substudy: Separate consent section or addendum for body composition substudy
- Future use of specimens: Optional consent for storage and future research use of biological specimens
- HIPAA Authorization: Separate HIPAA authorization form (US sites)

### 10.1.2 Study Discontinuation and Closure

The study may be discontinued early if:
- The DSMB recommends termination based on safety or futility analysis
- The FDA or other regulatory authority requests or orders study discontinuation
- The sponsor determines that continued conduct of the study is not in the best interest of participants or is not feasible

**Closure procedures:**
- All enrolled participants notified and offered a final safety visit
- IRBs notified with reason for early termination
- FDA notified per regulatory requirements (IND safety report or annual report)
- ClinicalTrials.gov updated with "Terminated" status and reason
- All data collected through termination analyzed and reported
- Final clinical study report prepared and submitted to the FDA

### 10.1.3 Confidentiality and Privacy

Participant confidentiality is protected through:
- Assignment of unique numeric participant identifiers (site number + sequential ID)
- No personal identifiers (names, dates of birth, medical record numbers) included in the study database or transmitted to the sponsor
- Site master identification log linking participant ID to identity maintained separately in a locked location with restricted access
- All electronic data stored on password-protected, encrypted, access-controlled servers
- Data transmitted via secure encrypted channels
- HIPAA authorization obtained at US sites
- GDPR compliance at European sites, including Data Processing Agreements between sponsor and sites
- All study personnel sign confidentiality agreements

### 10.1.4 Future Use of Stored Specimens and Data

Participants may optionally consent to the storage and future use of biological specimens (blood samples) collected during the study. Future research may include biomarker discovery, pharmacogenomic analyses, or other exploratory investigations. Specimens will be coded (linked to study ID only, not personal identifiers) and stored at a sponsor-designated biorepository for up to 15 years. Participants may withdraw consent for future specimen use at any time, at which point remaining specimens will be destroyed.

Deidentified study data may be made available to qualified researchers upon reasonable request for secondary analyses, meta-analyses, or regulatory submissions, subject to a data use agreement. Individual participant data sharing will comply with applicable regulations (ICH E6, GDPR) and will not occur until after publication of the primary study results.

### 10.1.5 Key Roles and Study Governance

**Sponsor:** Responsible for overall study oversight, IND submission and maintenance, regulatory correspondence, study drug supply, site selection and qualification, clinical monitoring, data management, pharmacovigilance, statistical analysis, and the final clinical study report.

**Principal Investigator (Site PI):** Responsible for the conduct of the study at their site in accordance with the protocol, ICH-GCP, and applicable regulations. Duties include: IRB submissions, informed consent, participant safety, AE/SAE reporting, data accuracy, study drug accountability, staff supervision and training, and cooperation with monitoring and audits.

**Global Coordinating Investigator:** Provides scientific leadership, chairs the Steering Committee, leads publication efforts, and serves as the primary clinical interface with the sponsor.

**Steering Committee:** Provides scientific oversight of the study. Comprises the Global Coordinating Investigator, 4-6 key opinion leaders in obesity medicine, a biostatistician representative, and sponsor medical representatives. Meets quarterly.

**DSMB:** See Section 10.1.6.

**Contract Research Organization (CRO):** [TBD] — may be contracted by the sponsor to perform clinical monitoring, data management, biostatistics, pharmacovigilance, and/or regulatory submissions.

### 10.1.6 Safety Oversight

**Data Safety Monitoring Board (DSMB):**

A DSMB is required for this study given its large sample size, Phase 3 pivotal design, blinded treatment assignment with interim analysis, and the novel alopecia safety signal requiring ongoing monitoring.

**Composition:** 5 members — 2 clinical experts in obesity medicine/endocrinology, 1 dermatologist (for alopecia safety oversight), 1 independent biostatistician, 1 ethicist/clinical trialist. All members are independent of the sponsor and investigators with no financial conflicts of interest.

**Charter:** The DSMB operates under a formal charter that specifies membership, meeting procedures, data access, confidentiality requirements, voting rules, and reporting procedures. The charter is finalized before the first participant is enrolled.

**Meetings:** Approximately every 6 months, or more frequently if safety concerns arise. Meetings include:
- Open session: Aggregate blinded safety data presented to DSMB and sponsor
- Closed session: Unblinded safety and efficacy data reviewed by DSMB only

**Recommendations:** After each review, the DSMB provides one of the following recommendations to the sponsor:
- Continue study as planned
- Continue with modifications (protocol amendment, enhanced monitoring)
- Suspend enrollment pending further evaluation
- Terminate the study

**Stopping Rules:**

| Rule | Trigger | Action |
|------|---------|--------|
| **Safety** | Mortality rate >1% in SkeetSteph arm (not attributed to non-study causes) | DSMB convenes emergency review |
| **Safety** | Acute pancreatitis rate >2% in SkeetSteph arm | DSMB convenes emergency review |
| **Safety** | Severe alopecia (SALT >75%) rate >5% in SkeetSteph arm | DSMB convenes emergency review |
| **Futility** | Conditional power <20% at interim (Section 9.4.6) | DSMB may recommend termination |
| **Efficacy** | Efficacy boundary crossed at interim (Section 9.4.6) | DSMB may recommend early success |

### 10.1.7 Clinical Monitoring

A risk-based monitoring approach per FDA guidance ("Oversight of Clinical Investigations — A Risk-Based Approach to Monitoring") will be implemented.

**On-Site Monitoring:**
- Site initiation visit (SIV): Before first participant enrolled at each site
- Periodic monitoring visits: Quarterly during active enrollment, transitioning to semi-annual during follow-up
- Close-out visit (COV): After last participant completes study at each site

**Key monitoring activities:**
- 100% source data verification for: informed consent, eligibility criteria, primary endpoint (body weight), SAEs, study drug accountability
- Targeted SDV (~20%) for: secondary endpoints, laboratory data, concomitant medications, non-serious AEs

**Central/Remote Monitoring:**
- Real-time eCRF data review for data quality, completeness, and consistency
- Statistical monitoring for site-level outliers (enrollment patterns, AE rates, data distributions)
- Risk indicators tracked: query rates, protocol deviation rates, SAE reporting timeliness, enrollment vs. target

### 10.1.8 Quality Assurance and Quality Control

**Quality System:**
- Study conducted per sponsor and CRO SOPs
- All study staff complete ICH-GCP training and protocol-specific training before study involvement
- Protocol-specific training includes: SkeetSteph injection administration, alopecia assessment (trichoscopy, SALT scoring, scalp photography), C-SSRS administration, lifestyle intervention delivery, EDC system use

**Audits:**
- Sponsor QA may conduct audits of selected sites, the CRO, central laboratories, and the DSMB process
- Sites maintain inspection-ready regulatory files at all times
- FDA may conduct routine or for-cause inspections at any time

### 10.1.9 Data Handling and Record Keeping

**Electronic Data Capture:**
- EDC system: [TBD — e.g., Medidata Rave, Oracle Clinical, Veeva, or REDCap]
- 21 CFR Part 11 compliant with audit trail, electronic signatures, role-based access control
- Data entered within 3 business days of each visit
- Data queries resolved within 5 business days

**Source Documentation:**
- Source documents include: medical records, laboratory reports, ECG printouts, DXA reports, scalp photographs, PRO questionnaires, pharmacy dispensing records
- Source data verification performed per monitoring plan

**Database Lock:**
- All data entered, queries resolved, monitoring complete
- Medical and statistical review complete
- Database lock meeting conducted
- Database frozen for analysis

**Record Retention:**
- Study records retained for a minimum of 2 years after the last approval of a marketing application, or 2 years after the IND is closed, or per local regulations (whichever is longest)
- Sponsor will notify sites when records may be destroyed

### 10.1.10 Protocol Deviations

All protocol deviations are documented, classified (major vs minor), and reported to the sponsor and IRB per applicable requirements.

**Major deviations** (affecting participant safety, rights, or data integrity): Reported to the sponsor within 24 hours and to the IRB per IRB-specific timelines. Examples: enrollment of ineligible participant, administration of incorrect study drug, failure to obtain informed consent, missed SAE reporting.

**Minor deviations** (not affecting safety or data integrity): Documented and reported to the sponsor during routine data transmission. Examples: visit conducted outside the protocol-specified window, minor documentation omission.

**Root cause analysis** is performed for all major deviations and for patterns of minor deviations. Corrective and preventive actions (CAPA) are implemented as needed.

### 10.1.11 Publication and Data Sharing Policy

**Publication:** Study results will be published in a peer-reviewed journal per ICMJE guidelines. The primary manuscript is targeted within 12 months of study completion. Authorship will follow ICMJE criteria. The sponsor has the right to review manuscripts before submission for accuracy and protection of confidential information (review period: 30 days).

**ClinicalTrials.gov:** Results posted per 42 CFR Part 11 requirements within 1 year of primary completion date.

**Data Sharing:** Deidentified individual participant data may be made available to qualified researchers upon reasonable request after publication of the primary manuscript, subject to a data use agreement.

### 10.1.12 Conflict of Interest Policy

All investigators and sub-investigators will complete financial disclosure forms per 21 CFR Part 54 at study initiation and at study completion. Disclosable financial interests include compensation tied to study outcome, proprietary interest in SkeetSteph, equity interest in the sponsor exceeding $50,000, and significant payments exceeding $25,000 annually. The sponsor will review all disclosures and implement conflict management strategies as needed (increased monitoring, independent data verification, or investigator exclusion).

## 10.2 Additional Considerations

**Alopecia Assessment Training:**
All sites will designate at least one trained assessor for hair/alopecia assessments. Training will include standardized trichoscopy technique, SALT scoring, hair pull test procedure, and scalp photography positioning. A training module and certification quiz will be provided by the sponsor. Assessor certification must be completed before the first participant undergoes baseline hair assessment at each site.

**Lifestyle Intervention Standardization:**
Monthly dietitian counseling sessions will follow a standardized curriculum developed by the sponsor in consultation with obesity medicine experts. Training for site dietitians/nutritionists will be provided during the SIV. Lifestyle intervention adherence will be documented via participant food diaries and physical activity logs reviewed at each visit.

**Emergency Procedures:**
A 24/7 emergency contact line is available for investigators to reach the sponsor medical monitor for urgent safety questions, emergency unblinding requests, and guidance on management of study-related medical emergencies.

## 10.3 Abbreviations

| Abbreviation | Full Term |
|-------------|-----------|
| ADL | Activities of Daily Living |
| AE | Adverse Event |
| AESI | Adverse Event of Special Interest |
| ALT | Alanine Aminotransferase |
| ANCOVA | Analysis of Covariance |
| AST | Aspartate Aminotransferase |
| BMI | Body Mass Index |
| BUN | Blood Urea Nitrogen |
| CAPA | Corrective and Preventive Action |
| CBC | Complete Blood Count |
| CFR | Code of Federal Regulations |
| CI | Confidence Interval |
| CKD-EPI | Chronic Kidney Disease Epidemiology Collaboration |
| CMO | Contract Manufacturing Organization |
| COV | Close-Out Visit |
| CRO | Contract Research Organization |
| C-SSRS | Columbia-Suicide Severity Rating Scale |
| CTCAE | Common Terminology Criteria for Adverse Events |
| DIO | Diet-Induced Obese (animal model) |
| DSMB | Data Safety Monitoring Board |
| DXA | Dual-Energy X-ray Absorptiometry |
| ECG | Electrocardiogram |
| eCRF | Electronic Case Report Form |
| EDC | Electronic Data Capture |
| eGFR | Estimated Glomerular Filtration Rate |
| EOT | End of Treatment |
| EOS | End of Study |
| EQ-5D-5L | EuroQol 5-Dimension 5-Level |
| FAERS | FDA Adverse Event Reporting System |
| FDA | Food and Drug Administration |
| FPG | Fasting Plasma Glucose |
| GCP | Good Clinical Practice |
| GDPR | General Data Protection Regulation |
| GGT | Gamma-Glutamyl Transferase |
| GI | Gastrointestinal |
| GLP-1 | Glucagon-Like Peptide-1 |
| HbA1c | Glycated Hemoglobin |
| hCG | Human Chorionic Gonadotropin |
| HDL-C | High-Density Lipoprotein Cholesterol |
| HED | Human Equivalent Dose |
| HIPAA | Health Insurance Portability and Accountability Act |
| HR | Hazard Ratio |
| ICF | Informed Consent Form |
| ICH | International Council for Harmonisation |
| IND | Investigational New Drug |
| IRB | Institutional Review Board |
| ITT | Intent-to-Treat |
| IWQOL-Lite | Impact of Weight on Quality of Life - Lite |
| IWRS | Interactive Web Response System |
| KDIGO | Kidney Disease: Improving Global Outcomes |
| LDL-C | Low-Density Lipoprotein Cholesterol |
| LTFU | Lost to Follow-Up |
| MAR | Missing at Random |
| MCAR | Missing Completely at Random |
| MCID | Minimal Clinically Important Difference |
| MedDRA | Medical Dictionary for Regulatory Activities |
| MEN2 | Multiple Endocrine Neoplasia Type 2 |
| MICE | Multiple Imputation by Chained Equations |
| mITT | Modified Intent-to-Treat |
| MMRM | Mixed Model for Repeated Measures |
| MOA | Mechanism of Action |
| MTC | Medullary Thyroid Carcinoma |
| NDA | New Drug Application |
| NOAEL | No-Observed-Adverse-Effect Level |
| OHRP | Office for Human Research Protections |
| OR | Odds Ratio |
| PD | Pharmacodynamics |
| PHI | Protected Health Information |
| PI | Principal Investigator |
| PK | Pharmacokinetics |
| PP | Per-Protocol |
| PRO | Patient-Reported Outcome |
| PT | Preferred Term |
| QTcF | QT Interval Corrected by Fridericia Formula |
| QW | Once Weekly |
| RA | Receptor Agonist |
| RCT | Randomized Controlled Trial |
| ROC | Receiver Operating Characteristic |
| ROR | Reporting Odds Ratio |
| SAE | Serious Adverse Event |
| SALT | Severity of Alopecia Tool |
| SAP | Statistical Analysis Plan |
| SC | Subcutaneous |
| SD | Standard Deviation |
| SDV | Source Data Verification |
| SF-36 | Short Form 36 Health Survey |
| SIV | Site Initiation Visit |
| SoA | Schedule of Activities |
| SOC | System Organ Class |
| SOP | Standard Operating Procedure |
| SUSAR | Suspected Unexpected Serious Adverse Reaction |
| T2DM | Type 2 Diabetes Mellitus |
| TEAE | Treatment-Emergent Adverse Event |
| TIBC | Total Iron-Binding Capacity |
| TSH | Thyroid-Stimulating Hormone |
| ULN | Upper Limit of Normal |
| UP | Unanticipated Problem |
| WOCBP | Women of Childbearing Potential |

## 10.4 Protocol Amendment History

| Amendment # | Date | Description | Sections Affected |
|------------|------|-------------|-------------------|
| Original | 11-FEB-2026 | Original protocol (Version 1.0 Draft) | All |

---

# 11 REFERENCES

## A. FDA Guidance Documents

1. FDA. Obesity and Overweight: Developing Drugs and Biological Products for Weight Reduction. Draft Guidance for Industry. January 2025. Available at: https://www.fda.gov/regulatory-information/search-fda-guidance-documents/obesity-and-overweight-developing-drugs-and-biological-products-weight-reduction

2. FDA. Investigational New Drug (IND) Application. 21 CFR Part 312. Available at: https://www.accessdata.fda.gov/scripts/cdrh/cfdocs/cfcfr/CFRsearch.cfm?CFRPart=312

3. FDA. IND Safety Reporting Requirements. Available at: https://www.fda.gov/regulatory-information/search-fda-guidance-documents/safety-reporting-requirements-inds

4. FDA. Oversight of Clinical Investigations — A Risk-Based Approach to Monitoring. August 2013. Available at: https://www.fda.gov/regulatory-information/search-fda-guidance-documents/oversight-clinical-investigations-risk-based-approach-monitoring

5. FDA. Protection of Human Subjects. 21 CFR Part 50. Available at: https://www.accessdata.fda.gov/scripts/cdrh/cfdocs/cfcfr/CFRSearch.cfm?CFRPart=50

6. FDA. Institutional Review Boards. 21 CFR Part 56. Available at: https://www.accessdata.fda.gov/scripts/cdrh/cfdocs/cfcfr/CFRSearch.cfm?CFRPart=56

## B. ICH Guidelines

7. ICH E6(R2). Guideline for Good Clinical Practice. November 2016. Available at: https://database.ich.org/sites/default/files/E6_R2_Addendum.pdf

8. ICH E9(R1). Addendum on Estimands and Sensitivity Analysis in Clinical Trials. November 2019. Available at: https://database.ich.org/sites/default/files/E9-R1_Step4_Guideline_2019_1203.pdf

9. ICH E10. Choice of Control Group and Related Issues in Clinical Trials. July 2000. Available at: https://database.ich.org/sites/default/files/E10_Guideline.pdf

10. ICH E1. The Extent of Population Exposure to Assess Clinical Safety for Drugs Intended for Long-Term Treatment of Non-Life-Threatening Conditions. October 1994.

## C. Pivotal GLP-1 RA Clinical Trials

11. Wilding JPH, Batterham RL, Calanna S, et al. Once-Weekly Semaglutide in Adults with Overweight or Obesity. N Engl J Med. 2021;384(11):989-1002. ClinicalTrials.gov Identifier: NCT03548935.

12. Jastreboff AM, Aronne LJ, Ahmad NN, et al. Tirzepatide Once Weekly for the Treatment of Obesity. N Engl J Med. 2022;387(3):205-216. ClinicalTrials.gov Identifier: NCT04184622.

13. Aronne LJ, Sattar N, Horn DB, et al. Continued Treatment With Tirzepatide for Maintenance of Weight Reduction in Adults With Obesity: The SURMOUNT-4 Randomized Clinical Trial. JAMA. 2024;331(1):38-48. ClinicalTrials.gov Identifier: NCT04660643.

14. Wadden TA, Bailey TS, Billings LK, et al. Effect of Subcutaneous Semaglutide vs Placebo as an Adjunct to Intensive Behavioral Therapy on Body Weight in Adults With Overweight or Obesity: The STEP 3 Randomized Clinical Trial. JAMA. 2021;325(14):1403-1413. ClinicalTrials.gov Identifier: NCT03611582.

15. Davies M, Faerch L, Jeppesen OK, et al. Semaglutide 2.4 mg once a week in adults with overweight or obesity, and type 2 diabetes (STEP 2): a randomised, double-blind, double-dummy, placebo-controlled, phase 3 trial. Lancet. 2021;397(10278):971-984. ClinicalTrials.gov Identifier: NCT03552757.

16. Orforglipron, an Oral Small-Molecule GLP-1 Receptor Agonist for Obesity Treatment. N Engl J Med. 2025. ClinicalTrials.gov Identifier: NCT05869903.

## D. Alopecia and GLP-1 Safety Literature

17. Hair Loss Associated With Glucagon-Like Peptide-1 (GLP-1) Receptor Agonist Use: A Systematic Review. PMC. 2025. Available at: https://pmc.ncbi.nlm.nih.gov/articles/PMC12530271/

18. Alopecia as an Emerging Adverse Effect Associated With Glucagon-Like Peptide-1 (GLP-1) Receptor Agonists for Weight Loss: A Scoping Review. Cureus. 2025.

19. Buontempo S, et al. Exploring the hair loss risk in glucagon-like peptide-1 agonists: Emerging concerns and clinical implications. J Eur Acad Dermatol Venereol. 2025.

20. Branyiczky C, et al. Effects of GLP-1 Receptor Agonists on Hair Loss and Regrowth: A Systematic Review. Int J Dermatol. 2025.

## E. Obesity Background Literature

21. World Health Organization. Obesity and Overweight Fact Sheet. 2024. Available at: https://www.who.int/news-room/fact-sheets/detail/obesity-and-overweight

22. Hales CM, Carroll MD, Fryar CD, Ogden CL. Prevalence of Obesity and Severe Obesity Among Adults: United States, 2017-2018. NCHS Data Brief. 2020;(360):1-8.

23. Apovian CM, Aronne LJ, Bessesen DH, et al. Pharmacological management of obesity: an Endocrine Society clinical practice guideline. J Clin Endocrinol Metab. 2015;100(2):342-362.

24. Garvey WT, Mechanick JI, Brett EM, et al. American Association of Clinical Endocrinologists and American College of Endocrinology Comprehensive Clinical Practice Guidelines for Medical Care of Patients with Obesity. Endocr Pract. 2016;22 Suppl 3:1-203.

## F. Regulatory References

25. FDA. Financial Disclosure by Clinical Investigators. 21 CFR Part 54. Available at: https://www.accessdata.fda.gov/scripts/cdrh/cfdocs/cfcfr/CFRSearch.cfm?CFRPart=54

26. FDA. Electronic Records; Electronic Signatures. 21 CFR Part 11. Available at: https://www.accessdata.fda.gov/scripts/cdrh/cfdocs/cfcfr/CFRSearch.cfm?CFRPart=11

27. World Medical Association. Declaration of Helsinki: Ethical Principles for Medical Research Involving Human Subjects. 2013. Available at: https://www.wma.net/policies-post/wma-declaration-of-helsinki-ethical-principles-for-medical-research-involving-human-subjects/

28. National Cancer Institute. Common Terminology Criteria for Adverse Events (CTCAE) v5.0. November 2017. Available at: https://ctep.cancer.gov/protocoldevelopment/electronic_applications/ctc.htm

## G. Statistical References

29. Rubin DB. Multiple Imputation for Nonresponse in Surveys. New York: John Wiley & Sons; 1987.

30. Lan KKG, DeMets DL. Discrete Sequential Boundaries for Clinical Trials. Biometrika. 1983;70(3):659-663.

31. O'Brien PC, Fleming TR. A Multiple Testing Procedure for Clinical Trials. Biometrics. 1979;35(3):549-556.

## H. Intervention Documentation

32. [Sponsor]. SkeetSteph Investigator's Brochure. Version [TBD]. [Date TBD].

33. [Sponsor]. SkeetSteph Pre-filled Pen Instructions for Use. Version [TBD]. [Date TBD].
