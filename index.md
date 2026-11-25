# Parallel Order Book Matching Engine
Azdeen Zack (azack) and Julian Koide (rkoide)

Our project is a simulated order book that receives buy and sell orders for one security and matches them by price and arrival order. We will study whether it can process those orders faster using multiple CPU cores while still producing the correct trades.

[Read our Project Proposal](proposal.pdf)
[Read the Project Milestone Report](milestone-report.pdf)

## Revised Schedule

| Period | Work completed or planned |
| --- | --- |
| Week 1, week of November 9 | Define the matching rules for limit orders. (Azdeen and Julian)<br>Build the sequential engine and repeatable order streams. (Azdeen)<br>Check the trade record and final book state. (Julian) |
| Week 2, week of November 16 | Build the whole book lock and first fine grained version, then check their results against the sequential engine. (Azdeen)<br>Begin comparing performance and investigating the cost of coordinating workers. (Azdeen and Julian) |
| November 23 through 26 | Finish the fine grained measurements and use them to decide what to study next. (Azdeen)<br>Implement dependency aware grouping, measure it on GHC and Delta, and revise it based on the results. (Julian)<br>Design the parallel large fill approach. (Azdeen)<br>Complete the milestone report and update the project website. (Azdeen and Julian) |
| November 27 through 30 | Implement parallel large fills and check the results against the sequential engine. (Julian)<br>Measure large fills across fill sizes and worker counts. (Julian)<br>Review the results and prepare figures and analysis for the final report. (Azdeen) |
| December 1 through 3 | Compare the approaches across workloads and worker counts. (Julian)<br>Measure the time spent finding groups, coordinating workers, calculating fills, and producing trades. (Julian)<br>Investigate improvements suggested by the measurements. (Azdeen)<br>Choose the main findings for the final report. (Azdeen and Julian) |
| December 3 through 6 | Begin the final report and prepare its main figures during travel for nationals. (Azdeen and Julian)<br>Complete focused measurements or code changes where needed. (Azdeen and Julian) |
| December 7 | Finish the code, main experiments, figures, conclusions, and final report. (Azdeen and Julian) |
| December 8 through 10 | Prepare the poster and presentation. (Azdeen)<br>Review the figures and results used in the poster and report. (Julian)<br>Make final revisions for the poster session on December 11. (Azdeen and Julian) |
