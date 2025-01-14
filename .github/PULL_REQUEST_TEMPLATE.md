# Task

<!---
Link to Related Odoo task
-->

# Description

<!---
What is changing and why? If someone is reading this 2 years from now to track down a bug, how will they make sense of these changes?
-->

# Reproduction

<!---
If this PR is for a bug fix, explain how to reproduce the bug
-->


# Development Checklist
> No PR should be approved until all items are complete. Plan and estimate tasks accordingly
>
> See the knowledge app for additional details (Knowledge > Delivery > Developers > Development)

- [ ] Custom code follows [PEP 8](https://peps.python.org/pep-0008/) using [black formatter](https://black.readthedocs.io/en/stable/)
    - 3rd party modules can be left unformatted
- [ ] Code documentation is complete
  - [ ] All functions have docstrings
  - [ ] [All interesting/clever code has a comment adding context](https://stackoverflow.blog/2021/12/23/best-practices-for-writing-code-comments/)
    - If code feel interesting or clever, be mindful of [Kernighan's Law](https://github.com/dwmkerr/hacker-laws#kernighans-law)
      > Debugging is twice as hard as writing the code in the first place. Therefore, if you write the code as cleverly as possible, how will you ever debug it?
- [ ] Module level documentation is complete
  - [ ] `changelog.md`
  - [ ] `README.md`
  - [ ] `__manifest__.py`
- [ ] Repo/Project Level Documentation is updated
  - `README.md`
- [ ] PR is being merged into the correct target branch (e.g. dev#1234 into E2E)
- [ ] Mindfully select reviewer(s)
    
  - Spread the love!  It's easy to request the same person each time, but that keeps us from getting better
  - You can add multiple reviewers. Don't be shy
  - If the merge is large, contains a lot of other developers code, feels complicated, etc... Please add your pod's Development SME as a reviewer
    > Given a large enough beta-tester and co-developer base, almost every problem will be characterized quickly and can be solved by someone who has encountered a similar problem before.
    >
    >[Linus's Law](https://github.com/dwmkerr/hacker-laws#linuss-law)

###  **EXTREMELY IMPORTANT**
- [ ] **Always** use the right type of merge:
  - **Squash merge development branches** into staging branches
  - **Normal merge staging branches** into all other branches
- [ ] **After Merging:** Update/Install all changed modules
  - This is a must, otherwise the changes may not get tested
