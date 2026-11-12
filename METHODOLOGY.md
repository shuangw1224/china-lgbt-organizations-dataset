# Methodology

*Working documentation | November 12, 2026*

## 1. Research Design and Scope

This project builds an organization-level dataset of LGBT+ organizational life in mainland China. The intended scope includes formal NGOs, informal community groups, advocacy groups, student organizations, and HIV/AIDS-related groups with documented connections to sexual and gender minority communities.

The current stage identifies organizational candidates in the body text of the China AIDS Group mailing-list archive, followed by online corroboration and researcher review. Email attachments and additional source collections are planned for subsequent stages.

Organizational existence and relevance are assessed separately. HIV/AIDS-related records are examined for evidence of their constituencies, activities, and connections to LGBT+ communities. Named initiatives such as hotlines, projects, and events receive additional assessment to determine whether they represent distinct organizations or activities of another entity.

## 2. Initial Source: China AIDS Group

The researcher collected the China AIDS Group mailing-list archive through web scraping. The current extraction covers more than 7,000 email bodies. Attachments have not yet been systematically extracted.

HIV/AIDS organizing overlaps substantially with LGBT+ community organizing in China, making the archive a productive starting point for discovering organizations, initiatives, and networks. Email references document that a name or collective initiative appeared in a historical context. The surrounding text, including descriptions of activities, organizational relationships, and the communities served, shapes the evidentiary weight of each reference.

## 3. AI-Assisted Extraction and Name Consolidation

AI agents extract candidate organization names and supporting evidence from de-identified email text. The initial extraction prioritizes broad coverage, producing a candidate pool for subsequent screening.

The processing workflow verifies whether extracted names appear verbatim in the corresponding source messages. Candidate records retain source references and supporting excerpts for later examination.

Names are then normalized and grouped to identify repeated references and potential variants. Rule-based consolidation screens out clearly irrelevant records, including government institutions, unrelated institutions, foreign organizations, and strings that describe titles, addresses, or activities.

For the China AIDS Group cleaning stage documented in the repository, GPT performed both the initial extraction and a second classification pass. The second pass used a different prompt and original source evidence while withholding first-pass labels.

Name matches and classifications at this stage are provisional. Similar names, generic labels, branches, and renamed organizations require contextual review before they can be treated as the same entity.

## 4. Online Corroboration and Human Review

Following extraction and screening, AI agents search the web using candidate names and record potentially relevant links in an Excel review workbook.

The researcher opens these links and assesses whether the webpage supports the identity and existence of the candidate under review. Ambiguous names, generic references to "tongzhi" groups, working groups, and hotlines receive particular attention, since a search result can refer to a different entity or a general service.

Review addresses three questions:

- Does the evidence support the existence of an identifiable entity?
- Does the evidence refer to the same entity as the original email reference?
- Does that entity meet the project's organizational and substantive inclusion criteria?

The review workbook records researcher decisions and comments alongside automated results and evidence links. A record may be retained for further investigation even when its organizational status remains unresolved.

When contemporary webpages are unavailable, records are assessed through their original email context, with open questions noted for later stages. Automated verification labels and completed researcher review are reported separately.

## 5. Evidence Records and Data Structure

The working data distinguish organizational candidates from the documentary references used to assess them. Source references, email evidence, name variants, and web links support the investigation of each candidate.

Each organizational entry requires traceable supporting evidence: a source identifier, a location within the source, and a relevant date where available.

The Excel workbook supports review of candidate identity, organizational form, LGBT+ relevance, and supporting webpages. Researcher comments document ambiguities and judgments that require further resolution.

Further coding of organizational trajectories, identity categories, and repertoires of action is planned as identification and review progress.

## 6. Research Roles and Computational Infrastructure

Shuang Wu directs the research, collects source materials, specifies substantive requirements, examines intermediate outputs, and conducts manual review.

Technical collaboration is provided by [@lfkdsk](https://github.com/lfkdsk), who configures and maintains the infrastructure supporting AI-agent execution.

Fleet coordinates agent tasks. Switchboard enables agents to remotely access designated source folders on the researcher's computer and carry out processing tasks. AI agents assist with extraction, name consolidation, preliminary classification, and online searches.

Researcher feedback informs revisions to the processing workflow. Inspection of candidate outputs has led to additional screening requirements and closer examination of ambiguous organizational names.

Scripts, prompts, reports, and proposed changes are documented in the working GitHub repository where available. Method descriptions and reported counts refer to specific processing stages, with pending pull requests distinguished from merged results.

## 7. Planned Source Expansion and Limitations

Subsequent stages will examine email attachments and additional materials collected by the researcher, including archived webpages, Weibo data, and scraped online forums. Organization-name searches will help locate further evidence of activities, name variants, and organizational histories. Source expansion will proceed iteratively: the coverage of name-based searches depends on the names already identified.

Several limitations should be noted. An HIV/AIDS-focused mailing list gives greater visibility to organizations connected to its topics and networks. Organizational mentions vary in specificity, and repeated or forwarded material can reproduce the same underlying claim. Web searches are affected by page disappearance, indexing gaps, and name ambiguity. AI-assisted processing can produce omissions, false positives, and incorrect name matches. Source-text checks, staged screening, and researcher review address different parts of this uncertainty, and the extent of completed human review will be reported with each data release.

Given the sensitivity of the research topic, public documentation separates methodological information from raw correspondence and personal information. Decisions about releasing organization-level records will consider evidentiary quality, source-access conditions, and disclosure risks.

**Current status:** Candidate extraction and cleaning of China AIDS Group email bodies have been carried out. Online corroboration and manual review are ongoing. Systematic processing of attachments and additional source collections is planned.
