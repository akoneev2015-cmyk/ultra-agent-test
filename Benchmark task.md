# ULTRA-Agent Benchmark — Task v1

## Objective

Create a deterministic text artifact from the specification below.

The artifact must contain exactly these five fields, in this order:

1. `name`
2. `version`
3. `status`
4. `goal`
5. `validation`

## Required values

name: ULTRA-Agent
version: 1.0
status: benchmark
goal: deterministic artifact generation
validation: all required fields must exist and preserve their names

## Requirements

- Do not rename any field.
- Do not omit any field.
- Preserve the field order.
- Preserve the specified values.
- Do not add additional fields.
- The output must be deterministic.
- The artifact must be plain UTF-8 text.

## Expected artifact

Create:

`benchmark/output.txt`

with exactly:

name: ULTRA-Agent
version: 1.0
status: benchmark
goal: deterministic artifact generation
validation: all required fields must exist and preserve their names

## Agent workflow

The agent should:

1. Read this task.
2. Create `benchmark/output.txt`.
3. Verify the output against `benchmark/CRITERIA.md`.
4. Report the verification result.
