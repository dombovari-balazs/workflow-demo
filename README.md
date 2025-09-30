# workflow-demo

Creating a sample workflow playground

Ideal scenario:

Priorities:

1. Minimize Github costs
2. Security
3. Replayable deployment procedure from cloud

- if push: feature/*  --> manually triggerable: build + test + linter
- if push: staging --> manually triggerable: build, test + lint, ECR push
- if PR: to main --> auto run: build, test + lint, ECR push (?) to staging
- if push: main --> auto run: build, test + lint, ECR push,
                --> manually triggerable: deploy (terraform apply)
