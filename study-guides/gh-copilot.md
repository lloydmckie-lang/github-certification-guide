![GitHub CoPilot Study Guide](../images/gh-copilot.png)

# GitHub CoPilot

Get exam-ready for your GitHub CoPilot Certification with our
comprehensive study guide. We’ve curated the essential
resources and learning activities to better prepare you for the
GitHub Actions exam and boost your chances of success.

## Objective Domains

An objective domain for a certification exam, often referred to as a “domain” or “exam domain,” is a structured outline or framework that defines the specific knowledge, skills, and topics that the certification exam will cover. It provides a clear roadmap for what candidates should expect to encounter on the exam and what they need to study and prepare for.

The domains provided in this study guide are intended to provide insight into the topic categories covered in the GitHub Actions exam, along with the learning objective within each domain.

Domain Breakdown
```
Domain 1: Responsible AI
Domain 2: GitHub Copilot plans and features 
Domain 3: How GitHub Copilot works and handles data
Domain 4: Prompt Crafting and Prompt Engineering
Domain 5: Developer use cases for AI
Domain 6: Testing with GitHub Copilot
Domain 7: Privacy fundamentals and context exclusions 
```

## Domain 1: Responsible AI
1. Risks and Limitations
Generative AI is a prediction engine, not a logic engine. You must understand these three pillars:

* Data Bias: Copilot is trained on public GitHub repositories. If the source data contains biased patterns (e.g., gendered language in comments or non-inclusive variable names), the AI may replicate them.

* Knowledge Cutoff: The model's "depth" is limited by when it was last trained. It may suggest deprecated APIs or libraries that have since been patched for security vulnerabilities.

* Hallucination: The AI can confidently suggest a library, function, or parameter that does not exist.

2. Identifying Potential Harms
The exam categorizes "harm" into specific buckets:

* Security: Suggesting code with known vulnerabilities (e.g., SQL injection or hardcoded credentials).

* Privacy: Accidentally leaking patterns that look like PII (Personally Identifiable Information).

* IP/Copyright: The risk of suggesting code that too closely matches a specific licensed public repository (mitigated by the Duplication Filter).

## Operating & Mitigating Risks
To "operate a responsible AI" in a professional workflow, GitHub emphasizes a Human-in-the-loop (HITL) approach.

Key Mitigation Strategies:
* Validation is Mandatory: You must treat Copilot as a "Pair Programmer," not an "Author." The human is always the final reviewer.

* Security Scanning: Using tools like GitHub Advanced Security (GHAS) or CodeQL alongside Copilot to catch insecure suggestions before they reach production.

* Duplication Detection: Enabling the filter that blocks suggestions matching public code (found in Settings -> Copilot).

* Prompt Engineering: Providing clear, high-quality context to reduce the chance of the model "guessing" and making mistakes.

## Domain 2: GitHub Copilot plans and features (TODO) 
## Domain 3: How GitHub Copilot works and handles data (TODO)
## Domain 4: Prompt Crafting and Prompt Engineering (TODO)
## Domain 5: Developer use cases for AI (TODO)
## Domain 6: Testing with GitHub Copilot (TODO)

## Domain 5: Measuring Impact & Productivity
The exam focuses heavily on how to prove Copilot is working. If you are on an Individual plan, you have zero access to these metrics, but for the exam, you must know how they work for Business/Enterprise.

The "Productivity API" (Copilot Metrics API)
Availability: Only for Copilot Business and Copilot Enterprise.

Data Retention: The API and Dashboard typically show the last 28 days of data.

### What it tracks:

* Acceptance Rate: (Total Acceptances / Total Suggestions).

* Lines of Code (LoC): Total lines suggested vs. total lines accepted.

* Active Users: Daily Active Users (DAU) to track adoption.

* Chat Metrics: Number of "turns" (back-and-forth) and how many chat suggestions were inserted into the editor.

* What it does NOT track: Individual developer names (data is aggregated to protect privacy).

### Qualitative vs. Quantitative Metrics
If a question asks how to measure impact without the API, look for these answers:

* SPACE Framework: A GitHub-recommended framework (Satisfaction, Performance, Activity, Communication, Efficiency).

* DORA Metrics: Focus on Lead Time for Changes and Deployment Frequency.

* Developer Surveys: Asking developers about "Flow State" and "Perceived Toil."
