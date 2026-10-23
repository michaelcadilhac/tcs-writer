# tcs-writer

Reusable writing and review instructions for theoretical computer science papers, addressed to a first-year TCS PhD student oriented toward ICALP Track B. The set covers five roles: writer, scientist, student, reviewer, and copy editor.

These are the author's working preferences, not official ICALP policies or a substitute for a particular year's submission rules.

## Get started

```sh
git clone https://github.com/michaelcadilhac/tcs-writer.git
```

Keep this checkout available alongside your paper and point the coordinating assistant to [AGENTS.md](AGENTS.md). Alternatively, copy the complete instruction set into a dedicated directory in the paper's workspace. Preserve any existing workspace instructions rather than replacing them.

Supply a brief for your paper using the [project-brief checklist](AGENTS.md#project-brief), then request the task you want performed. Available agents and tools depend on the system you use; these files do not create agents themselves.

## Example requests

For a revision:

> Follow tcs-writer/AGENTS.md. Revise the manuscript identified in the attached project brief to address the listed issues.

For a complete review:

> Follow tcs-writer/AGENTS.md. Use separate scientist, fresh student, and reviewer agents to check the complete current revision identified in the attached brief.

For typography:

> Follow tcs-writer/AGENTS.md. Have the copy editor inspect the current source and rendered PDF identified in the attached brief.

Replace `tcs-writer/` with the path to your checkout or copied instruction directory.

## Documentation

- [AGENTS.md](AGENTS.md): coordination, role inputs, revision workflow, records, and acceptance.
- [WRITER.md](WRITER.md): shared writing requirements.
- Role instructions: [scientist](SCIENTIST.md), [student](STUDENT.md), [reviewer](REVIEWER.md), and [copy editor](COPY_EDITOR.md).
