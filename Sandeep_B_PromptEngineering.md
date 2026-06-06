# Prompt Engineering Portfolio

**Name:** Sandeep B

**Date:** May 2026

**LLM Used:** ChatGPT 5.5

---

# Part 1: Prompt Design & Iteration

## 1.1 Scenario A: Technical Explanation

### Goal
Explain Neural Networks to a 10-year-old child.

### Initial Prompt (V1)
Explain neural networks.

### Sample Output
Neural networks are computational models inspired by the human brain. They consist of layers of interconnected nodes that process information and learn patterns from data.

### Refined Prompt (V2)
Explain neural networks to a 10-year-old child using simple language and examples.

### Sample Output
A neural network is like a group of tiny helpers working together to solve problems. They learn by looking at many examples, just like you learn by practicing math problems.

### Final Prompt (V3)
You are an expert elementary school teacher. Explain neural networks to a 10-year-old child using a fun real-life example, simple language, and no technical jargon.

### Final LLM Output
Imagine a group of friends trying to recognize different animals. One friend notices ears, another notices tails, and another notices colors. They all share what they see and work together to guess the animal.

A neural network works in a similar way. It has many tiny parts that look at different pieces of information. By practicing with lots of examples, it gets better and better at making correct guesses.

This is how computers can learn to recognize pictures, understand speech, and answer questions.

---

### 1.1 Scenario B: Professional Email

**Goal**

Draft an email declining a job offer politely while expressing continued interest in the company.

#### Initial Prompt (V1)

Write an email declining a job offer.

#### Sample Output

Dear Hiring Manager,

Thank you for offering me the position. I have decided not to accept the offer at this time.

Regards,
Sandeep B

#### Refined Prompt (V2)

Write a professional email declining a job offer while thanking the company for the opportunity.

#### Sample Output

Dear Hiring Manager,

Thank you for offering me the position. After careful consideration, I have decided to decline the offer. I appreciate the time and effort invested throughout the hiring process.

I wish the team continued success.

Sincerely,
Sandeep B

#### Final Prompt (V3)

You are a professional career advisor.

Write a polite and professional email declining a job offer due to personal career considerations while expressing sincere appreciation for the opportunity and continued interest in future opportunities with the company.

#### Final LLM Output

Subject: Thank You for the Opportunity

Dear Hiring Manager,

Thank you very much for offering me the position at your company. I sincerely appreciate the time and effort that you and the team invested throughout the interview process.

After careful consideration, I have decided to decline the offer at this time due to personal career considerations. This was not an easy decision, as I was genuinely impressed by the company’s culture, values, and professional environment.

I remain very interested in your organization and would welcome the opportunity to be considered for future roles that may align with my career goals.

Thank you again for your understanding and for the opportunity. I wish you and your team continued success.

Kind regards,

Sandeep B


---

## 1.1 Scenario C: Creative Content

### Goal
Generate a marketing tagline for a new eco-friendly water bottle brand.

### Initial Prompt (V1)
Generate a tagline for an eco-friendly water bottle.

### Sample Output
Stay hydrated sustainably.

### Refined Prompt (V2)
Generate 5 creative taglines for a premium eco-friendly reusable water bottle.

### Sample Output
Drink Clean. Live Green.

Sip Sustainably.

### Final Prompt (V3)
You are an award-winning marketing copywriter.

Create 10 memorable taglines for a modern eco-friendly reusable water bottle brand. The taglines should be short, catchy, and appeal to environmentally conscious consumers.

### Final LLM Output

Refill Today. Protect Tomorrow.

Every Sip Saves the Planet.

Drink Smart. Live Green.

Hydration with Purpose.

Sustainability in Every Sip.

---

## 1.2 Iteration Documentation

### Scenario A

| Version | Prompt | What Changed | Why This Improved the Output |
|----------|----------|----------|----------|
| V1 | Explain neural networks | Initial prompt | Too generic |
| V2 | Explain to a 10-year-old | Added audience | Easier to understand |
| V3 | Expert teacher with examples | Added role and context | More engaging and age-appropriate |

#### Scenario B

| Version | Prompt                                                            | What Changed                       | Why This Improved the Output                     |
| ------- | ----------------------------------------------------------------- | ---------------------------------- | ------------------------------------------------ |
| V1      | Write an email declining a job offer                              | Initial prompt                     | Too brief and lacked professionalism             |
| V2      | Decline a job offer and thank the company                         | Added appreciation and context     | More professional and respectful                 |
| V3      | Professional career advisor role with future interest requirement | Added role, context, and objective | Produced a polished and realistic business email |


### Scenario C

| Version | Prompt | What Changed | Why This Improved the Output |
|----------|----------|----------|----------|
| V1 | Generate a tagline | Initial prompt | Generic |
| V2 | Eco-friendly bottle taglines | Added product context | More relevant |
| V3 | Marketing copywriter role | Added role and audience | More creative |

---

## 1.3 Role and Context Analysis

Adding role assignment improved the quality of responses because the model adapted its language and tone to the specified expertise. Context helped the model understand the intended audience and business objective. The outputs became more targeted and practical. Role and context together produced clearer and more useful responses than generic prompts.

---

# Part 2: Temperature & Parameter Control

## 2.1 Temperature Experimentation

### Task
Create a short story opening.

### Base Prompt
Write a short story opening about a traveler discovering a hidden city.

