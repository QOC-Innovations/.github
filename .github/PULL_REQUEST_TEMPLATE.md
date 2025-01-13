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
- [ ] Module level documentation is complete
  - [ ] `index.html`
  - [ ] `changelog.md`
  - [ ] `README.md`
  - [ ] `__manifest__.py`
- [ ] Repo/Project Level Documentation is updated
  - `README.md`
- [ ] PR is being merged into the correct target branch (e.g. dev#1234 into E2E)
- [ ] Mindfully select reviewer(s)
  - Spread the love!  It's easy to request the same person each time, but that prevents knowledge sharing
  - You can add multiple reviewers. Don't be shy
  - If the merge is large, contains a lot of other developers code, feels complicated, etc... Please add your pod's Development SME as a reviewer

###  **EXTREMELY IMPORTANT**
- [ ] **Always** use the right type of merge:
  - **Squash merge development branches** into staging branches
  - **Normal merge staging branches** into all other branches
- [ ] **After Merging:** Update/Install all changed modules
  - This is a must, otherwise the changes may not get tested
