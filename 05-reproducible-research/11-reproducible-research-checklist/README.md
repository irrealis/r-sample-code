# R Data-Science Samples and Guidelines
## 05 Reproducible Research
### 11 Reproducible Research Checklist
#### Questions and Answers:


'Overview'
What are some things to try to do in order to ensure reproducibility?

- DO start with good science.
- DO teach a computer.
- DO use version control.
- DO track your software environment.
- DO set your seed.
- DO think about the entire pipeline.



'Overview'
What are some things to avoid in order to ensure reproducibility?

- DON'T do things by hand.
- DON'T save irreproducible output.



What is meant by _DO start with good science_?

- Garbage in, garbage out.
- Try to start with coherent, focused questions.
    - They simplify many problems.
    - They can rule out possibilities/approaches/data/variables... you don't care about.
    - Vague questions tend to bloat complexity and to-do lists.
- Try to work with collaborators you like/admire/respect/work well with.
- Try to work on interesting problems.
    - That interest you.
    - That you think may interest others.



What is meant by _DO teach a computer_?

- If something needs to be done for a project, try to script or code it.
    - Even if you only need to do it once.
- Makes you say exactly what you mean to do, and how.
- Almost guarantees reproducibility/auditability.



What is meant by _DO use version control_?

- It's easy to publish results with GitHub/BitBucket/SourceForge/etcetera.
- Track and tag snapshots; simplifies reverting to old versions.
- Try to commit in small chunks.
- Avoid massive commits.
- Tends to slow things down enough to reduce mistakes.



What is meant by _DO track your software environment_?

- Can be critical for reproducing complex projects.
- Some components:
    - Computer architecture (CPUs/GPUs/...)
    - Operating system (Linux/macOS/Windows/...)
    - Software toolchain (compilers/interpreters/shells/languages/databases/analysis-software/...)
    - Internal dependencies (libraries/packages/...)
    - External dependencies (websites/repos/repos/remote-dbs/...)
    - Versions for all of the above.