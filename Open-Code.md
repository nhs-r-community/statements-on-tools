# Open code in the NHS

## Introduction

There are number of organisations and publications advocating open coding in its various guises within the NHS and more generally across the public sector and academia.  This page is intended as a place to collate pertinent literature and proposed/tried approaches to implementation of open code policies in situations in the NHS from individual teams up to entire organisations.

There is also a significant crossover between open code and software engineering best practice, which means that they are often (always?) promoted together as an effective means to improve reproducibility, 

### Glossary (DRAFT)

- **Reproducible Analytics Pipelines (RAP)**: analytics processes developed in open source programming languages and adhering to software engineering best practices to allow for reproducing analyses with very little effort.
- **Repo/Repository**: a set of files organised in a project for a specific purpose (such as [statements-on-tools](https://github.com/nhs-r-community/statements-on-tools) itself), containing code or documentation under version control.

## References

The following is a list of some of the material available online discussing and supporting open coding and software engineering approaches to code development in the NHS:

- [The Goldacre Report](https://www.gov.uk/government/publications/better-broader-safer-using-health-data-for-research-and-analysis) - a systematic and far-reaching report, written on behalf of the Department of Health, advocating for open coding and reproducible analytical pipelines (RAP) in the NHS,
- [Office for Statistics Regulation – Overcoming Barriers to Adoption of RAP](https://osr.statisticsauthority.gov.uk/publication/reproducible-analytical-pipelines-overcoming-barriers-to-adoption/) - a report written in support of RAP for adoption by all government departments doing analytics, describing the challenges and recommending solutions to address those challenges covering both organisational, team-level and individual barriers,
- [NHSX Open Source Policy](https://github.com/nhsx/open-source-policy) (currently in DRAFT) - a comprehensive description of why and how open source should be implemented in the NHS, including statements about best practice and a checklist for open sourcing code,
- [NHSD RAP Community of Practice](https://github.com/NHSDigital/rap-community-of-practice) - a repository containing a wealth of material pertaining to setting up and running RAP, including open source - based on their internal work to implement RAP in various NHSD analytical teams.

## Specific challenges

### Opening code without exposing data/'secrets'

This issue is often raised (and rightly) when discussing open sourcing of code - how do you ensure that personal clinical or other sensitive data are not shared?  In practice there are a number of approaches to this (see the [NHSX Open Source Policy](https://github.com/nhsx/open-source-policy) for more practical advice on this) including setting up repos with automated checking for datasets and secrets (such as API keys) in order that risk of unintentional disclosure is minimised.

### Opening code without giving away commercial/business/clinical proprietary information (and IP)

Many members of the NHS-R community work in teams or individually without any formal training or support to enable them to determine whether there would be significant ramifications of publishing particular code, especially where business processes might be encoded in the project, or where there might be some IP issue. This makes the prospect of open sourcing rather daunting.

### Coding in the open

The [NHSX Open Source Policy](https://github.com/nhsx/open-source-policy) recommends that all development/analytics work done in the NHS be coded in the open unless there is good reason not to.  However it also states that ["an internal code review should be conducted for all open source projects before publication"](https://github.com/nhsx/open-source-policy/blob/main/open-source-policy.md#e-assurance-requirements), which is at odds with coding in the open.

