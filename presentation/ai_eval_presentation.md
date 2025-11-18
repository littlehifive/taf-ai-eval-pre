<style>
.title-slide {
  background: linear-gradient(135deg, #2c3e50 0%, #34495e 50%, #2c3e50 100%);
  color: white;
}
.title-slide h1 {
  color: #ecf0f1;
  font-weight: 700;
}
</style>

# Introduction

## The Challenge

- Generative AI tools in low- and middle-income countries are
  multiplying

  - AI-powered math tutors for children
  - Digital advisory tools for farmers
  - Health assistants

- **Problem**: While some studies show effectiveness (e.g., [Henkel et
  al., 2024](https://arxiv.org/abs/2402.09809)), others show AI
  applications exhibit unexpected and unwanted behavior that can be
  harmful to users (e.g., [Bastani et al.,
  2024](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4895486))

- **Gap**: While there is broad consensus on the importance of
  evaluating GenAI in the development sector, there has been little
  agreement on what this actually means

- **Consequence**: In the absence of clear standards, organizations have
  adopted very different evaluation approaches

## The Problem: Fragmented Approaches

- **Tech-focused organizations**: Emphasize model/product performance,
  neglect development outcomes

- **Development-focused organizations**: Default to RCTs, ignore model
  and product evaluations

- **Funders**: Lack clarity on what evaluations to expect or what
  “right-sized” evaluation entails

- **Reality**: All methods are complementary and should be used together
  at different stages

## The Solution: Four-Level Framework

This playbook organizes evaluation around four levels:

1.  **Level 1 – Model evaluation**: Does the AI model produce the
    desired responses?

2.  **Level 2 – Product evaluation**: Does the product facilitate
    meaningful interactions?

3.  **Level 3 – User evaluation**: Does the product positively support
    users’ thoughts, feelings, knowledge, and behaviors?

4.  **Level 4 – Impact evaluation**: Does access to the product improve
    development outcomes?

## 

<img src="images/ai-eval-framework.jpg" width="40%" height="auto" style="display: block; margin: auto;" />

## Continuous Evaluation: The Central Element

- Unlike earlier rule-based digital tools, GenAI’s unique sensitivity to
  the underlying model, architecture, data, and prompts demands new
  evaluation methods

- The underlying components can evolve far faster than in earlier
  digital technologies - with new AI models and technologies being
  released weekly

- Developers must ensure their applications perform as intended over
  time, even as updates are released

- **Continuous evaluation** thus becomes essential, enabling developers
  to:

  - Iterate quickly
  - Maintain expected behavior
  - Steadily improve performance and impact

- This focus on continuous evaluation, while commonplace in software
  companies, might be less familiar in the development sector where
  programs are often judged by one-off experiments

## The Development Sector Challenge

- Development sector: Programs often judged by one-off experiments
  (evaluation as finish line)

- **Our approach**: Rapid, ongoing cycles where deployment, adaptation,
  evaluation, and improvement happen in tandem

- This is commonplace in software companies, but less familiar in
  development sector

## Framework Origins

- Lessons from **[AI for Global Development (AI4GD)
  accelerator](https://agencyfund.notion.site/ai-for-global-development)**
  - Led by [The Agency Fund](https://www.agency.fund/) (TAF)
  - Collaboration with [OpenAI](https://openai.com/) and [Center for
    Global Development](https://www.cgdev.org/) (CGD)
  - $5 million investment supporting 8 non-profit organizations
  - Focus: Education, health, and agricultural livelihoods
- Incorporates lessons from [AI4GD accelerator
  teams](https://theagencyfund.substack.com/p/ai-for-global-development-accelerator)
  and other leading organizations

## Natural Progression of Evaluation Levels

1.  **Level 1**: Build AI model pipeline, benchmark performance
2.  **Level 2**: Test product for usability and user engagement
3.  **Level 3**: Understand effects on thoughts, feelings, knowledge,
    behaviors
4.  **Level 4**: Assess long-term improvements in development outcomes

**Tech sector**: Typically stops at Levels 1-2 (engagement predicts
success)

**Development sector**: Higher bar - does it improve lives in
meaningful, measurable, cost-effective ways?

## Who Should Use This Guide?

- **AI Engineers** → Model behavior (Level 1)
- **Product Managers & Data Scientists** → Product analytics (Level 2)
- **Psychologists & Behavioral Researchers** → User thoughts, feelings,
  behaviors (Level 3)
- **Impact Evaluators** → Social impact (Level 4)

**Key**: All actors must see beyond their slice of the evaluation
process

## Building Blocks for GenAI Evaluation

Four concrete, actionable steps that move evaluation from theory into
practice:

1.  Construct a clear user funnel across Levels 1-4
2.  Build and track metrics through robust ETL pipelines
3.  Diagnose weak links through targeted hypotheses
4.  Run experiments with rigor and speed

## Building Block 1: User Funnel

A **user funnel** is a structured way to map how individuals move
through your product or program, from first exposure to long-term life
impact. A comprehensive funnel creates a shared framework for tracking a
user’s experience through a journey.

**To build a robust funnel**, teams should begin by defining the final
development outcome they’re targeting (Level 4) - for instance, improved
learning outcomes, better health, or increased crop yields. From there,
work backward to break down the journey into specific user stages.

## User Funnel: The 6 Stages

<table>
<colgroup>
<col style="width: 18%" />
<col style="width: 34%" />
<col style="width: 47%" />
</colgroup>
<thead>
<tr>
<th>Stage</th>
<th>Description</th>
<th>Evaluation Level</th>
</tr>
</thead>
<tbody>
<tr>
<td><strong>1. Recruitment</strong></td>
<td>Beneficiary identified and enters program</td>
<td>Level 2</td>
</tr>
<tr>
<td><strong>2. Onboarding</strong></td>
<td>User introduced to AI product and completes setup</td>
<td>Level 2</td>
</tr>
<tr>
<td><strong>3. Engagement</strong></td>
<td>User begins actively interacting with AI product</td>
<td>Level 2</td>
</tr>
<tr>
<td><strong>4. Retention</strong></td>
<td>User continues engaging over time (not dropping off)</td>
<td>Level 2</td>
</tr>
<tr>
<td><strong>5. Proximal Outcome</strong></td>
<td>Near-term cognitive or behavioral change</td>
<td>Level 3</td>
</tr>
<tr>
<td><strong>6. Development Outcome</strong></td>
<td>Long-term desired result achieved</td>
<td>Level 4</td>
</tr>
</tbody>
</table>

## User Funnel: What to Define for Each Stage

For each stage, teams should clearly define:

<table>
<colgroup>
<col style="width: 40%" />
<col style="width: 59%" />
</colgroup>
<thead>
<tr>
<th>Element</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><strong>What program does</strong></td>
<td>Actions to bring users into that stage</td>
</tr>
<tr>
<td><strong>What user must do</strong></td>
<td>User actions that count as entering the stage</td>
</tr>
<tr>
<td><strong>Metric</strong></td>
<td>Measurement that confirms entry (e.g., login rate, session
length)</td>
</tr>
<tr>
<td><strong>Target values</strong></td>
<td>Target metric values and transition rates between stages</td>
</tr>
<tr>
<td><strong>Costs</strong></td>
<td>Costs associated with moving a user through the stage</td>
</tr>
<tr>
<td><strong>DRIs</strong></td>
<td>Directly Responsible Individuals for performance and metrics</td>
</tr>
</tbody>
</table>

## Building Block 2: ETL Pipelines

A well-designed evaluation framework is only as good as the data
infrastructure that supports it. At the heart of that infrastructure is
a robust **ETL pipeline** - a system that extracts, transforms, and
loads data to power consistent, reliable measurement of program
indicators.

- **Extract**: Collect data from various sources - chat logs, product
  telemetry, survey tools, third-party APIs, or spreadsheets

- **Transform**: Clean, standardize, and reshape the raw data into a
  usable format. This could involve timestamp alignment, anonymization,
  session stitching, or deriving new metrics like time-on-task
  indicators

- **Load**: Store the transformed data in a centralized system (like a
  data warehouse or analytics dashboard) where teams can access it for
  analysis, visualization, or modeling

- **Why critical**: AI products, especially those using generative
  models, produce high volumes of complex, often unstructured data:
  prompts, outputs, clicks, feedback, engagement patterns, and more.
  Without a clear ETL pipeline, turning raw data into actionable metrics
  at scale becomes unreliable and slow.

- **Example**: A product designed to support adolescent mental health
  might collect model-level outputs (Level 1), engagement logs (Level
  2), behavioral indicators (Level 3), and outcome data (Level 4) - all
  requiring integration through a robust pipeline.

## Building Block 3: Targeted Hypotheses

Once a user funnel is in place and metrics are flowing through a robust
ETL pipeline, the next challenge is understanding why certain funnel
metrics are underperforming.

**Process**:

1.  **Identify drop-offs**: Start by identifying major user drop-offs
    along the funnel

2.  **Develop hypotheses**: Pose specific, testable questions: *Why are
    users stalling? What mechanism explains this?*

3.  **Surface competing hypotheses**: For example, if engagement dips
    after onboarding: *Is value proposition unclear? Are users
    overwhelmed? Do they mistrust the AI?*

4.  **Test hypotheses**: Each hypothesis becomes a lens for focused
    measurement or experiments

**Goal**: Make evaluation generative - helps teams ask better questions,
faster. This approach sits at the intersection of product management, UX
research, and behavioral science.

## Building Block 4: Experiments

Test hypotheses through experimentation:

- **A/B tests**: For lightweight product tweaks (prompts, messages)
- **Hold-out tests**: For more complex behavioral shifts
- **Pragmatic RCTs**: For policy-relevant questions
- **Full RCTs**: When causal question justifies cost

**Key**: Match experimentation to product maturity, hypothesis scale,
and decision stakes. Tools like
[**Evidential**](https://docs.evidential.dev/welcome/) help teams
automate randomization and track results.

## Building Cross-Functional Teams

Evaluation is a **team sport** - no single role covers all four levels.

<table>
<colgroup>
<col style="width: 20%" />
<col style="width: 35%" />
<col style="width: 44%" />
</colgroup>
<thead>
<tr>
<th>Level</th>
<th>Lead Roles</th>
<th>Support Roles</th>
</tr>
</thead>
<tbody>
<tr>
<td><strong>Level 1</strong></td>
<td>AI Engineers, ML Researchers</td>
<td>Domain Experts, Product Owners</td>
</tr>
<tr>
<td><strong>Level 2</strong></td>
<td>Product Managers</td>
<td>Data Scientists, Data Engineers</td>
</tr>
<tr>
<td><strong>Level 3</strong></td>
<td>Psychologists, UX Researchers</td>
<td>Data Scientists</td>
</tr>
<tr>
<td><strong>Level 4</strong></td>
<td>Policy Researchers, Economists</td>
<td>AI Engineers</td>
</tr>
</tbody>
</table>

## Best Practices for Cross-Functional Teams

1.  **Look Beyond Your Slices**: Understand how your work affects other
    levels
2.  **Pair Engineers with Domain Experts Early**: Involve domain experts
    at Level 1 from start
3.  **Identify Cross-Functional Lead**: Product Managers connect dots
    across roles
4.  **Use Shared Evaluation Language**: Common vocabulary using levels
5.  **Use Tools that Support Collaboration**: Evaluation platforms,
    dashboards, experimentation tools

## Level 1: Model Evaluation

**Question**: Does the AI model produce the desired responses?

**Why important**: AI models, especially large language models (LLMs)
and related foundational models, do not
[“understand”](https://www.sciencenews.org/article/ai-large-language-model-understanding?utm_source=chatgpt.com)
content in the way humans do. Instead, they generate outputs by
predicting the next word in a sequence based on statistical patterns in
their training data. Because of this, models can **hallucinate** or
appear fluent and convincing while still being inaccurate, biased,
irrelevant, or even harmful.

This makes structured model evaluation essential. We need to
systematically and rigorously assess whether an AI system consistently
meets conditions such as usefulness, accuracy, appropriateness, and
safety across diverse tasks and user contexts. This is especially
critical when AI tools are deployed in sensitive domains like education,
health, or agriculture, where misinformation or misalignment can cause
real harm.

Beyond ensuring safety, developers must also evaluate that their AI
systems exhibit desirable behaviors and characteristics proven to have a
real-world impact. For instance, an AI tutor should follow pedagogical
best practices - such as withholding answers to encourage self-directed
learning and accurately gauging a student’s level to tailor instruction.

## What is Being Assessed?

Most Generative AI applications are built on foundational models like
those from OpenAI (GPT), Anthropic (Claude), Google (Gemini), or Meta
(Llama). However, your application is a full system, not just the
foundational model. It includes many other components that can be
grouped into three buckets:

- **Pre-processing**: Before handing off the input from the user to the
  LLM, you may wish to transform it into a format suitable for the LLM.
  Examples include: sanitizing or filtering language; converting speech
  to text; paraphrasing the user’s request; translation from a
  low-resource language to a high-resource one.

- **LLM context preparation**: An LLM takes three things as input: the
  “prompt” or system instructions, the user’s input after being
  pre-processed, and a “context” which can include past conversation
  history, relevant content retrieved from your knowledge base, or even
  tools available for the LLM to call.

- **Post-processing**: Before returning the output to the user, you may
  also wish to transform it into the correct format and check the output
  using safety or quality guardrails. Examples include: hallucination
  checker, converting text to speech, translation to the user’s
  preferred language.

**Example**: An AI agronomist in Senegal, answering questions from
farmers in Pulaar, might: (a) check input for malicious intent, (b)
translate from Pulaar to English, (c) retrieve relevant content from
database, (d) retrieve information about the farmer, (e) generate an
answer, (f) check that the answer is grounded, (g) translate back to
Pulaar. Model evaluations cover this entire pipeline.

## Who is Most Involved?

<table>
<colgroup>
<col style="width: 27%" />
<col style="width: 72%" />
</colgroup>
<thead>
<tr>
<th>Role</th>
<th>Responsibility</th>
</tr>
</thead>
<tbody>
<tr>
<td><strong>AI Engineers, ML Researchers</strong></td>
<td>Execute - Lead model evaluation process</td>
</tr>
<tr>
<td><strong>Domain Experts, Product Owners</strong></td>
<td>Support - Define evaluation rubrics</td>
</tr>
</tbody>
</table>

## How to Evaluate: 6 Steps

1.  **Decide on rubric**: What characteristics should the solution
    embody?
2.  **Decide on metrics**: How to measure performance against rubric
3.  **Develop golden dataset**: Representative user interactions
4.  **Run automated evaluations**: Integrate into CI/CD pipeline
5.  **Measure scores and refine**: Use scores to improve solution
6.  **Red-teaming**: Actively try to break/pressure test before release

## 

<img src="images/l1-framework.png" width="100%" style="display: block; margin: auto;" />

## Step 1: Decide on Rubric

**Responsible**: Product Owners and Domain Experts (with Engineering
support)

**Question**: “What characteristics should our AI solution embody?”
These are qualitative goals (e.g., “Trustworthy”, “On-Brand”,
“Concise”). Most of the rubric will be determined by your use case,
context, and impact goals. This step requires reflection and discussion
with stakeholders - it is critical and guides the rest of your
evaluation steps.

## Step 1: Rubric Examples

<table>
<colgroup>
<col style="width: 37%" />
<col style="width: 24%" />
<col style="width: 37%" />
</colgroup>
<thead>
<tr>
<th>Organization</th>
<th>Product</th>
<th>Rubric Items</th>
</tr>
</thead>
<tbody>
<tr>
<td><strong><a href="https://jacarandahealth.org/">Jacaranda
Health</a></strong></td>
<td>PROMPTS: Maternal health SMS service (Swahili/English)</td>
<td>Medical accuracy, personability, simplicity (<a
href="https://cdh.stanford.edu/our-research-portfolio/generative-ai-health-low-middle-income-countries">Stanford
Center for Digital Health, 2025</a>)</td>
</tr>
<tr>
<td><strong><a href="https://digitalgreen.org/">Digital
Green</a></strong></td>
<td>Farmer.Chat: Agricultural advice platform (40+ crops, 4
countries)</td>
<td>Faithfulness, relevance, accessibility (<a
href="https://arxiv.org/abs/2409.08916">Singh et al., 2024</a>)</td>
</tr>
</tbody>
</table>

**Recommendation**: Restrict to ~5 items. Longer lists = more expensive
and difficult. Tradeoffs exist (e.g., concise vs. complete, friendly
vs. direct).

## Step 2: Decide on Metrics

**Responsible**: Engineering (with Product Owner validation)

Engineering translates qualitative rubric into quantitative metrics
(e.g., “Trustworthy” → “Factual Consistency Score”). Product Owner
validates that technical metrics are acceptable proxies for business
goals.

**Terminology**: Rubric item → Metric → Scorer → Score  
*Example*: “helpful” → “answer relevance” → “LLM-as-judge” → “4 out of
5”

## Step 2: Scorer Categories

<table>
<colgroup>
<col style="width: 18%" />
<col style="width: 18%" />
<col style="width: 13%" />
<col style="width: 18%" />
<col style="width: 11%" />
<col style="width: 18%" />
</colgroup>
<thead>
<tr>
<th>Category</th>
<th>Examples</th>
<th>Speed</th>
<th>Accuracy</th>
<th>Cost</th>
<th>Best For</th>
</tr>
</thead>
<tbody>
<tr>
<td><strong>Statistical</strong></td>
<td><a href="https://en.wikipedia.org/wiki/BLEU">BLEU</a>, <a
href="https://en.wikipedia.org/wiki/ROUGE_(metric)">ROUGE</a>, <a
href="https://en.wikipedia.org/wiki/METEOR">METEOR</a>, <a
href="https://en.wikipedia.org/wiki/Word_error_rate">WER</a></td>
<td>+++++</td>
<td>++</td>
<td>+</td>
<td>Specific tasks</td>
</tr>
<tr>
<td><strong>Model-based</strong></td>
<td><a href="https://github.com/yuh-zha/AlignScore">AlignScore</a>/<a
href="https://arxiv.org/pdf/2404.06579">LIM-RA</a>, <a
href="https://github.com/google-research/bleurt">BLEURT</a>, <a
href="https://arxiv.org/pdf/2106.11520">BARTScore</a>, <a
href="https://unbabel.github.io/COMET/html/index.html">COMET</a></td>
<td>+++</td>
<td>+++</td>
<td>+++</td>
<td>Domain-specific tasks</td>
</tr>
<tr>
<td><strong>LLM-as-judge</strong></td>
<td><a href="https://arxiv.org/abs/2303.16634">G-Eval</a>, <a
href="https://arxiv.org/abs/2210.08726">RARR</a></td>
<td>++</td>
<td>+++++</td>
<td>+++++</td>
<td>Flexible evaluation</td>
</tr>
<tr>
<td><strong>Human evaluation</strong></td>
<td><a
href="https://github.com/huggingface/evaluation-guidebook/blob/main/contents/human-evaluation/basics.md">Human
evaluation</a></td>
<td>+</td>
<td>+++++</td>
<td>++++++</td>
<td>Calibration &amp; QA</td>
</tr>
</tbody>
</table>

**Ideal**: Combination of methods. Human evaluation’s primary role:
create “answer key” to calibrate automated scorers and final QA. Note:
Human evaluation has [its own biases](https://arxiv.org/pdf/2307.03025).

## Step 3: Develop Golden Dataset

**Responsible**: Product Owner (with Domain Experts and Engineering
support)

Product Owner ensures quality, scope, and representativeness. Domain
Experts author ideal answers. Engineering provides technical support.

## Step 3: Dataset Sources

<table>
<colgroup>
<col style="width: 28%" />
<col style="width: 46%" />
<col style="width: 25%" />
</colgroup>
<thead>
<tr>
<th>Source</th>
<th>When to Use</th>
<th>Notes</th>
</tr>
</thead>
<tbody>
<tr>
<td><strong>Past transaction data</strong></td>
<td>Adding AI to existing application</td>
<td>Extract question-answer pairs from human-answered queries</td>
</tr>
<tr>
<td><strong>Human-annotated data</strong></td>
<td>Building new AI offering</td>
<td>Generate questions + expert answers. <strong>Warning</strong>: Don’t
use LLM to generate answers for experts to verify - correcting is harder
than creating</td>
</tr>
<tr>
<td><strong>Customize public datasets</strong></td>
<td>High-quality public dataset exists</td>
<td>Subset and augment to match your context</td>
</tr>
</tbody>
</table>

## Step 3: Good Dataset Characteristics

A good dataset should cover:

- **Types of questions**: Not just what, but also how (tone, language,
  code-switching, informality, spelling errors, verbosity)
- **Out-of-context requests**: Questions your application doesn’t
  support
- **Adversarial requests**: Abusive input, prompt injection,
  jailbreaking, data & privacy attacks

## Step 4: Running Automated Evals

**Responsible**: Engineering (with Product Owner support)

Automate evaluations and integrate into CI/CD pipeline. Product Owner
monitors performance trends over time.

## Step 4: Evaluation Frequency Strategy

<table>
<colgroup>
<col style="width: 28%" />
<col style="width: 26%" />
<col style="width: 28%" />
<col style="width: 15%" />
</colgroup>
<thead>
<tr>
<th>Eval Type</th>
<th>Examples</th>
<th>Frequency</th>
<th>When</th>
</tr>
</thead>
<tbody>
<tr>
<td><strong>Low-Cost</strong></td>
<td>Statistical scorers (ROUGE), model-based</td>
<td>Every commit</td>
<td>Fast feedback, limited scope</td>
</tr>
<tr>
<td><strong>High-Cost</strong></td>
<td>LLM-as-judge scorers</td>
<td>Nightly/weekly/before release</td>
<td>Comprehensive but expensive</td>
</tr>
</tbody>
</table>

**Tracking**: Use observability tools (Logfire, Helicone, Langfuse) to
plot metric scores over time. Dashboard helps track progress against
rubric goals.

## Step 5: Measure Scores and Refine

**Responsible**: Engineering (with Product Owner support)

Initial scores will reveal areas for improvement. Results are a
diagnostic tool, not a final grade. Engineering analyzes results and
diagnoses root causes. Product Owner prioritizes refinement work.

## Step 5: Refinement Process

<table>
<colgroup>
<col style="width: 26%" />
<col style="width: 34%" />
<col style="width: 39%" />
</colgroup>
<thead>
<tr>
<th>Step</th>
<th>Action</th>
<th>Purpose</th>
</tr>
</thead>
<tbody>
<tr>
<td><strong>1. Isolate Problem</strong></td>
<td>Identify which component is failing</td>
<td>Modern AI has many components (retrieval, prompting, model
params)</td>
</tr>
<tr>
<td><strong>2. Use Traces</strong></td>
<td>Inspect inputs/outputs of each component</td>
<td>Pinpoint root cause (e.g., ineffective retrieval, poor prompt)</td>
</tr>
<tr>
<td><strong>3. Unit Tests</strong></td>
<td>Implement component-level tests</td>
<td>Validate specific logic, catch regressions early</td>
</tr>
</tbody>
</table>

**Goal**: Turn evaluation into a process that helps teams ask better
questions and improve iteratively.

## Step 6: Red-Teaming

**Responsible**: Product Owner (with Engineering, QA, or Security/Ethics
Team support)

Product Owner ensures red-teaming is conducted and prioritizes
remediation. Technical teams execute adversarial testing.

**What is red-teaming?** Structured adversarial testing to proactively
discover vulnerabilities, biases, and failure modes before users do.
Think like a malicious actor, confused user, or edge-case generator.

## Step 6: When is Red-Teaming Critical?

<table>
<colgroup>
<col style="width: 41%" />
<col style="width: 58%" />
</colgroup>
<thead>
<tr>
<th>Scenario</th>
<th>Why Critical</th>
</tr>
</thead>
<tbody>
<tr>
<td><strong>Agentic/Flexible Solutions</strong></td>
<td>More pathways for failure (web browsing, code execution, multi-step
decisions)</td>
</tr>
<tr>
<td><strong>Long Conversation Histories</strong></td>
<td>Cumulative errors - small issue in turn 1 amplified by turn 10</td>
</tr>
<tr>
<td><strong>High-Risk Domains</strong></td>
<td>Maternal health, medical advice, financial planning - severe impact
of failure</td>
</tr>
<tr>
<td><strong>Population-Scale</strong></td>
<td>Unknown interaction patterns; improbable behaviors will occur at
scale</td>
</tr>
</tbody>
</table>

## Step 6: Red-Teaming Process

**Plan** → **Probe** → **Prioritize**

1.  **Plan**: Define goals, choose testers, decide where to test
2.  **Probe**: Adopt adversarial mindset, try to
    confuse/exploit/stress-test, capture failures
3.  **Prioritize**: Review by severity/likelihood, assign owners, rerun
    after fixes

**Resources**: [Red-Teaming AI for Social Good
Playbook](https://humane-intelligence.org/insights/research/#:~:text=UNESCO's%20Red%20Teaming%20Playbook%20is,promote%20ethical%20and%20inclusive%20AI.)
(UNESCO & Human Intelligence, 2024), [Planning Red-Teaming for Large
Language
Models](https://learn.microsoft.com/en-us/azure/ai-foundry/openai/concepts/red-teaming)
(Microsoft Learn, 2024)

## Level 2: Product Evaluation

**Question**: Does the product facilitate meaningful interactions?

**Why important**: Beyond evaluating how the AI model performs against
key metrics, organizations need to assess how well the product engages
real users and whether it solves a meaningful problem for the user. It
is unlikely that a product will shift development outcomes if it fails
to engage its users. Like model evaluation, this type of evaluation is a
continuous and iterative process, rather than one-off.

Technology companies frequently evaluate and improve products by
collecting user interaction metrics and then running rapid cycles of
digital experiments. For example, they may track a user’s journey on a
website, automatically collecting records like which products users
click on and whether they return to the site. Then, they can compare how
different web or app experiences affect browsing time or user
satisfaction.

**Unique advantages of digital**: This rapid, iterative process is
enabled by two factors unique to digital interventions: (1) iterations
of the product can be precisely and efficiently deployed to different
users, and (2) on-platform engagement outcomes are costless to collect
and transform into meaningful engagement metrics.

## Who is Most Involved?

<table>
<colgroup>
<col style="width: 27%" />
<col style="width: 72%" />
</colgroup>
<thead>
<tr>
<th>Role</th>
<th>Responsibility</th>
</tr>
</thead>
<tbody>
<tr>
<td><strong>Product Managers</strong></td>
<td>Execute - Directly responsible for product metrics</td>
</tr>
<tr>
<td><strong>Data Scientists</strong></td>
<td>Support - Apply evaluation methods</td>
</tr>
<tr>
<td><strong>Engineers</strong></td>
<td>Support - Build and roll out features</td>
</tr>
</tbody>
</table>

## Evaluation Methods

- **A/B testing**: Feature A vs. Feature B
- **Multi-armed bandit**: Performance-based adaptive allocations
- **Holdout testing**: AI vs. non-AI; status quo vs. accumulated
  improvements

**Resources**: [AI4GD A/B Testing
Playbook](https://docs.google.com/document/d/1_i1LjHIA3MHBCez1gxvSqZohN9zkwjG09h5L2k4BryQ/edit?tab=t.0#heading=h.wdgt1uho9q75),
[AI4GD User Funnel and Metrics
Playbook](https://docs.google.com/document/u/0/d/18OFMLI70IZLQuwhuxTwZXrDhw6Z-kpT-QUqZZJugEZ4/edit)

## Measurement Tools: Categories

<table>
<colgroup>
<col style="width: 30%" />
<col style="width: 39%" />
<col style="width: 30%" />
</colgroup>
<thead>
<tr>
<th>Category</th>
<th>Metric Type</th>
<th>Examples</th>
</tr>
</thead>
<tbody>
<tr>
<td><strong>Retention</strong></td>
<td>User-Level Retention</td>
<td>DAU/MAU, session count</td>
</tr>
<tr>
<td><strong>Engagement</strong></td>
<td>Action-Based</td>
<td>Response rate, clicks, rewrites</td>
</tr>
<tr>
<td><strong>Engagement</strong></td>
<td>Interaction Duration</td>
<td>Session length, conversational turns</td>
</tr>
<tr>
<td><strong>Engagement</strong></td>
<td>Feature Uptake</td>
<td>Click-through to links, feature use</td>
</tr>
<tr>
<td><strong>Non-Engagement</strong></td>
<td>Quality Scores</td>
<td>Toxicity score, informativeness</td>
</tr>
<tr>
<td><strong>Non-Engagement</strong></td>
<td>Item-Level Surveys</td>
<td>“Helpful” ratings, “want more” votes</td>
</tr>
<tr>
<td><strong>Non-Engagement</strong></td>
<td>User-Level Surveys</td>
<td>Overall satisfaction, usability</td>
</tr>
<tr>
<td><strong>Non-Engagement</strong></td>
<td>User Control</td>
<td>Topic subscriptions, filtering</td>
</tr>
</tbody>
</table>

## Level 3: User Evaluation

**Question**: Does the product positively support users’ thoughts,
feelings, knowledge, and behaviors?

**Why important**: Once product functions correctly (Level 1) and
engages users (Level 2), ask:

**Is it changing how users think, feel, or act?**

User psychological and behavioral changes are early indicators of
long-term development goals. These evaluations are faster and cheaper
than full impact evaluations, allowing rapid iteration.

## Level 3: Focus Areas

<table>
<colgroup>
<col style="width: 17%" />
<col style="width: 28%" />
<col style="width: 54%" />
</colgroup>
<thead>
<tr>
<th>Area</th>
<th>Question</th>
<th>Example Constructs</th>
</tr>
</thead>
<tbody>
<tr>
<td><strong>Cognitive</strong></td>
<td>Are users gaining new knowledge or correcting misconceptions? Do
they demonstrate improved skills or decision-making ability as a result
of using the AI?</td>
<td>Users’ comprehension, reflection, reasoning, and perceived clarity
or understanding during interaction</td>
</tr>
<tr>
<td><strong>Affective</strong></td>
<td>How does the product make users feel? Do users report feeling
supported, motivated, and capable after interactions, or are there
indications of frustration, confusion, or emotional distress?</td>
<td>Mood, sense of belonging, perceived empathy, trust, or comfort
interacting with AI</td>
</tr>
<tr>
<td><strong>Behavioral</strong></td>
<td>Are users taking small but meaningful actions (e.g., asking more
questions, trying out recommended behaviors) that would predict their
longer-term development?</td>
<td>Users’ acquisition, recall, and application of factual or procedural
information, and observable behaviors (e.g., asking more questions,
trying out recommended behaviors) that are proxies for longer-term
development outcomes</td>
</tr>
</tbody>
</table>

## Who is Most Involved?

<table>
<colgroup>
<col style="width: 27%" />
<col style="width: 72%" />
</colgroup>
<thead>
<tr>
<th>Role</th>
<th>Responsibility</th>
</tr>
</thead>
<tbody>
<tr>
<td><strong>Psychologists, UX Researchers</strong></td>
<td>Execute - Apply evaluation methods</td>
</tr>
<tr>
<td><strong>Data Scientists</strong></td>
<td>Support - Design A/B tests and experiments</td>
</tr>
</tbody>
</table>

## Evaluation Methods

- A/B testing: Feature A vs. Feature B
- Multi-armed bandit: Performance-based adaptive allocations
- Holdout testing: AI vs. non-AI

## Measurement Tools: 4 Categories

1.  **On-Platform Behavioral Measures**:

    - Frequency and depth of queries
    - Changes in language complexity
    - Follow-up question rate
    - Session duration & return rate
    - Feature utilization and AI suggestions followed

2.  **Short Self-Report Surveys**: Validated scales, brief and specific,
    integrated into flow

3.  **NLP and Text Analysis**: Sentiment analysis, topic modeling, LIWC,
    LLM-based analysis

4.  **Off-Platform Measures**: Longer surveys, observer reports,
    objective performance data

## Level 4: Impact Evaluation

**Question**: Does the product improve development outcomes?

**Why important**: IEs measure effects on outcomes like mortality,
learning, and earnings. The challenge: many things happen
simultaneously, making simple before-and-after comparisons unreliable.

**Solution**: Use a **counterfactual** - a similar sample that didn’t
receive the intervention. This captures what would have happened without
the intervention, allowing us to isolate the intervention’s impact.

## Level 4: Counterfactual Methods

<table>
<colgroup>
<col style="width: 25%" />
<col style="width: 41%" />
<col style="width: 32%" />
</colgroup>
<thead>
<tr>
<th>Method</th>
<th>Description</th>
<th>Best For</th>
</tr>
</thead>
<tbody>
<tr>
<td><strong>RCT</strong></td>
<td>Random assignment to treatment/control</td>
<td>Most credible; gold standard</td>
</tr>
<tr>
<td><strong>Propensity Score Matching</strong></td>
<td>Match on observable characteristics</td>
<td>When randomization not possible</td>
</tr>
<tr>
<td><strong>Difference-in-Differences</strong></td>
<td>Compare trends before/after</td>
<td>When parallel trends assumption holds</td>
</tr>
<tr>
<td><strong>Regression Discontinuity</strong></td>
<td>Compare units just above/below cutoff</td>
<td>When cutoff exists and is exogenous</td>
</tr>
</tbody>
</table>

**RCTs** are the most credible way to determine causal impact. Random
assignment ensures differences can be attributed to the intervention,
not population differences or external factors.

## Who is Most Involved?

<table>
<colgroup>
<col style="width: 27%" />
<col style="width: 72%" />
</colgroup>
<thead>
<tr>
<th>Role</th>
<th>Responsibility</th>
</tr>
</thead>
<tbody>
<tr>
<td><strong>Policy Researchers, Economists</strong></td>
<td>Execute - Apply evaluation methods</td>
</tr>
<tr>
<td><strong>AI Engineers</strong></td>
<td>Support - Ensure product functions as expected</td>
</tr>
</tbody>
</table>

## Why Do an Impact Evaluation?

There are 3 main reasons to do an impact evaluation:

1.  **Proof of concept**: By isolating the effect of the intervention
    from the rest of the world, the impact evaluation allows you to
    causally attribute changes in outcomes to the intervention - giving
    you proof of concept.

2.  **Proof in different settings**: Once you know it works in a
    particular setting, with a particular target population, you may
    want to show it will work in other settings or for other
    populations - then you can do additional impact evaluations.

3.  **Cost-benefit analysis**: For many funders and public sector
    partners, IEs are critical for decision-making. They want credible
    evidence that a product meaningfully improves people’s lives -
    beyond engagement metrics or self-reported satisfaction - before
    committing to scale. A well-designed IE sends a strong signal that
    your product works in real-world conditions, and that scaling it is
    likely to generate meaningful social returns (see e.g. [Hauser et
    al.,
    2025](https://www.nature.com/articles/d41586-025-02266-7.epdf?sharing_token=jCKO3Tx8dFeQfucqP5VCcNRgN0jAjWel9jnR3ZoTv0PS1htX8Sko7IudKf1MVjrKQ-g3NeuYAsnuJ-Io9wHN3uMBrjSLLnu_wjpJLF2G-unWgOw27UqLqC_yalnt2AFTYmMZAO31agMcWvNwKRpfYsfrMt3fmIKm0iVbftxqAsY%3D);
    [UK GOV,
    2025](https://www.gov.uk/government/publications/the-magenta-book/guidance-on-the-impact-evaluation-of-ai-interventions-html)).

IEs also help funders compare across opportunities. When paired with
cost data, they allow for robust estimates of cost-effectiveness and
cost-benefit analysis - crucial when governments, donors, and
multilateral institutions are allocating scarce resources. In many
cases, the result of an IE becomes a key input in decisions to scale,
replicate, or exit.

**Important**: It is important to be clear on why you are doing the
impact evaluation at the outset, as this will affect the data you
collect and how you design the evaluation. For example, if you are doing
a proof of concept evaluation, you may want to invest more in collecting
a rich set of outcomes in your Level 3 evaluations to understand how
these map to ultimate welfare outcomes.

## When is it Appropriate?

IEs are high-investment undertakings, both financially (they often cost
millions of dollars) and operationally (service providers have to adapt
their operations, often in challenging ways, to make them work). They
are most useful when your product is mature enough to test and when the
decision stakes are high enough to justify the effort.

**In general, consider an IE when**:

- **Levels 1-3 are strong**: The model performs well, users engage
  meaningfully, and early evidence suggests improvements in knowledge,
  attitudes, or behavior.
- **You are preparing to scale**: Funders or policymakers are
  considering wider adoption, but want evidence, including
  cost-effectiveness or cost-benefit estimates, to support the decision.
- **You have bandwidth**: Implementing an IE is a lot of work for both
  the research team and implementer; doing it well takes time and
  effort.
- **You are confident your product works**: The world may be uncertain
  that your product has a meaningful impact, but you shouldn’t be. Your
  earlier stage evaluations should give you confident priors that you’ll
  find effects on development outcomes.

## When is it Appropriate?

**You do NOT need to run an IE if** your product is still in early
design or if usage is inconsistent to the point where you are worried
about impacts. In those cases, Level 3 evaluations can be more
appropriate.

## Plan for Evaluability Early

Although impact evaluations are typically conducted at later stages,
designing credible and cost-effective IEs often requires thinking about
design decisions far earlier in the process. Incorporating features like
holdout groups, staged rollouts, or embedded randomization into the
initial product architecture (which could also be useful for A/B tests)
ensures that rigorous causal evaluation remains possible - without
requiring disruptive redesigns later on.

Even if a full IE is not yet justified, these design choices create
structured opportunities for credible inference when the time comes and
can significantly reduce the burden of evaluation. Funders assessing
scale readiness should look for these signals of early evaluability.

## How to Do an IE Responsibly

Rigorous IEs require expertise. We recommend working with an
**independent evaluator** - such as an academic partner, a research NGO
(e.g., J-PAL, IPA), or a third-party M&E firm. This enhances both the
technical quality and the perceived credibility/independence of your
evaluation.

**At a minimum, we suggest**:

- **Clarifying roles**: Who builds the product, who runs the study, who
  communicates findings
- **Pre-registering the design**: On platforms such as the AEA RCT
  Registry, EGAP, or RIDIE
- **Sharing results transparently**: Disclose all findings, including
  null or negative results, and make methods and materials publicly
  available where feasible to support reproducibility and sector-wide
  learning

## Impact Evaluation Methods

1.  **Randomized Control Trials**: Random assignment to
    treatment/control
2.  **Propensity Score Matching**: Match on observable characteristics
3.  **Difference-in-Differences**: Compare trends before/after
    intervention
4.  **Regression Discontinuity Design**: Compare units just above/below
    cutoff

**Resources**: [Impact Evaluation in
Practice](https://openknowledge.worldbank.org/server/api/core/bitstreams/4659ef23-61ff-5df7-9b4e-89fda12b074d/content)
(Gertler et al., World Bank), [Running Randomized
Evaluations](https://www.amazon.co.uk/Running-Randomized-Evaluations-Practical-Guide/dp/0691159270)
(Glennerster & Takavarasha)

**Focus**: What is distinctive when evaluating AI-based products

## Key Design Consideration 1: Counterfactual Selection

**Options**:

- **Pure control**: No intervention at all

- **Business-as-usual**: No digital support or sporadic human guidance

- **Non-AI digital tools**: Static chatbots or curated content

- **Human-delivered services**: When AI substitutes for scarce labor
  (measure costs: [Cost Measurement
  Guide](https://www.worldbank.org/en/programs/sief-trust-fund/brief/cost-measurement))

**Important**: Justify selection and explain what it helps illuminate

## Key Design Consideration 2: Measuring Latent Access

**Critical**: Marginal benefit depends on what other support users
already have

**Measure**:

- Existing technology use (frequency, type, purpose)

- What users rely on today (informal networks, human advisors, basic
  tech)

- Leakage - how much control group has access to intervention

**Why**: Shapes incremental value added by AI product

## Key Design Consideration 3: Managing Product Dynamism

**Challenge**: SUTVA assumption (same version for all treated units)
often violated

**AI products**: Designed to improve iteratively - different
participants may interact with different versions

**Solutions**:

- Tag your versions

- If A/B testing, randomize test participation

- Maintain hold-out group on baseline version

-Pre-specify at high level (not overly detailed)

## Key Design Consideration 4: Measuring True Development Outcomes

**Challenge**: AI tools often simulate expertise - does user learn or
just copy?

**Solutions**:

- Use industry-standard validated assessments

- Use administrative data

- Avoid measures that can be gamed by repeating AI output

- Test ability when users don’t have access to AI

## Key Design Consideration 5: Managing Spillovers and Contamination

**Challenge**: AI tools designed for scale - freely accessible, easy to
share

**Strategies**:

- **Controlled access**: Individual or cluster assignment

- **Publicly available**: Randomized encouragement design

- **High contamination risk**: Run in settings with low existing
  exposure

- **Cluster randomization**: By school or clinic

- **Monitor usage**: Be prepared to adjust power calculations

## Common Pitfalls to Avoid

1.  **Being underpowered**: Test uptake with small groups, bring
    pessimists into planning
2.  **Mismanaging transparency**: Balance rigor and responsiveness
3.  **Letting product evolution obscure analysis**: Pre-specify how
    changes handled analytically
4.  **Underestimating attrition risks**: Track engagement from start,
    plan for dropouts

## Summary: The Four-Level Framework

**Level 1 - Model**: Does the AI model produce desired responses? -
Rubric → Metrics → Golden Dataset → Automated Evals → Refine → Red-team

**Level 2 - Product**: Does the product facilitate meaningful
interactions? - A/B tests, engagement metrics, retention, feature uptake

**Level 3 - User**: Does product support thoughts, feelings, knowledge,
behaviors? - Cognitive, affective, behavioral outcomes via surveys, NLP,
behavioral measures

**Level 4 - Impact**: Does access improve development outcomes? - RCTs
and other methods to measure causal impact on mortality, learning,
earnings

## Key Principles

1.  **Continuous evaluation**: Rapid, ongoing cycles, not one-off
    experiments
2.  **Cross-functional teams**: All four perspectives must be
    represented
3.  **Building blocks**: User funnels, ETL pipelines, targeted
    hypotheses, experiments
4.  **Complementary methods**: All levels work together at different
    stages
5.  **Right-sized evaluation**: Make informed tradeoffs about what’s
    “enough”

## Additional Resources

**Level 1 Case Studies**: - [Generative AI for Health in Low & Middle
Income
Countries](https://cdh.stanford.edu/generative-ai-health-low-middle-income-countries) -
[Evaluation framework of PROMPTS at Jacaranda
Health](https://cdh.stanford.edu/generative-ai-health-low-middle-income-countries) -
[Evaluation framework at Precision
Development](https://precisiondev.org/evaluating-ai-for-learning-a-framework/)
([slides](https://docs.google.com/presentation/d/1agCgpDWNVWtbOFhdlDYUpLM3OxyHP5CxyzON_tn61x0/edit?slide=id.p#slide=id.p)) -
[Evaluation of Farmer.Chat at Digital
Green](https://arxiv.org/abs/2409.08916) - [Evaluation of mMitra at
Armman](https://docs.google.com/presentation/d/1mAF1lI8tkTjLLW3SjwrV8mdz4VDkTdog/edit?slide=id.p1#slide=id.p1)

**Level 3 Case Studies**: - [ChatSEL
Documentation](https://agency-fund.github.io/chatsel-docs/docs/t1-intro) -
[User Evaluation Workshop -
ChatSEL](https://docs.google.com/document/d/18AXtIeDx6HsidhMKTJ2kIDb7hUwHEkEnwGPZuC9JJo0/edit?tab=t.0)

## Questions?

**Authored by:** - **[The Agency Fund](https://www.agency.fund/)**  
- **IDInsight**  
- **[Center for Global Development](https://www.cgdev.org/)**

**November 2025**

Please reach out to [Zezhen Wu](mailto:zezhen@agency.fund) for questions
or comments.

*This is a living playbook. Current version grounded in lessons from
[AI4GD accelerator
teams](https://theagencyfund.substack.com/p/ai-for-global-development-accelerator)
and experts across disciplines.*
