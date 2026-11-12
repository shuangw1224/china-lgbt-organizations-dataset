# Methodology

*Working documentation | November 2026*

## 1. Research Design and Scope

This project is building an organization-level dataset to study the emergence, development, and transformation of LGBT+ organization landscape in mainland China. The intended scope includes formal NGOs, informal community groups, advocacy groups, student organizations, and HIV/AIDS-related groups with documented connections to sexual and gender minority communities.

The current stage focuses on identifying organizational candidates in the body text of the China AIDS Group mailing-list archive, followed by online corroboration and researcher review. Email attachments and additional source collections are planned for subsequent stages.

Organizational existence and relevance to the research scope are assessed separately. HIV/AIDS-related records are examined for evidence of their constituencies, activities, and connections to LGBT+ communities. Hotlines, projects, events, and other named initiatives require additional assessment to determine whether they represent distinct organizations or activities associated with another entity.

## 2. Initial Source: China AIDS Group

The researcher collected the China AIDS Group mailing-list archive through web scraping. The current extraction stage covers more than 7,000 email bodies. Attachments have yet to undergo systematic extraction.

The archive was selected as an initial source because HIV/AIDS organizing offers an important window into LGBT+ community organizing in China. Its correspondence provides documentary traces of groups, initiatives, and networks whose organizational histories and online presence require further investigation.

Email references provide evidence that a particular name or collective initiative was documented in a historical context. Their evidentiary value depends on the surrounding text, including descriptions of activities, organizational relationships, and the people or communities served.

The archive is treated as a source for candidate discovery and historical evidence. Its coverage reflects the subjects, participants, and networks represented in the mailing list.

## 3. AI-Assisted Extraction and Name Consolidation

AI agents extract candidate organization names and supporting evidence from de-identified email text. The initial extraction prioritizes broad coverage, producing a candidate pool for subsequent screening and review.

The processing workflow checks whether extracted names appear verbatim in the corresponding source messages. Candidate records retain source references and supporting excerpts so that their documentary basis can be examined.

Names are normalized and grouped to identify repeated references and potential variants. The current workflow includes rule-based name consolidation and screening of clearly irrelevant records, including government institutions, unrelated institutions, foreign organizations, and strings that describe titles, addresses, or activities.

For the China AIDS Group cleaning stage documented in the repository, GPT performed both the initial extraction and a second classification pass. The second pass used a different prompt and original source evidence while withholding first-pass classification labels.

Proposed name matches and classifications remain provisional. Similar names, generic labels, branches, and renamed organizations require contextual review before they can be treated as the same organizational entity.

## 4. Online Corroboration and Human Review

Following extraction and screening, AI agents search the web using candidate names and record potentially relevant webpage links in an Excel review workbook.

The researcher opens these links and assesses whether the webpage supports the identity and existence of the candidate under review. Particular attention is given to ambiguous names, generic references to “tongzhi” groups, working groups, and hotlines, for which a search result can refer to a different entity or a general service.

Review considers three distinct questions:

- Does the evidence support the existence of an identifiable entity?
- Does the evidence refer to the same entity as the original email reference?
- Does that entity meet the project’s organizational and substantive inclusion criteria?

The review workbook contains researcher decisions and comments alongside automated results and evidence links. Retaining a record for further investigation can therefore coexist with a judgment that it represents a project, service, or event whose organizational status remains unresolved.

Historical email evidence remains relevant when contemporary webpages are unavailable. Such records are assessed through their original context, with unresolved questions retained for further investigation. Automated verification labels and completed researcher review are reported separately.

## 5. Evidence Records and Data Structure

The working data distinguish organizational candidates from the documentary references used to assess them. Source references, email evidence, name variants, and web links support the investigation of each candidate.

The data-construction protocol requires organizational entries to have traceable supporting evidence, including a source identifier, a location within the source, and a relevant date where available.

The Excel workbook supports review of candidate identity, organizational form, LGBT+ relevance, and supporting webpages. Researcher comments document ambiguities and substantive judgments that require further resolution.

Further coding of organizational trajectories, identity categories, and repertoires of action is planned as identification and review progress.

## 6. Research Roles and Computational Infrastructure

Shuang Wu directs the research, collects source materials, specifies substantive requirements, examines intermediate outputs, and conducts manual review.

Technical collaboration is provided by [@lfkdsk](https://github.com/lfkdsk), who configures and maintains the infrastructure supporting AI-agent execution. This is an independent collaboration.

Fleet coordinates agent tasks. Switchboard enables agents to remotely access designated source folders on the researcher’s computer and carry out processing tasks. AI agents assist with extraction, name consolidation, preliminary classification, and online searches.

Researcher feedback informs revisions to the processing workflow. Inspection of candidate outputs has led to additional screening requirements and closer examination of ambiguous organizational names.

Scripts, prompts, reports, and proposed changes are documented in the working GitHub repository where available. Method descriptions and reported counts refer to specific processing stages and versions, with pending pull requests distinguished from merged results.

## 7. Planned Source Expansion and Limitations

Subsequent stages will examine email attachments and additional materials collected by the researcher, including archived webpages, Weibo data, and scraped online forums. Searches using organization names will help locate further evidence of activities, name variants, and organizational histories.

Source expansion will proceed iteratively. Organization-name searches depend on the names already identified, so their coverage will be assessed alongside opportunities to discover additional candidates.

The current source introduces several limitations. An HIV/AIDS-focused mailing list gives greater visibility to organizations connected to its topics and networks. Organizational mentions vary in specificity, and repeated or forwarded material can reproduce the same underlying claim. Web searches are also affected by page disappearance, indexing, and name ambiguity.

AI-assisted processing can produce omissions, false positives, and incorrect name matches. Source-text checks, staged screening, and researcher review address different parts of this uncertainty. The extent of completed human review will be reported with each data release.

Given the sensitivity of the research topic and the mailing-list material, public documentation will separate methodological information from raw correspondence and personal information. Decisions about releasing organization-level records will consider evidentiary quality, source-access conditions, and disclosure risks.

**Current status:** Candidate extraction and cleaning of China AIDS Group email bodies have been carried out. Online corroboration and manual review are ongoing. Systematic processing of attachments and additional source collections is planned.
