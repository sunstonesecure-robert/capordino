# Outline of Unit and Data Testing

## MISC PUNCHLIST
- generate synthetic markdown content with all sorts of formatting to ensure no funny problems - especially wrt. escapeSquareBrackets
  - see: src/test/resources/cprt_800-171r3_sample.json
- ODP in element text regexes: ```  "(\\[Assignment: .+?\\])"  ```
  - [related assessment objectives in ODPs](https://github.com/sunstonesecure-robert/capordino/commit/b6c4541c0a12f18949a70fbf51f19177c034b5cb#diff-e0312d67ebb09e71cfbc827f084be1408ff92143c1c29812bf9e7437cff1f1b5R231)
    - replace with insert element
  - Pattern ``` odp_pattern = Pattern.compile("<(.+?): .+?>") ```
  - // Assumes assessment objective is correctly connected to the control it assesses
  - escapeSquareBracketsWithParentheses
- assessment-objective
  - all parts included
  - all links included
  - assessment_for_relationship: assessment-for
- global identifiers eg getSourceGlobalIdentifier
- Citations (reference publication links)
- sort-id props on controls, groups
- controls
  - statements
  - control links
  - RLinks to references to 800-53 controls, represented in CPRT site as Source Controls (no element type, external reference relationship type)
  - [should the base URL](https://github.com/sunstonesecure-robert/capordino/commit/f21c7074ecb11bb3a127eb9e0db9d4801b6c62d0#diff-e0312d67ebb09e71cfbc827f084be1408ff92143c1c29812bf9e7437cff1f1b5R171) be hardcoded or maybe added to some global vars?
- BackMatter
  - resources, citations/supporting pubs, links
- 
 