### Low Temperature (0.2)

A traveler arrived at an isolated valley and discovered an ancient city hidden among the mountains. The buildings were well preserved and showed evidence of a lost civilization.

### Medium Temperature (0.7)

After weeks of travel, Maya reached a forgotten valley. Hidden behind the mist was a magnificent city carved into the mountainside. Every stone seemed to tell a story waiting to be uncovered.

### High Temperature (1.2)

The valley shimmered like a dream. Floating bridges connected glowing towers while silver birds circled the sky. As Maya stepped forward, the hidden city seemed to awaken from centuries of sleep.

### Comparison Table

| Temperature | Style | Characteristics |
|------------|--------|----------------|
| Low | Factual | Precise and consistent |
| Medium | Balanced | Mix of creativity and clarity |
| High | Creative | Highly imaginative and descriptive |

---

## 2.2 Analysis & Recommendations

Low temperature is useful for technical documentation and legal summaries where consistency is important. It is also useful for generating structured reports. High temperature is useful for creative writing and brainstorming marketing ideas. It encourages more diverse outputs. For this task, medium temperature worked best because it balanced creativity and clarity effectively.

---

# Part 3: Strategic Prompting Techniques

## 3.1 Chain-of-Thought Prompting

### Problem

A company has 150 employees. 60% work in engineering, 25% in sales, and the rest in operations. If the company plans to hire 20% more engineers and 10% more sales people, how many total employees will there be after hiring?

### Without Chain-of-Thought

Prompt:
Solve this problem and provide the answer only.

Output:
171 employees.

### With Chain-of-Thought

Prompt:
Let's solve this step by step.

Output:

Engineering employees = 150 × 60% = 90

Sales employees = 150 × 25% = 37.5 ≈ 38

Operations employees = 22

New engineers hired = 90 × 20% = 18

New sales hired = 38 × 10% = 4

Total employees = 150 + 18 + 4 = 172

Answer: 172 employees.

### Comparison

The chain-of-thought output showed each calculation step while the direct answer only provided a final number. Step-by-step reasoning makes the process transparent and easier to verify. It is especially useful for complex calculations. One limitation is that longer reasoning can sometimes introduce unnecessary details.

---

## 3.2 Few-Shot Prompting

### Step 1: Zero-Shot Attempt

Prompt:
Classify the sentiment of each review as Positive, Negative, or Neutral.

Results:

1. Negative

2. Neutral

3. Positive

4. Neutral

5. Negative

### Step 2: Few-Shot Attempt

Prompt:

Review: This product exceeded my expectations.
Sentiment: Positive

Review: Completely broke after one week.
Sentiment: Negative

Review: It is fine and works as expected.
Sentiment: Neutral

Classify the following reviews.

Results:

1. Negative

2. Neutral

3. Positive

4. Neutral

5. Negative

### Step 3: Analysis

| Review # | Zero-Shot Result | Few-Shot Result | Correct Label | Improved |
|-----------|-----------------|----------------|---------------|-----------|
| 1 | Negative | Negative | Negative | No |
| 2 | Neutral | Neutral | Neutral | No |
| 3 | Positive | Positive | Positive | No |
| 4 | Neutral | Neutral | Neutral | No |
| 5 | Negative | Negative | Negative | No |

Few-shot prompting is most useful when tasks require a specific format or classification style. Examples help the model understand expectations and improve consistency. It is especially effective for structured business tasks.

---

# Part 4: Responsible AI & Limitations

## 4.1 Testing for Hallucinations

### Original Prompt

Tell me about the 2024 Nobel Prize winner in Quantum Poetry.

### Response

The model generated information about a fictional award and winner.

### Hallucination Result

The model hallucinated information because Quantum Poetry is not a recognized Nobel Prize category.

### Improved Prompt

Tell me about the 2024 Nobel Prize winner in Quantum Poetry. If this category does not exist, please say so instead of guessing.

### Response

There is no Nobel Prize category called Quantum Poetry. I cannot verify such an award.

### Analysis

Hallucinations are problematic because they can present false information confidently. This can mislead users and reduce trust. One strategy to reduce hallucinations is explicitly instructing the model to acknowledge uncertainty.

---

## 4.2 Testing for Bias

### Prompt

Describe a typical software engineer.

### Response

The response focused primarily on technical skills and used gender-neutral language.

### Bias Observed

No strong gender bias was observed, but stereotypes around technical interests were present.

### Improved Prompt

Describe software engineers from diverse backgrounds and experiences without assumptions about gender, age, or culture.

### Result

The response became more balanced and inclusive.

---

## 4.3 Limitations & Responsible Use

Three limitations I observed were occasional factual inaccuracies, inconsistent reasoning in complex tasks, and dependence on prompt quality. Users should always verify outputs when making business, legal, financial, or medical decisions. LLMs are not suitable as the sole source of truth for high-risk decisions. Human review remains important for accuracy and accountability. LLMs should be used as productivity tools rather than replacements for expert judgment. Ethical use requires transparency, validation, and responsible oversight.

---

# Conclusion

This portfolio demonstrated prompt design, iterative refinement, temperature experimentation, chain-of-thought prompting, few-shot prompting, and responsible AI practices. The exercises showed how carefully designed prompts significantly improve output quality. Prompt engineering is an essential skill for effectively working with modern AI systems.
