# **R&D Engineering Aptitude Test — Evaluation Report**

**Candidate Name:** Nandan S. B
**Application ID / Email:** —
**Date of Evaluation:** 2026-01-13

---

## **Overall Score Summary**

| Trait / Section                            | Score (1–4) |
| ------------------------------------------ | ----------- |
| 1. Systematic Thinking & Problem Breakdown | 3           |
| 2. Information Synthesis & Contradiction Resolution | 4           |
| 3. Pattern Recognition & Transfer          | 3           |
| 4. Hypothesis Formation & Testing          | 3           |
| 5. Prioritization & Trade-offs             | 4           |
| 6. Rapid Learning Ability                  | 4           |
| 7. Reflection & Self-Awareness             | 3           |
| 8. Communication Clarity (implicit)        | 4           |
| **Total Score**                            | **28/32**   |

**Final Band:**

* 28–32 → *Strong Hire*
* 22–27 → *Hire (Conditional on GD/Interview)*
* 18–21 → *Borderline / Consider*
* <18 → *Reject*

**AI-determined Band:** Strong Hire

---

## **Section-wise Evaluation Notes**

### **1. Systematic Thinking & Problem Breakdown**

**Score: 3 (Strong)**

Categories are clear and non-overlapping: Technical issues (server space, code optimization), Network issues (congestion, DDoS), Student-side (weak network, shared WiFi). Mentions specific technical concerns like "DDoS (Denial of Service) attacks which use botnets to overwhelm a network."

Diagnostic plan is logical with 4 sequential steps, though could be more granular in isolating variables. Good mention of "Create a mail addressed to all students outlining network requirements."

### **2. Information Synthesis & Contradiction Resolution**

**Score: 4 (Exceptional)**

Excellent synthesis identifying both agreements (buses late, GPS needs work) and disagreements (budget vs bus numbers, overcrowding vs 10% utilization).

Outstanding contradiction handling: "Decrease the number of buses that run in the morning... allocate the saved budget... to deploy more buses in the evening." This is budget-neutral and creative.

Solution uses all sources: GPS with route planning (mentions "Dijkstra's algorithm"), student lists for verification, destination planning.

High-value missing information requested: "Why GPS system was discontinued," "alternative modes of transport," "number of buses currently in deployment."

### **3. Pattern Recognition & Transfer**

**Score: 3 (Strong)**

Correctly identifies the pattern as "Congestion" — "When a specific period of time deals with heavy traffic, or influx due to the reasons given."

Cafeteria application is sound: "The most congested time of the day is lunch, where all employees gather." Solution of increasing seats is practical but not the most creative.

### **4. Hypothesis Formation & Testing**

**Score: 3 (Strong)**

Four clear hypotheses: "Incorrect values given to the timer," "system timer is faulty," "trigger function... triggered prematurely or delayed," "input error causing the timer to misunderstand."

Tests are reasonable: "Query testing," "Re-check date & time," "Check trigger function... cross-check using an independent timer," "different inputs to pinpoint exact error."

Root cause methodology: "Logical input querying & code-reviews. We must cross-check each output with a working timer."

### **5. Prioritization & Trade-offs**

**Score: 4 (Exceptional)**

Excellent feasibility assessment: "Answer top 50 common questions... can just be stored in a database... does not require a lot of processing power." Correctly identifies voice input as "difficult as the model must understand and translate the voice input to text, which is not easy for beginners."

Clear prioritization: database Q&A, UI, accurate input matching.

Detailed 4-week plan with specific technologies: "Week 1: Create a concise plan... SQLite or MongoDB." "Week 2: Optimize UI for mobile... Link an existing LLM model... Ollama." "Week 4: Deploy & Containerize the model using Docker. Deploy the bot using AWS EC2 (Free version)."

Strong backup: "Scale back some features such as voice-input and mobile support to deliver an efficient desktop-based chatbot."

### **6. Rapid Learning Ability**

**Score: 4 (Exceptional)**

Clear explanation: "If the filter returns with all positions as 1, the item MAY be in the set. However, if even one position is 0, the item is definitely not in the set." Accurately captures false positives vs no false negatives.

Good real-life examples: "E-commerce... check if the user-entered item exists," "Lost & found algorithm."

Thoughtful unknowns: "Why does the Bloom Filter return false-positives?" "The type of hashing (SHA-216, SHA-516 etc)," "how will input quality affect the algorithm?"

Practical experiment idea: "Analyzing how companies such as Amazon, Flipkart or E-bay implement the algorithm."

### **7. Reflection & Self-Awareness**

**Score: 3 (Strong)**

Identifies Section 3 & 5 as easiest with reasoning: "found pattern & understood it easily," "something I tried to implement previously."

Section 1 as hardest: "difficulty of choosing the most appropriate reason from the root of the problem."

Improvement plan: "Approach this paper with a more critical mindset and try to really delve; dive into the problem scenarios." Reasonable but could be more specific.

### **8. Communication Clarity (Implicit)**

**Score: 4 (Exceptional)**

Excellent structure throughout with numbered lists, clear headers, and bullet points. Writing is clear and concise with appropriate technical vocabulary. Logical flow addresses all prompt components systematically.

---

## **Strengths**

* Exceptional information synthesis with creative, budget-neutral solutions (reallocating buses between morning/evening)
* Strong technical awareness demonstrated through specific tool mentions (Docker, AWS EC2, Ollama, Dijkstra's algorithm)
* Excellent understanding of Bloom Filter with thoughtful questions about implementation details
* Clear, well-organized communication throughout the response
* Practical project planning with realistic constraints and contingencies

---

## **Concerns / Weaknesses**

* Section 1 diagnostic plan could be more granular in variable isolation
* Pattern recognition solution (add seats) is straightforward rather than creative
* Reflection section improvement plan is somewhat generic

---

## **Final Recommendation (AI Generated)**

* **Strong Hire**

Nandan demonstrates consistent high-level thinking across all dimensions. His ability to synthesize conflicting information into creative solutions (bus reallocation), combined with practical technical knowledge and excellent communication, makes him a strong candidate. He shows genuine intellectual curiosity (Bloom Filter questions) and realistic project planning skills essential for R&D work.
