# Naming Convention

This naming convention defines how workflow steps, branches, and actions are structured in **ConnectionSphere**.

#### Example Workflow (ASCII)

```
  rule2a.00
      |
      v
  rule2b.00
      |
      +-----------------------+
      |                       |
      v                       v
  rule2b.1a              rule2b.2a
      |                       |
      v                       v
  rule2b.1b              rule2b.2b
```

* The main branch flows from `rule2a` → `rule2b`
* Two branches originate from `rule2b`
* Each branch has two sequential steps (`a` → `b`)

## General Format

```
<flow>.<version>-<rule>.<branch>.<sequence>-<uuid>.<action>
```

#### Example

```
standard.2.1-rule2c.1a.00-175b8693-d4b8-4b63-b1cf-3e3ca92df31f.seq00.linkedin-connection-request
```

## Components

#### 1. Flow and Version

```
standard.2.1
```

* `standard` → workflow type
* `2.1` → version of the workflow

#### 2. Rule

```
rule2a
rule2b
rule2c
```

* Represents sequential steps in the main workflow
* Ordered alphabetically (`2a`, `2b`, `2c`, etc.)

#### 3. Branch

```
00   → main path
1a   → first step in branch 1
1b   → second step in branch 1
2a   → first step in branch 2
```

* `00` indicates the main (non-branching) flow
* Branches originate from a rule
* The number (`1`, `2`, etc.) identifies the branch
* The letter (`a`, `b`, etc.) defines the sequence of steps within that branch

Examples:

```
rule2c.00     → main path
rule2c.1a     → branch 1, step a
rule2c.1b     → branch 1, step b (next step in same branch)
rule2c.2a     → branch 2, step a
```

#### 4. Campaign ID

```
175b8693-d4b8-4b63-b1cf-3e3ca92df31f
```

* Identifier of the campaign that all rules belong to
* Ensures that all steps are grouped under the same campaign

#### 5. Action

```
tag
append-country
lead-approval
seq00.linkedin-connection-request
seq01.linkedin-direct-message
```

* Describes the operation performed at this step
* Should be human-readable and action-oriented

## Key Rules

* Main workflow steps must follow a strict sequence (`rule2a → rule2b → rule2c`)
* Branch numbers define independent branches from the same rule
* Letters (`a`, `b`, etc.) define sequential steps within the same branch
* `1a → 1b` means continuation of the same branch, not a new branch
* Action names should be descriptive and consistent across workflows
