# R Data-Science Samples and Guidelines
## 05 Reproducible Research
### 03 Structure of a Data Analysis
#### Questions and Answers:


'Overview'
What are the typical steps of a data analysis?

- Define the question.
- Define the ideal data set.
- Determine what data you can obtain.
- Obtain the data.
- Clean the data.
- Exploratory data analysis.
- Statistical prediction/modeling.
- Interpret results.
- Challenge results.
- Synthesize/write up results.
- Create reproducible code.



What characterizes good questions for data analyis?

- Science generally determines the questions.
- The questions are focused and concrete.
- The questions lead to required data.
- Required data lead to applied statistics.



What are the benefits of focused, concrete questions for data analysis?

- They allow identifying/discarding data/variables that aren't pertinent.
    - This reduces noise in subsequent analyses.
- They reduce the search space for finding answers.



What characterizes the ideal dataset for your data analysis?

Depends on your goal.

- Descriptive analysis: requires an entire population.
- Exploratory analysis: requires a random sample measuring many variables.
- Inferential analysis: requires a random sample of the right population.
    - Requires carefully-selected population.
    - Requires carefully-selected sampling method.
- Predictive: requires training and testing subsets from the same population.- Causal: requires experimental data from a randomized study.
- Mechanistic: requires data about all components of the system.



What are some ways to obtain data?

- Mine the Web for free.
- If you can't find it for free, buy the data.
- If you can't buy the data, design and run a study to generate the data.
- If you can't generate the data, settle for a less-than-ideal dataset.


What are some important things to do when obtaining data?

- Obtain raw data.
    - Polite emails go a long way.
- Note and reference the source.
- When mining Web data:
    - Respect the terms of use.
    - Record URLs and access times when downloaded.



What are some important things to do when cleaning data?

- Understand the data source (census, sample, convenience sample, etc.)
- Understand any upstream preprocessing.
- Process data following tidy-data rules; in particular, be ready to provide to others:
    - The unaltered raw data.
    - The tidy data.
    - Scripts used to process the raw data into the tidy data.
    - Code books describing the tidy data.
- Determine whether the data are good enough. If not:
    - obtain more or different data;
    - or try a different question;
    - or quit -- continuing with bad data can lead to inappropriate inferences/conclusions.



What are some general steps for exploratory analyses?

- Look at data summaries.
- Check for missing data.
- Create exploratory plots.
- Perform exploratory analyses (e.g. clustering)



What are some general steps for statistical prediction/modeling?

- Should be informed by:
  - The questions of interest
  - Results of exploratory analysis
- Exact methods depend on the question of interest
- Prediction: prep to build a model for classification:
	- Subsample to generate test and training sets.
- Transformations/processing should be accounted for when necessary
- Measures of uncertainty should be reported
- What are the sources of uncertainty?



What are some general guidelines to follow when interpreting results?

- **Use appropriate language.** Don't use language going beyond the analysis that was performed:
  - "describes"
  - "correlates with"/"associated with"
  - "leads to"/"causes"
  - "predicts"
- Explain why certain models predict better than others.
- Interpret coefficients
- Interpret measures of uncertainty.
- Use uncertainty measures to calibrate interpretation of final results.



How and why should you challenge your results?

- _If you don't do this, someone else will._ Get a step ahead of everyone by doing it yourself first.
- Challenge all steps:
  - Question
    - Is it even valid?
  - Data source (where from, how obtained)
  - Processing (how done)
  - Analysis (how done)
  - Conclusions (how drawn, how solid)
  - Measures of uncertainty (do you have any?)
  - Models (why they're appropriate, choices of terms included, why some are better)
  - **What good is it?**
  - Think of potential alternative analyses.
    - Maybe useful in different ways.
    - Maybe produce better predictions.
- Have reasonable answers so when someone asks, you can respond.



What are some guidelines for synthesizing results and a write-up?

- **Tell a coherent story.**
- Lead with the question.
  - Helps people mentally establish context.
- Questions lead to data and analyses:
  - What kinds are appropriate for this question?
- Summarize the analyses into the story.
	- Winnow what you did down to the most important aspects.
  - Don't include every analysis. Critera for inclusion:
    - If it is needed for the story.
    - If it is needed to address a challenge.
- Keep all analyses in back pocket in case challenged.
  - "Did that analyses, but it was problematic because..."
- Order analyses according to the story, rather than chronologically.
- Include "pretty" figures that contribute to the story.
