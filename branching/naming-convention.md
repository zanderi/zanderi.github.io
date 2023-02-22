---
layout: page
title: Naming Conventions
permalink: /branching/naming-conventions
parent: Branching Strategy
---

# Naming Conventions

## Creating Branches

Feature branches follow:
`/feature/[ticket number]`

Bug Fix
`/bug-fix/[ticket number]`

Release
`/release/[release-name]`

Hot Fix
`/hotfix/[ticket number]`

Devops
`/devops/[ticket number/name]`


## Commits




**Multiple commands on multiple issues**<br/>

| Syntax         | `<ISSUE KEY> <ISSUE KEY2> ... <ISSUE KEYn> #<COMMAND_1>` |
| Commit message | `JRA-123 JRA-234 JRA-345 #resolve #time 2d 5h #comment Task completed` |
| Result         | Logs 2 days 5 hours of work against issues JRA-123, JRA-234 and JRA-345, adds the comment 'Task completed' to all three issues, and resolves all three issues. <br/> Multiple issue keys must be separated by whitespace or commas. |