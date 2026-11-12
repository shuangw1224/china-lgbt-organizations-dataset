# China AIDS Group: Stage 2 Cleaning Report

**Preliminary Processing Results | Documentation updated November 12, 2026**

## Purpose and Scope

This report summarizes an initial cleaning stage for organization names extracted from the body text of the China AIDS Group mailing-list archive. It documents progress toward an organization-level database of LGBT+ organizations in mainland China.

The figures below summarize the Stage 2 processing output. Email attachments are outside the scope of this stage.

## Workflow

1. **Broad extraction:** GPT extracted candidate organization names and supporting references from email text, prioritizing coverage for later screening.
2. **Name consolidation:** Containment-based fuzzy matching grouped repeated names and potential variants.
3. **Rule-based screening:** Clearly irrelevant institutions and non-organization strings were removed.
4. **Second-pass GPT review:** A different prompt classified the remaining candidates using original source evidence, without access to first-pass labels.
5. **Preliminary classification:** Candidates were retained, marked pending, or excluded. Organizational form, LGBT+ relevance, and geographic scope were assessed separately.

Both passes used GPT; the second was an independent automated review, not a substitute for human validation.

## Processing Results

| Processing stage | Count |
|---|---:|
| Extracted occurrence rows | 43,086 |
| Candidate names after initial consolidation | 9,012 |
| Excluded by rule-based screening | 2,174 |
| Sent to second-pass GPT review | 6,838 |
| Retained after screening and review | 780 |
| Pending further verification | 1,789 |
| Excluded across both screening steps | 6,443 |
| Provisional mainland LGBTQ-related records selected for the working master | 208 |
| Of these, records not in the Stage 1 seed list | 167 |

The 780 retained candidates, 1,789 pending candidates, and 6,443 excluded candidates account for all 9,012 consolidated candidates. The 208 working-master records are a subset of the 780 retained candidates.

## Interpreting the Results

"Retained" here means kept for further investigation, not confirmed as eligible for the LGBT+ dataset. Among the 780 retained candidates, the preliminary LGBT+ relevance classifications were:

| Classification | Count |
|---|---:|
| Primary LGBT+ focus | 176 |
| Documented LGBT+ component | 32 |
| No documented LGBT+ component | 335 |
| LGBT+ relevance unknown | 237 |

The 208 records selected for the working master met the preliminary mainland and LGBT+ relevance criteria. Their identities and evidence are under further review. The 167 records not in the Stage 1 seed list are provisional additions.

Excluded material included foreign organizations and funders, government bodies, unrelated institutions, and strings referring to titles, addresses, roles, or activities rather than organizations. Some HIV/AIDS-related groups were retained for investigation without entering the LGBT+ working master because relevant evidence was absent or unclear.

## Limitations and Next Steps

This stage reduces a broad candidate pool to a more manageable set for investigation. It does not constitute a formal accuracy assessment.

Generic names, possible duplicates, and relationships between hotlines, projects, branches, and parent organizations require further review. Repeated email mentions may reproduce the same underlying information. The archive also gives greater visibility to organizations connected to HIV/AIDS networks.

Next steps are to corroborate the 208 provisional working-master records, investigate pending candidates, and resolve ambiguous entity relationships. Further work will extend processing to attachments and additional source collections. Public documentation will be updated as researcher review progresses.

See [METHODOLOGY.md](METHODOLOGY.md) for the broader research approach and [README.md](README.md) for the project overview. This report presents aggregate results; underlying candidate lists, correspondence, and personal information are not included.
