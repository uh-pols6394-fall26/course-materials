# Social Science Computation and Data Science

**POLS 6394 | Fall 2026**
**University of Houston**

**Instructor:** Boris Shor
**Email:** bshor@uh.edu
**Website:** https://bshor.github.io/
**Office:** PGH 396
**Office Hours:** By appointment via Calendly
**Teaching Assistant:** Amanda Austin (in class at every meeting)

**Class Meeting:** Tuesday/Thursday 1:00–2:20 PM
**Location:** PGH 310
**Required:** A laptop, brought to every class meeting

---

## Course Description

This course teaches the practical side of working with data and computing resources — the craft that surrounds statistics but is rarely taught alongside it. Our methods sequence teaches you the minimum R needed to estimate models; this course teaches everything around that: writing real programs, managing and acquiring data, producing publication-quality documents and websites, collaborating and version-controlling your work, and using modern AI tools productively and critically. These are the skills academics otherwise pick up slowly, badly, or never — and for students headed to non-academic careers, they are concrete, marketable skills that belong on a CV.

The semester has two parts. In **Part I (weeks 1–10), AI tools are strictly prohibited.** You'll learn to do the work by hand: the tidyverse, programming, version control, the command line, APIs, and interactive applications. In **Part II (weeks 11–14), AI tools are required.** You'll use chat assistants, IDE copilots, and programmatic LLM access, with three sessions centered on **agentic coding through Codex**. You'll use it on real work, including your own final project. You'll also use LLMs as research instruments, including live demonstrations of synthetic survey respondents from my forthcoming Cambridge book on LLMs for public opinion research.

Here's why: you cannot supervise a tool you cannot understand at a deep level. AI coding tools are enormously productive for someone who can read code, debug it, and recognize wrong output. For someone who can't do those things yet, they're risky because the errors look just like the successes. Part I gives you the skills you need for Part II.

R is the course's primary programming language. We also work directly with Quarto, git, GitHub, YAML, and the command line. We start on Posit Cloud, so there's nothing to install on day one.

## Instructional Approach

This is a hands-on skills course, not a discussion seminar and not a lecture course. Each 80-minute class mixes guided instruction with lab time — roughly half and half — and you'll write code in every single class meeting. We work in shared Quarto documents with deliberate blank space: I demonstrate, then you fill in the gaps while Amanda and I circulate. The first session of each instructional pair introduces new material; the second extends it and is more lab-heavy. There is no class on September 3.

Bring your laptop to every class. You can't pass this course without attending it: a large share of your grade is earned by work committed and pushed during class time.

## Learning Objectives

By the end of the semester, students will be able to:

- Organize a research project as a reproducible pipeline in R and Quarto, from raw data to a published paper, presentation, and website
- Use git and GitHub fluently for version control, collaboration, and reproducible research
- Write real programs in R using functions, iteration, vectorization, and debugging, and understand when parallel execution is worthwhile
- Wrangle, join, reshape, and visualize data with the tidyverse at a professional level
- Acquire data through web APIs — authentication, rate limits, JSON, and the political science API landscape — and supervise AI-written scrapers for sites without one
- Work hands-on at the command line and, if the course server is available, through SSH on a shared Linux system—not just in a GUI on a laptop
- Build a simple Quarto dashboard; read and modify a small Shiny application; and share work through GitHub Pages or Posit Connect Cloud
- Work with an agentic coding tool (Codex) on a real research project: scoping tasks, steering with project conventions, reviewing agent-written code, and verifying results
- Write a full academic paper in Quarto — sections, cross-references, and a managed BibTeX bibliography (JabRef + Google Scholar) — rendered to journal-ready formats
- Use AI tools — chat, copilots, and programmatic LLM APIs — productively, verifiably, and critically, including as research instruments for measurement and annotation
- Articulate where AI assistance helps, where it fails, and how to verify its output

---

## Course Requirements

*Preliminary — weights may be adjusted before the first day of class.*

