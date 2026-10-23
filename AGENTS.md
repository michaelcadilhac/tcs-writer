# Coordinating the five writing roles

Use this file for task coordination. Human setup instructions and example requests belong in [README.md](README.md); scientific and editorial criteria belong in the five role files linked below. Read the applicable role files rather than replacing their detailed requirements with a summary.

## Scope and authority

- Follow the user's current task, authorized manuscript version, preservation requirements, and review scope. Do not expand a local correction into a complete review or edit a paper when the user asked only about these instructions.
- The audience is always a first-year TCS PhD student oriented toward ICALP Track B. The scientist is a Track B expert; the reviewer is an exacting, adversarial ICALP Track B reviewer. Do not change these roles to make a difficult passage seem acceptable.
- [WRITER.md](WRITER.md) supplies the shared writing requirements. Each role also reads its own file. These coordination instructions do not weaken either set of requirements.
- The scientist adjudicates scientific questions with explicit arguments. The student independently judges accessibility; the reviewer independently challenges correctness and presentation. Scientific authority is not a reason to dismiss either reader's objection.
- Use separate agents when requested and supported. If independent agents or isolated contexts are unavailable, state that limitation. Do not present one assistant's successive role changes as independent reviews.

## Project brief

Before work on a paper, locate or obtain a brief identifying:

- The scientific question, contribution, and status of the claims.
- The current manuscript and supporting source or rendered files.
- Which version may be edited, which versions must be preserved, and whether a new version is required.
- The requested task and review scope.
- The submission format, length limit, and available compilation or rendering tools, where relevant.
- Where the scientist's continuing record and review reports are kept.

The brief supplies the paper's facts and constraints, not a replacement audience or assumptions imported from a different paper. A fresh student receives only the permitted reading material specified below, not the accumulated project brief or its revision history.

## Responsibilities and inputs

| Role | Instructions and material | Responsibility |
| --- | --- | --- |
| Writer | [WRITER.md](WRITER.md), the project brief, current manuscript, and agreed scientific changes | Revise the authorized source and preserve the user's requirements and earlier versions. |
| Scientist | [SCIENTIST.md](SCIENTIST.md), WRITER.md, current manuscript, relevant sources, and the complete continuing record for this paper | Establish correctness, resolve objections, and retain the full argument continuously. |
| Fresh student | [STUDENT.md](STUDENT.md), WRITER.md, the fixed audience and accepted prerequisites, and the complete current manuscript with appendices | Read from the beginning without prior knowledge of this paper and record difficulties when first encountered. |
| Reviewer | [REVIEWER.md](REVIEWER.md), WRITER.md, and the complete current manuscript | Assess the text independently before consulting earlier reports for regressions. |
| Copy editor | [COPY_EDITOR.md](COPY_EDITOR.md), WRITER.md, current source and rendered document, and the requested scope | Check typography and layout only when the user requests this role. |

The coordinator assigns work, controls versions and information flow, tracks objections, and reports what was actually checked. Coordination does not substitute for any role's assessment. Give each role only the material appropriate to its task; in particular, do not send the fresh student this coordinator's project notes or the scientist's record.

## Preserve the scientist's continuous record

1. Before scientific work on an existing paper, locate its continuing record. The scientist recovers the relevant complete arguments, not just a prior approval or a conversation summary.
2. Keep an accessible index of definitions, hypotheses, claims, full justifications, dependencies, examples, failed approaches, external sources, and unresolved questions. The record must support reconstruction of the argument, including details omitted from the manuscript.
3. Record scientific changes and their consequences as they arise. Mark superseded arguments as superseded while retaining their history and failure reasons. Recheck claims that depend on a changed assumption or lemma.
4. Preserve this record when the manuscript changes, the student is replaced, a session ends, or the scientist's active context is shortened. Before a handoff, save the complete supporting material and identify the exact current manuscript and unresolved issues.
5. A replacement scientist resumes from the same record. If a justification is missing, retrieve or re-establish it before relying on the associated claim. Do not erase the gap by carrying forward an old verdict.
6. Keep the record for each paper separate. The reusable role files are not a place to store a paper's proof or private review history.

Continuity means durable, retrievable arguments; it is not a claim that an agent has unlimited memory. The scientist must inspect the relevant justification when answering a question about it.

## Protect the student's fresh reading

For each complete student review of an updated manuscript, use a newly instantiated context with no inherited drafting conversation whenever the system supports it. A previously involved student may help diagnose or check a local repair, but cannot supply the isolated fresh reading of that new revision.

Provide only:

