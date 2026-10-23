# Writing papers for an ICALP Track B audience

Reusable instructions for writing and checking theoretical computer science papers. The topic may change; the audience, roles, and writing requirements stay fixed. These are the author's working preferences, not official ICALP policies or a substitute for the submission rules of a particular year.

## The five roles

| File | Responsibility |
| --- | --- |
| [WRITER.md](WRITER.md) | Writing requirements, organization, motivation, definitions, notation, wording, and version preservation. |
| [SCIENTIST.md](SCIENTIST.md) | Scientific correctness and a continuous, explicit record of the complete argument. |
| [STUDENT.md](STUDENT.md) | An isolated fresh reading by a first-year TCS PhD student oriented toward ICALP Track B. |
| [REVIEWER.md](REVIEWER.md) | Exacting, adversarial review at ICALP Track B standards. |
| [COPY_EDITOR.md](COPY_EDITOR.md) | Typography and rendered-document checks, only when requested. |

The scientist is an expert in ICALP Track B and related TCS topics. That expertise does not remove the need to verify unfamiliar mathematics or external results. The reader always has the same first-year background; do not make an explanation acceptable by quietly treating the student as a specialist.

## Start a paper

Clone this repository, then make these files available to the assistant working on the paper:

```sh
git clone https://github.com/michaelcadilhac/icalp-track-b-writing.git
```

You can reference this checkout directly or copy the five role files into a dedicated directory in the paper's workspace. If the workspace already has instructions, integrate references to these files rather than overwriting them. Keep the five files together because the role instructions refer to WRITER.md.

These filenames do not automatically create agents or activate a workflow. Explicitly ask the assistant to read the applicable files and perform a particular task. If separate agents are available and you want them, explicitly request them. A single assistant can apply the instructions too, but must not claim independent reviews or an isolated fresh reading that did not occur.

Supply a short brief for the particular paper, covering:

- The scientific question, contribution, and status of the claims.
- The current manuscript and any supporting source or rendered files.
- Which version may be edited, which versions must be preserved, and whether a new version is required.
- The requested work: drafting, revision, scientific verification, student reading, reviewer assessment, or copy editing.
- Any relevant submission format, length limit, and available compilation or rendering tools.
- Where the scientist's continuing record and review reports should be kept.

The brief supplies the paper's facts and constraints. It does not replace the fixed audience or import the notation and assumptions of a previous paper.

## Give each role the right material

| Role | Material to provide |
| --- | --- |
| Writer | WRITER.md, the brief, the current manuscript, and the scientific arguments and corrections needed for the task. |
| Scientist | SCIENTIST.md, WRITER.md, the brief, the current manuscript, relevant sources, and the complete continuing scientific record for this paper. |
| Fresh student | STUDENT.md, WRITER.md, the fixed audience and accepted prerequisites, and the complete current manuscript including appendices. |
| Reviewer | REVIEWER.md, WRITER.md, and the complete current manuscript; inspect it independently before using earlier reports to check regressions. |
| Copy editor | COPY_EDITOR.md, WRITER.md, the current source and rendered document, and the requested inspection scope. |

Do not give a fresh student earlier drafts, previous reviews, private explanations, revision notes, the scientist's record, or the conversation that developed the paper. The student starts from scratch on every submitted revision. General writing preferences and ordinary disciplinary knowledge are retained; knowledge of this paper is not.

The scientist does the opposite: preserve the entire argument continuously, including proofs, hypotheses, dependencies, failed approaches, examples, and unresolved questions. Never replace that record with a bare statement that an earlier revision was approved. Keep records for different papers separate.

## A revision workflow

1. Have the scientist establish the claims, their justifications, and any unresolved issues.
2. Have the writer prepare or revise the manuscript using WRITER.md and the agreed science.
3. Request an isolated student reading of the complete current revision. Repair the actual manuscript when a reader encounters an undefined concept, unexplained change of goal, or apparently contradictory assignment.
4. Request the reviewer's scrutiny of the actual revised document. Resolve scientific objections with the scientist; do not substitute agreement among agents for a proof.
5. After further revisions, obtain the fresh readings and scientific checks required by the role files. Tie each assessment to the exact version actually read.
6. Request a copy-editor pass when desired. Compile and inspect the rendered document, preserving definitions, motivation, and mathematical content.

A requested local check is useful, but it is not acceptance of the whole manuscript. A reader who retains the drafting conversation is not an isolated fresh student. State review scope and limitations plainly. General approval of a proposed edit does not certify its eventual wording.

The copy editor is not required after every change. When a copy-editor pass is requested, its verdict concerns the actual rendered artifact inspected.

## Example requests

For an initial revision:

> Read WRITER.md and SCIENTIST.md. The current manuscript and the continuing argument record are identified in the brief below. Verify the proposed scientific change, then revise the authorized version for the fixed first-year ICALP Track B audience. Preserve earlier versions, definitions, and motivation. Report unresolved scientific issues explicitly.

For separate scientific and reader checks:

> Use separate scientist, fresh student, and reviewer agents with their corresponding role files and WRITER.md. Have the scientist retain the complete argument record. Give the student only the role instructions, general writing requirements, accepted prerequisites, and the complete current manuscript. Have the reviewer first assess the manuscript itself. Identify the precise version and scope of every assessment.

For typography:

> Apply COPY_EDITOR.md and WRITER.md to the current source and rendered PDF. Inspect the complete document for clipping, overflow, awkward mathematical line breaks, lone symbols, and broken headings. Make only authorized typographical repairs; escalate changes that could affect scientific meaning. Recompile and inspect the result.

## Requirements that must survive reuse

- No manuscript-specific undefined term used; no defined term or notation left unused.
- Every sentence must contribute a useful assertion, explanation, or transition at the point where the reader encounters it.
- Introduce goals and motivate constructions before relying on them. Challenge changes of goal and apparently contradictory choices.
- Keep abstracts precise, with relevant problems introduced before reductions or constructions; no display mathematics in abstracts.
- Keep the result central. An overview explains the ideas; formal proofs and appendices supply the appropriate detail. Conclusions recap results, significance, limitations, and explicit questions rather than retelling proofs.
- Preserve the wording preferences in WRITER.md, including the rejection of ChatGPTisms and ambiguous labels or verbs. Reserved technical vocabulary must not be reused in a conflicting ordinary sense. Mathematical examples in the role files illustrate these rules; they do not prescribe every paper's objects or notation.
- Succinctness must not remove necessary definitions, reasoning, or articulation.
- The scientist maintains the complete argument without resetting; the student starts over on each submitted revision.
- Preserve earlier versions, annotations, and user edits. An open editor tab is not permission to overwrite another version.
- Compilation, numerical checks, polished layout, and agent agreement do not establish mathematical correctness.

This checklist is a reminder, not a replacement for the full role files. Do not shorten the detailed instructions to this checklist when assigning work.

## Maintaining these instructions

Keep general writing requirements in WRITER.md and role-specific behavior in the corresponding file. Put a paper's definitions, proof record, review reports, submission-specific formatting, and version paths in that paper's workspace, not in this reusable repository. When updating the instructions, check the changes for lost requirements and contradictory role descriptions.