| Component | Weight |
|-----------|--------|
| In-class lab work (committed and pushed before leaving class) | 10% |
| Take-home problem sets (7 or 8, submitted via GitHub) | 15% |
| Part I midterm practical (in class, October 29 — AI off) | 15% |
| Part II final practical (exam period, December 14 — AI required) | 15% |
| Problem-set walkthroughs | 5% |
| Part II AI-critique assignments (2) | 10% |
| Semester research and portfolio project | 30% |

Your lowest score is dropped separately in each of these three categories: in-class lab work, take-home problem sets, and problem-set walkthroughs.

### In-Class Lab Work (10%)

Before class, you'll receive that session's Quarto workbook. Keep it open for guided notes and follow-along exercises while I teach, then continue in the same file during the lab block and finish with a short learning/error log. Amanda and I will circulate, answer questions, and help you locate problems. You submit the whole workbook by committing and pushing it before leaving class. Guided notes and the closing log are graded for good-faith completion, not correctness; a documented failed attempt is worth full credit, while an empty document is not. Solutions are released after the submission deadline.

### Take-Home Problem Sets (15%)

Seven or eight take-home problem sets extend the lab work; the full schedule will be posted during Week 1. Unless the schedule gives a later date, a problem set is due at **10:00 AM on the day of the next class**. They are submitted as pull requests in your private course repository and graded for good-faith completion rather than polish. We may begin class by discussing approaches, common errors, or questions from the submitted work.

Questions are welcome. Show me what you tried and what you expected. I will clarify the prompt, help identify where an error begins, and point you toward a relevant example or piece of documentation. Amanda will provide the same help during class. I will not supply a finished pipeline or debug a blank file. You may discuss a problem and troubleshoot with classmates, but each student submits their own code. The walkthroughs draw directly from recent problem sets.

The Part I AI rule applies to take-home problem sets. These sets prepare you for the walkthroughs and midterm; using AI instead of doing the work will leave you unprepared for both.

### Part I Midterm Practical (15%)

The second half of class on **Thursday, October 29** — the last day of Part I — is a supervised practical: a realistic task (import a dataset you have not seen, clean it, summarize it, produce one polished figure) done solo, in the room, with AI off. Documentation and your own past work are fair game. Committed, sensible, unfinished work earns most of the credit; time pressure is handled generously.

### Part II Final Practical (15%)

During the **exam period (Monday, December 14)**, alongside your final presentation, you sit a supervised practical in which AI use is **required**. You get a task you haven't seen and about 35–40 minutes with your full toolkit — Codex, chat, and the API. Grading is based on whether the result is verified correct and on a short account of what the AI got wrong and how you caught it.

If a UH-recognized excused absence prevents you from taking either practical at the scheduled time, contact me to arrange a rescheduled practical. Labs, problem sets, and walkthroughs are covered by the dropped-score rule rather than individual absence makeups.

### Problem-Set Walkthroughs (5%)

About four times during the semester, I will schedule a short conversation with you about a recently submitted problem set. You will have your code, output, and notes open. I will ask you to explain what the task required, walk through one pipeline or choice, interpret the result, and consider a small change to the input. You will not be asked to write code from a blank screen.

The aim is explanation and diagnosis, with no reward for speed. Finding an error while explaining your work and describing how you would correct it demonstrates understanding. I will identify the relevant problem in advance so you can review your submission.

### Part II AI-Critique Assignments (10%)

In Part II, AI use is required. Two take-home assignments are graded on your supervision of the tool rather than the tool's output. **Assignment 1** (assigned November 5; due before class November 10) is the written version of the November 5 scraper lab: submit the scraper and a critique memo explaining what the AI got wrong, how you caught it, and what you verified by hand. For **Assignment 2** (assigned November 19; due December 3), you **build your own eval**: design 10–20 test prompts with ground truth and a scoring rule on a task from your own research domain, run it with GPT-5.6 Luna and GPT-5.6 Terra, and submit the mini leaderboard plus a memo on what the gap means. An eval is a systematic, quantified test of a model on *your* task.