- STUDENT.md and the general writing requirements in WRITER.md.
- The fixed audience and accepted background, without a summary of this paper's argument or a list of intended fixes.
- The complete current manuscript, including appendices and figures needed to read it, and an identifier for that revision.
- A neutral request to read it sequentially and record where meaning, motivation, or reasoning first becomes unclear.

Do not provide previous drafts, diffs, prior reviews, the writer's account of the changes, the scientist's record, private explanations, expected answers, or the conversation that developed the paper. Do not reuse a context that has already seen those materials. If agents share a filesystem, supply a clear reading-file list and instruct the student not to inspect other project records; a fresh conversation alone does not enforce filesystem access restrictions.

The student retains ordinary TCS knowledge and general writing preferences. Reset knowledge of this paper, not disciplinary competence. The student builds a new reading record from what the current text supplies, and explicitly challenges changes of goal and apparently contradictory assignments.

After an initial objection has been recorded, the student may ask the scientist for a scientific explanation to diagnose the problem. That conversation does not repair the manuscript or count as evidence that the missing explanation was already present. Have the writer implement the agreed correction. A new revision submitted for complete student acceptance requires another fresh reading.

If isolation is unavailable, report the retained context and the limited status of the reading. Do not claim a fresh-student acceptance. A specifically requested local check is allowed, but must not be reported as a complete review.

## Coordinate a revision

1. Read the project brief and current source before editing; preserve intervening user changes.
2. Have the scientist establish the scientific content and the validity of proposed substantive changes before the writer implements them. Unresolved claims remain unresolved; do not improve the prose by silently strengthening a conclusion or deleting a hypothesis.
3. Designate one writer to integrate source edits. Readers report issues and proposed repairs unless editing has been explicitly assigned to them. Avoid simultaneous edits to the same manuscript.
4. Prepare a fixed revision for review and identify it by version and, where practical, a content hash. Reviews concern those actual files. If the user edits them meanwhile, preserve those edits and identify which review results need updating.
5. Have the scientist check the implemented scientific changes and affected dependencies. Then obtain the requested fresh-student and reviewer assessments. Respect any order specified by the user. Keep the student's initial reading independent of the other assessments.
6. Track each substantive objection by location, exact wording or claim, defect, required repair, and status. Send scientific questions to the scientist, prose repairs to the writer, and unresolved reading problems back for diagnosis. Do not close an objection solely because the agents agree outside the manuscript.
7. After a repair, check the actual implementation. Use a new isolated student for complete acceptance of an updated document. Have the reviewer recheck the affected argument, or the complete paper when its structure or proof has changed. Have the scientist update the continuous record and recheck scientific dependencies.
8. Activate the copy editor only when requested. Supply both source and current rendered output. Typographical repairs must preserve meaning; changes that may affect it return to the writer and scientist. Recompile and inspect the affected artifact after edits.
9. Deliver the authorized version and report the actual scope and outcome of each check. Identify unresolved objections, external dependencies, retained-context limitations, and any source/render mismatch. Do not claim approval for bytes or pages a role did not examine.

Independent checks of the same fixed revision can run in parallel when authorized, provided the student receives no prior explanations and the user has not specified a sequential order. Parallel readers do not authorize parallel source edits.

## Records and acceptance

Keep paper-specific working files in that paper's workspace, at paths selected for that project. Maintain:

- The current project brief.
- The scientist's indexed, continuing record with complete supporting arguments.
- A revision record identifying the source and rendered artifact actually reviewed.
- Separate student and reviewer reports with locations, findings, scope, verdict, and unresolved issues; include copy-editor reports only for requested passes.
- An issue list connecting each objection to its implemented repair and subsequent check.

Give the scientist access to these records as needed. Give a fresh student only the permitted reading material, not the accumulated records. Keep earlier reviews as historical evidence rather than silently relabeling them as approval of a later revision.

Before reporting a fully reviewed manuscript as acceptable, establish that the scientist checked its scientific content, a fresh student read that revision without unresolved barriers, and the reviewer examined the final relevant text. A requested copy-editor verdict must match the rendered artifact delivered. A local check supports only a local conclusion. Successful compilation, numerical checks, attractive layout, and agreement among agents do not prove mathematical correctness.

## Maintaining this instruction repository

When the user asks to maintain tcs-writer itself, edit the requested guidance rather than invoking a manuscript-review cycle. Preserve the detailed requirements in all five role files. Keep human setup and usage examples in README.md, coordination rules in this file, and role-specific criteria in the corresponding role file. Link to the authoritative section instead of maintaining duplicate instructions. Update cross-references when moving material, and check relative links and consistency of the fixed roles. Do not add paper sources, scientific records, private review reports, or submission-specific settings to this reusable repository.
