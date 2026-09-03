# Unit Outline Helper

**Current iteration:** Unit Outline Helper v1.2_29042025  
**Audience:** Sydney Law School academic and professional staff  
**Platform:** Cogniti

The supplied 2025 guide identified an earlier ChatGPT4o configuration. The current resource does not hard-code an underlying model because the current model configuration is not stated in the supplied materials. The tool itself remains **Unit Outline Helper**.

## What Unit Outline Helper can do

The agent can:

1. draft or revise **Unit Learning Outcomes (ULOs)**;
2. draft or revise an **assessment summary** for Sydney Curriculum (AKARI);
3. extract relevant ULO or assessment information from existing text;
4. analyse ULOs against:
   - Course Learning Outcomes (CLOs);
   - Sydney University Graduate Qualities;
   - Australian Qualifications Framework expectations, especially Level 9 where relevant; and
   - Council of Australian Law Deans Threshold Learning Outcomes for the LLB and JD; and
5. analyse alignment between assessments and ULOs.

You can work through these tasks individually or ask the agent to combine them.

## Getting started

The agent may begin by asking which task you want to complete:

1. Write new ULOs.
2. Write a new assessment summary.
3. Write both ULOs and an assessment summary.
4. Extract ULO information from existing text and create new ULOs.
5. Extract assessment information from existing text and create an assessment summary.

You can reply with the relevant number or describe the task directly.

## Using existing unit material

You can paste existing material from a unit outline, handbook entry or curriculum document into the agent and ask it to extract and reorganise the information.

A direct prompt can be as simple as:

```
Analyse the following text:

"""
[paste the existing ULOs, assessment summary or unit material here]
"""

Create a new set of Unit Learning Outcomes in the required format.
```

For an assessment summary, replace the final instruction with:

```
Create a new assessment summary in the required format.
```

In this context, **required format** means the output format configured for the agent. Staff should still check that the result satisfies current University curriculum requirements.

## Checking constructive alignment

After drafting ULOs and an assessment summary, ask:

```
Create a matrix showing the alignment between ULOs and assessments in this unit.
```

The supplied methodology uses a 0–2 scale:

- **0** = ULO not addressed;
- **1** = ULO partially addressed;
- **2** = ULO addressed.

The analysis considers the unit title, description, ULOs and assessment summary to evaluate the extent to which the assessment design gives students opportunities to demonstrate the intended outcomes.

## Broader curriculum mapping

The supplied curriculum-mapping methodology extends the analysis by considering:

- the purpose and nature of each assessment;
- expected student outputs;
- formative/summative and individual/collaborative characteristics;
- correspondence between assessment demands and ULO verbs;
- full or partial coverage of each ULO;
- gaps or over-concentration across the assessment suite;
- assessment weighting where appropriate; and
- consistency with relevant educational and professional frameworks.

The detailed methodology is reproduced in `resources/curriculum-mapping-methodologies.md` and on the main GitHub Pages site.

## Human review

Generated ULOs, assessment summaries and mapping judgements are draft curriculum-development artefacts. They should be checked against current University curriculum requirements, the actual design of the unit and any relevant course or accreditation requirements.

Do not enter personal, protected or highly protected data where the model is not deployed in an Australian geographic region.
