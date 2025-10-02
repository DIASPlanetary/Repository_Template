# Repository_Template
The goal of this repository is to provide a template and tips on repository best practices. This particularly geared publications and public code.



# How to make a doi with Zenodo
https://docs.google.com/presentation/d/1aWgv5r5GE3uPKDw5TePER4RoForSRIRGPHxeaXPGSnI/edit?usp=sharing

# Citation File
Make your own with https://citation-file-format.github.io/cff-initializer-javascript/#/

# Protecting the main branch
In a collaborative environment it can be important to protect your main branch so that no one can accidentally make changes to or delete the main branch causing other users to have problems. It is recommended to set up a rule to prevent any changes to the main branch without a pull request and without someone approving the pull request. Here is the step by step:
```mermaid
flowchart TD
A[Click Settings] --> B[Click Branches]
B --> C[Click Add branch ruleset]
C --> D[Give the ruleset a name. Suggestion protect main]
D --> E[Click Enforcement status and change to active]
E --> F[Select target branch, this will most likely be the default branch for your uses]
F --> G[Select the rules. The minium should be Restict deletions, Require a pull request before merging and Block force pushes]
G --> H[Click create]