### Semester Research and Portfolio Project (30%)

The capstone is **a paper of your own that you work on throughout the semester**. You can use a dissertation prospectus (or a chapter of one), a seminar paper you owe another course, a working paper, an MPP capstone, or whatever else you actually need to write this semester. **You must author it end-to-end with this course's tools.** By December you'll have a reproducible repository, a managed bibliography, the paper rendered to PDF, a revealjs presentation, and a simple Quarto dashboard. A suitable Shiny app may substitute if your project benefits from server-side interaction. **If your project does not naturally support a data pipeline, first figure, or dashboard, propose an alternative computational artifact in your September 29 project plan for instructor approval.**

The package also includes your data-driven CV and academic website, first made functional in Week 6 and then maintained through the semester. The site must render correctly, but public deployment is your choice; posting the rendered CV is also optional. By December the site should present you and the work you would want to make public. You present the research project during the final exam period. AI tools are permitted from Part II onward, and the repo must include an AI-use statement. **If an LLM measures anything in your paper—annotations, classifications, synthetic responses—your repository must contain the eval that justifies it** (the human-labeled subset, the scoring code, the agreement numbers).

The 30% is divided as follows:

| Project component | Weight |
|-------------------|--------|
| Final paper and reproducible repository | 18% |
| On-time, good-faith milestone work | 4% |
| Dashboard or approved alternative computational artifact | 3% |
| Presentation and defense | 3% |
| Updated CV and website | 2% |

Milestones are progress checks, not polished submissions. The milestone portion is graded for timely, good-faith completion; each checkpoint should show the specified work in the repository even if it still needs revision.

**Milestones (each is a commit in your paper repository):**

| Date | Deliverable |
|------|-------------|
| Thu Sep 10 (Week 3) | **Paper repo exists** with a one-paragraph topic statement (README) |
| Tue Sep 22 (Week 4) | **Materials in hand**: raw data committed (or documented if unshareable) and the first cleaning script runs; for a data-light project, essential sources or other project materials are acquired and organized |
| Tue Sep 29 (Week 5) | **Project plan** (1 page): question, materials, intended analyses, and outputs; request approval here for any alternative to the default pipeline, figure, or dashboard |
| Tue Oct 6 (Week 6) | **Paper skeleton** renders to PDF with a managed `.bib`, at least three real citations, and a first figure or approved equivalent |
| Tue Oct 13 (Week 7) | **Professional materials**: CV and minimal website both render; public deployment and a public CV link are optional |
| Thu Nov 5 (Week 11) | **First real result**: the current pipeline runs end-to-end on your own materials and produces one real result or approved equivalent |
| Thu Nov 19 (Week 13) | **Repository check**: pipeline runs end-to-end from a clean clone and a full draft renders. A good-faith complete attempt may correct reproducibility problems identified by this check through December 1 without penalty. |
| Mon Dec 14, 2:00–4:00 PM | Exam period: **final practical** (~35–40 min, AI required) + **presentation** (revealjs, from your repo); final paper, repository, dashboard or approved alternative, AI-use statement, and **updated CV + website** due |

---

## Materials and Costs

There is no required textbook to purchase. The backbone readings are free, current, and online:

- Jenny Bryan, *Happy Git and GitHub for the useR* — happygitwithr.com
- Chester Ismay, Albert Y. Kim, and Arturo Valdivia, *ModernDive: Statistical Inference via Data Science*, 2nd ed. — moderndive.com/v2
- Kieran Healy, *Data Visualization: A Practical Introduction*, 2nd ed. draft — socviz.co
- Kieran Healy, *The Plain Person's Guide to Plain Text Social Science* — plain-text.co
- Hadley Wickham et al., *R for Data Science*, 2nd ed. — r4ds.hadley.nz (reference)

Recommended for your permanent shelf (not required): Edward Tufte, *The Visual Display of Quantitative Information*.

**About readings in this course:** this is a skills course, and its readings look like the field's actual conversation — **blog posts and sections of free online books**, plus a small number of journal articles (provided as PDFs). Expect posts by working quantitative social scientists on both sides of the AI-in-research controversy, chapters from the online books above, and classics on replication as the scientific standard. Readings are short, assigned per week, and fair game for discussion.

**Required course costs (~$50 total, in place of a textbook):**

1. **Two months of ChatGPT Plus (~$20/month, ~$40 total)** covering November and December — this provides **Codex**, the agentic coding tool at the center of Part II (the subscription's agent-usage limits go further than the alternatives), plus the chat interface used throughout Part II and your final project.
2. **~$10 of OpenAI API credit** for the programmatic LLM work (the ellmer/silicon-sampling week and any API use in your final project). GPT-5.6 Luna is the workhorse for routine and batch calls; GPT-5.6 Terra is used for the comparison eval and harder tasks.

Both purchases are with one vendor (OpenAI); note the API credit is billed separately from the Plus subscription.

You'll also need: a laptop you can bring to every class, a free GitHub account, and a Posit Cloud account (free tier to start; the course provides a shared workspace).

---

## Schedule of Classes

*Preliminary. The first meeting of each instructional pair introduces; the second extends and practices. There is no class on September 3. Readings are listed as preparation; the working materials are Quarto documents distributed via the course repository.*

## Part I: Computing Without a Copilot (Weeks 1–10)

*Strict no-AI policy in effect — see AI Policy below.*

### Week 1 (August 25, 27): The Plain-Text Research Life

Why this course exists and why Part I bans AI. Posit Cloud orientation; RStudio and projects; files, folders, and the anatomy of a reproducible pipeline. On Thursday, create a short Quarto paper and presentation, then publish one of them to Posit Connect Cloud.

**Read:** Healy, *Plain Person's Guide*, chs. 1–2, 4, 7 (skip the Emacs material); Gentzkow & Shapiro, *Code and Data for the Social Sciences: A Practitioner's Guide* (2014), chs. 1–3 — why professionals organize code and data the way this course will make you.

### Week 2 (September 1, 8): Git and GitHub

Version control as the researcher's safety net: commit, push, pull; connecting RStudio to GitHub; burn-it-all-down recovery. The course pull-request workflow starts here and is used for every submission thereafter.

**There is no class on Thursday, September 3.** The course resumes Tuesday, September 8.

**Read:** Bryan, *Happy Git*, “Why Git? Why GitHub?,” “Repo, Commit, Diff, Tag,” and “Early GitHub Wins.”

### Week 3 (September 10, 15): Tidyverse I — Wrangling

Importing data; identifying the observational unit, identifiers, and measurements; the dplyr verbs; pipes; cleaning with janitor, inspecting with skimr, narrating with tidylog.

**Read:** ModernDive §§1.4 and 3.1–3.4; *R4DS* chs. 1, 3–4 (reference as needed). **Optional practice:** Heiss's interactive primers on [tibbles](https://r-primers.andrewheiss.com/transform-data/01-tibbles/), [isolating rows](https://r-primers.andrewheiss.com/transform-data/02-isolating/), and [deriving variables](https://r-primers.andrewheiss.com/transform-data/03-deriving/).

### Week 4 (September 17, 22): Tidyverse II — Reshaping and Joining

Joins with single and composite keys; checks for duplicate and unmatched keys; pivots; strings, dates, and factors — the operations real projects live on.

**Read:** ModernDive ch. 4. **Optional practice:** Heiss's interactive primer on [reshaping data](https://r-primers.andrewheiss.com/tidy-data/01-reshape-data/).

### Week 5 (September 24, 29): Visualization

ggplot2 from grammar to publication polish: aesthetics, layers, facets, scales, themes, annotation. Compressed and fast — this is a full course elsewhere (I teach it at ICPSR); here it is one intense week.

**Read:** Healy, *Data Visualization* 2e draft, chs. 3–5. ModernDive ch. 2 and Heiss's [visualization primer](https://r-primers.andrewheiss.com/basics/01-visualization-basics/) are optional practice.

### Week 6 (October 1, 6): Writing and Publishing — Papers, Bibliographies, CV, Website

**October 1 is the paper session:** building a full academic paper in Quarto — sections, figures and tables with cross-references, footnotes, citations — rendered to HTML, PDF, and Word, working from a complete example paper. Central to it is **bibliography management as a workflow**: BibTeX as plain text, **Google Scholar** as the citation source, and **JabRef** as the reference manager that owns your `.bib` file across every paper you will ever write. **October 6 is the publishing session:** sharing work through Posit Connect Cloud and building an academic site with Quarto and GitHub Pages.

The October 6 lab produces two functional drafts. First, a **real academic CV**: we start from the [`christopherkenny/quarto-cv`](https://github.com/christopherkenny/quarto-cv) template (MIT-licensed; PDF via Typst), driven by YAML and BibTeX data files. Second, a **one-page academic website**: you copy the course's [minimal Quarto starter](https://github.com/bshor/cv-minimal-site), which contains simple places for a picture, publications, working papers, and teaching, and replace its placeholders. You may deploy it publicly to `yourname.github.io` or keep the source private and demonstrate the rendered site locally. A public-safe `cv.pdf` link is optional. The starter credits Gang He's MIT-licensed Quarto academic website template. The session is an 80-minute terminal workshop.

### Week 7 (October 8, 13): Programming I — Functions and Iteration

Writing functions; vectorization; control flow; iterating with purrr. The week the course shifts from *using* R to *programming* R.

### Week 8 (October 15, 20): Programming II — Debugging, the Shell, and Scale

Debugging and basic error handling; hands-on command-line work — navigation, files, wildcards, interrogating a CSV without opening R, and running R non-interactively with `Rscript`. A fresh R process exposes scripts that depend on objects or settings left behind in an interactive session. We then clone a small repository created by someone else, follow its instructions, restore its R packages from an `renv.lock` file, and try to reproduce its result. Parallel execution with future/furrr remains a short demonstration rather than a second workflow to master. Posit Cloud's terminal is the guaranteed baseline environment. If the course Linux server is available, students will also receive individual accounts and practice remote access with SSH.

### Week 9 (October 22, 27): Getting Data from APIs

Most data acquisition now starts with an API. Tuesday covers the fundamentals: what an API is, httr2, JSON, authentication and keys, rate limits, pagination, and turning nested responses into tidy data frames. Thursday tours APIs political scientists actually use, including Congress.gov, the Census via tidycensus, and FRED. We'll compare calling a REST API directly with using a client package and practice reading unfamiliar API documentation. We skip hand-written web scraping; in Week 11, we'll have AI write a scraper and then verify it ourselves.

### Week 10 (October 29, single session): Dashboards and Shiny in Forty Minutes; the Midterm Practical

First half: build a simple Quarto dashboard that combines headline values, an interactive figure, and a lookup table. We then run and make one small modification to a Shiny app with one selector and one plot. The take-home problem set extends the dashboard; a Shiny extension is optional. It is due at **10:00 AM November 3** and remains AI-free. Second half: the **Part I midterm practical** (see Course Requirements). This closes the in-class portion of Part I.

## Part II: Computing With AI (Weeks 11–14)

*AI tools are now required—see the policy below. Part II includes sustained, supervised work with Codex.*

### Week 11 (November 3, 5): The Controversy; LLMs and Assisted Coding

Part II opens by **teaching the controversy** over AI in research. This course allows it, but that should be a considered position rather than a default. We read working quantitative social scientists on both sides: the adoption case (Andrew Hall's *Free Systems*; Alexander Kustov's *Popular by Design*), the skeptics' case (peer-reviewed critiques of LLMs in research), and the standard that adjudicates between them, **replication** (King's classic statement; Gentzkow & Shapiro's *Code and Data*). Allowing AI in *research* is separate from allowing it in *training*; Part I's ban was pedagogy, not research ethics. We then cover how LLMs work well enough to know when to distrust them, the three interfaces (chat, IDE copilots, in-editor tools), prompting patterns, and the verification loop. In the lab, AI writes a web scraper and you verify its output against the page. *Specific readings are listed in the course repository (`Resources/`).*

### Week 12 (November 10, 12, 17): Agentic AI with Codex

We spend three sessions doing hands-on agentic work with the ChatGPT Plus subscription purchased for the course (see Materials and Costs). In the first, you'll learn the Codex terminal workflow, approval modes, and initial supervised tasks, with git as the safety net. The second covers AGENTS.md project conventions, planning before coding, breaking work into manageable tasks, reviewing diffs, and checking whether the agent did what it claims. In the third, you bring your functioning final-project repository and use Codex to build and verify a real piece of the pipeline before Thursday's diagnostic repository check.

### Week 13 (November 19; December 1): LLMs as Research Instruments

*No class November 24 or 26 — Thanksgiving week. Diagnostic repository check due Thursday November 19; good-faith attempts have through December 1 to correct reproducibility problems found by the check.* Silicon sampling: LLMs as synthetic survey respondents via ellmer and structured output, validated against real CCES respondents — a live demonstration from Kennedy, Shor, and Austin, *Large Language Models for Public Opinion Research* (Cambridge). Then LLM text annotation at scale: classifying open-ended responses and documents, with validation.

### Week 14 (December 3): RAG, Local Models, and Wrap

We start with **retrieval-augmented generation (RAG)**: grounding an LLM's answers in a document corpus such as bills, speeches, or platforms. The demonstration uses `ragnar` with a real political-text corpus and shows what retrieval fixes and what it doesn't. We then turn to **local models**. Consumer hardware constrains model size and throughput, while hosted APIs make parallel batch work easier. Local models remain valuable when privacy or IRB constraints require them and when a pinned model file improves reproducibility. We close with privacy, cost, and a course wrap. Office hours this week and next are project clinics for the paper.

---

### Exam Period: Monday December 14, 2:00–4:00 PM

Two things in the two-hour slot: the **Part II final practical** (about 35–40 minutes, AI required, supervision graded) and four **final presentations** (about 12–15 minutes including Q&A for each student), with a transition and buffer between them. Final paper, repository, dashboard or approved alternative, AI-use statement, and updated CV + website all due the same day.

---

## Class Policies

### Course Repositories and Privacy

You'll work in three kinds of repository, split by who owns them and who can see them:

1. **Course materials** (slides, labs, data, problem-set prompts) live in a **public** repository — open courseware, like my ICPSR books.
2. **Your coursework** — labs, problem sets, and your semester paper — lives in **one private repository I create for you**, owned by the course organization. Only you, Amanda, and I can see it. Your drafts, dead ends, and mistakes are nobody else's business; this repo is your workshop, and every submission is a pull request inside it.
3. **Your website and CV are yours to keep after the course** (Week 6). Their source may live in private repositories. If you want a public professional site, deploy the website from your personal GitHub account to `username.github.io`; otherwise, render it locally and submit it privately. Posting a public-safe CV is optional. Do not publish a home address, personal phone number, or anything else you do not want indexed.

Setting all this up is the subject of Week 2 (coursework repo) and Week 6 (website + CV); until then, materials will be available on Posit Cloud. You'll need a free GitHub account — create one before the first class (any username you'd be comfortable putting on a CV).

### AI-Assisted Grading

I may use AI agents to assist with grading under rubrics I write and supervise. Agents run mechanical checks (does your repo render? do your results reproduce?) and draft rubric-based feedback, and I review every draft before any grade is assigned.

### AI Policy

**Part I assignments, including the dashboard problem set due at 10:00 AM on November 3: AI tools are prohibited.** No ChatGPT, no Claude, no Copilot, no AI autocomplete, no "just checking one error message." This includes problem sets done at home. Before Part I work begins, disable any generative autocomplete or assistant built into your editor or browser; Amanda or I will help you find the setting. Ordinary non-AI resources—documentation, books, Stack Overflow, package vignettes, your classmates, and me—are all fair game and encouraged.

**Part II (beginning with class on November 3): AI tools are required.** Assignments must be done with AI assistance, and the graded artifact is your supervision of it: verification, critique, and correction. You remain fully responsible for everything you submit — "the AI did it" is not a defense; catching what the AI did is the assignment.

**Data used with AI tools:** work from public, synthetic, or anonymized copies that would be safe to release publicly. Remove names, email addresses, phone numbers, street addresses, respondent contact information, and any key that connects records back to people. Random case ID numbers may remain when the linking key is not included. Check whether combinations such as a rare occupation, precise location, and exact age could still identify someone; coarsen, alter, or replace those fields in the AI-facing copy when needed. Keep the protected original outside any repository or folder an AI tool can access, and document any changes made to the working copy.

**Always, in both parts:** you must be able to explain any line of code you submit. Problem-set walkthroughs and the practicals give you opportunities to demonstrate this. Inability to explain submitted work may trigger an individual follow-up review and can result in loss of credit when you cannot establish authorship or understanding; it is evidence to investigate, not by itself a finding of academic dishonesty.

### Classroom Participation

Don't be afraid of saying something "wrong," and don't be afraid of asking questions — in a four-person skills course, your confusion is almost certainly shared, and surfacing it is a contribution. Amanda and I will both be present at every class, so ask for help as soon as you are stuck.

### Laptops and Classroom Etiquette

Keep your laptop on course work during class; texting and social media diminish the learning environment for everyone, and in a room this small, everyone notices. I'll do my best to start and end class on time; please make every effort to do the same.

### Office Hours

By Microsoft Teams appointment via [Calendly](https://calendly.com/bshor). We can talk about course material, your projects, your experience in the department, or your future plans. In the final weeks, office hours double as project clinics.

### Communication

Use Microsoft Teams chat for course questions and messages. I will also post class announcements in Teams, so check the course Team regularly.

### Civility

You are free to disagree, even strongly, with each other and with me. However, I expect and demand civility and kindness to each other in class.

### Letters of Recommendation

I am happy to write a letter of recommendation for any student who has done well in my course. I need at least three weeks' notice, and it is your responsibility to provide any necessary supporting paperwork.

### Excused Absences

Regular class attendance, participation, and engagement in coursework are important contributors to student success. Absences may be excused as provided in the University of Houston Graduate Excused Absence Policy for reasons including: medical illness of student or close relative, death of a close family member, legal or government proceedings that a student is obligated to attend, recognized professional and educational activities where the student is presenting, and University-sponsored activity or athletic competition.

### Religious Observance

If you have religious holidays which conflict with the class, this is fine, but send me a Teams chat message ahead of time.

### Academic Honesty

All students are expected to adhere to the University of Houston's Policy on Academic Honesty. Cheating and plagiarism in this class will be punished to the maximum extent possible; failure of the course at the very least. This course's AI Policy is part of its academic honesty expectations. See the University of Houston graduate handbook or [uh.edu/provost/stu/stu_syllabsuppl.html](http://www.uh.edu/provost/stu/stu_syllabsuppl.html) for the full statement of UH's rules.

### Students with Disabilities

Students seeking accommodation in this course should contact the instructor after obtaining the appropriate documentation through the UH Center for Students with Disabilities (713-743-5400). The University of Houston System complies with Section 504 of the Rehabilitation Act of 1973 and the Americans with Disabilities Act of 1990.

### Counseling and Psychological Services

Counseling and Psychological Services (CAPS) can help students who are having difficulties managing stress, adjusting to college, or feeling sad and hopeless. You can reach CAPS (www.uh.edu/caps) by calling 713-743-5454.

### Recording of Class

Students may not record all or part of class, livestream all or part of class, or make/distribute screen captures, without advanced written consent of the instructor.

### Syllabus Updates

This is a preliminary syllabus; adjustments will be made before and as the semester progresses.
