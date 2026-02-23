# R&D Engineering Aptitude Test

**Duration:** 3 Hours
**No coding required.**

---

## Section 1 — Understanding How Work Happens

### Time: 35 minutes

Your neighbor runs a small catering business with three helpers. She describes how orders work:

> "Customers call me to place orders — they tell me the event date, number of guests, and what kind of food they want. I check my diary to see if we're free that day. If yes, I note down everything and give them a price estimate based on guest count and menu.
>
> My cook plans the menu details and makes a shopping list. Sometimes customers call back to change guest count or add dishes — I have to tell the cook so he can update the list. My helper does the shopping a day before.
>
> On event day, we prepare everything and my driver delivers it. Sometimes customers pay in advance, sometimes on delivery, and some regular customers pay monthly. I keep all payment notes in a separate book.
>
> Last month was a mess — a customer increased guests from 50 to 100 the day before, but I forgot to tell the cook. We didn't have enough food. Another time, my helper bought items for the wrong order because the shopping lists got mixed up."

**1.1** List all the distinct **things** (objects/items) that are mentioned or implied in this description. Think beyond what's explicitly stated.

**1.2** List all the **events** (moments when something happens or changes) in the typical order flow, from customer inquiry to final payment.

**1.3** The neighbor says: "A customer increased guests from 50 to 100, but I forgot to tell the cook."
- What **dependency** was violated here? Express it as a rule: "When X happens, Y must happen."
- What **other parts** of the system would be affected by a guest count change? List at least three downstream effects.

**1.4** The shopping lists got mixed up between orders.
- What information should each shopping list contain to prevent this confusion?
- What **link** must exist between a shopping list and its source?

---

## Section 2 — Understanding and Combining Information

### Time: 40 minutes

Your college wants to improve the bus system. You are given the following information:

### Source A — Student Survey

* 62% say buses are late
* 70% want real-time tracking
* 45% want more buses
* 30% say mornings are empty but evenings are crowded

### Source B — College Admin

* Budget cannot be increased
* Only 10% of buses run full
* GPS tracking pilot was done but discontinued
* Evening demand is 4× morning demand

### Source C — Bus Drivers

* Delays due to traffic
* Students take time because of ID scanning
* GPS devices did not work well
* Better route planning needed

**2.1** What do all three sources agree on? What do they disagree on?

**2.2** Students want more buses, but the college cannot increase the budget. Explain how you would handle this contradiction in a practical way.

**2.3** Suggest a balanced solution for improving the bus system. Use information from all three sources.

**2.4** Write three pieces of additional information that would help you make a better recommendation.

---

## Section 3 — Finding Patterns

### Time: 25 minutes

### Situation A:

College WiFi becomes slow between 2–4 PM.

### Situation B:

The gym is full between 6–8 PM but empty at most other times.

### Situation C:

The library printer queue becomes very long right before assignment deadlines.

**3.1** What is the common idea or pattern in all three situations?

**3.2** Describe this pattern in simple, general terms without mentioning WiFi, gym, or printers.

**3.3** Apply the same pattern to this situation:
"In a cafeteria with 120 seats, students sometimes cannot find seats even though the average occupancy is only 40%."
Explain why this happens and suggest one solution.

**3.4** A college fest has these roles: Sponsorship Head, Design Head, Logistics Head. The Sponsorship Head signs a new sponsor and promises them "the stall near the main entrance." But Logistics Head has already given that stall to another sponsor.
- What went wrong in terms of **information that should have flowed but didn't**?
- What is the **underlying pattern** this shares with the WiFi/gym/printer situations? (Hint: it's related but different)

---

## Section 4 — Figuring Out Why Something Is Wrong

### Time: 25 minutes

You built a simple timer app. When you set it for 10 minutes, sometimes it rings at 11 minutes, and sometimes at 9 minutes.

**4.1** Write at least four possible reasons why this might be happening.
(*Possible reason = hypothesis, your guess for why something is happening.*)

**4.2** For each reason, write a simple test to confirm it. Each test should check only one thing.

**4.3** If more than one reason seems possible, explain how you would find the actual root cause.

---

## Section 5 — Working with Limits and Choosing What Matters

### Time: 35 minutes

You and three friends want to build a simple FAQ chatbot for new students joining your college.

### Requirements

* Answer top 50 common questions
* Work on mobile
* Fast responses
* Support both text and voice input

### Your Limits

* 4 weeks
* All team members are beginners
* No paid tools
* Exams in Week 3
* Only 8–10 hours per week per person

**5.1** Which requirements are easy or realistic? Which are difficult or unrealistic? Why?

**5.2** Choose the top three features to build first and explain why these matter most.

**5.3** Create a practical 4-week work plan based on your limits.

**5.4** After two weeks, you realize you are behind schedule. What will you do now? Write a practical backup plan.

**5.5** Your chatbot sometimes gives wrong answers to students.

- **(a)** You can either: (i) Have a human review every answer before showing it, (ii) Show answers immediately but let students flag wrong ones, or (iii) Only answer questions where the system is confident, and say "I don't know" otherwise. Which approach would you choose for your first version? Why?

- **(b)** A student receives a wrong answer about hostel registration deadline and misses it. How would you **trace back** what went wrong? What information would you need to have recorded?

- **(c)** You discover the wrong answer came from an incorrect entry in your FAQ database. How would you **fix this** so that: (i) The wrong answer stops appearing immediately, (ii) Students who already received wrong answers can be identified, and (iii) You can prevent similar errors in future?

---

## Section 6 — Quick Learning Challenge

### Time: 25 minutes

Read the explanation below:

> **Event Sourcing** is a way of storing data where you don't store the current state directly. Instead, you store every change (event) that ever happened. To get the current state, you replay all events from the beginning.
>
> For example, instead of storing "Bank account balance = ₹5000", you store:
> - Account opened with ₹1000
> - Deposited ₹3000
> - Withdrew ₹500
> - Deposited ₹1500
>
> The current balance is calculated by replaying these events: 1000 + 3000 - 500 + 1500 = ₹5000.
>
> **Advantages:** You have complete history. You can answer "what was the balance on March 15?" by replaying events up to that date. You can undo mistakes by removing or correcting events. You have a full audit trail.
>
> **Disadvantages:** Calculating current state requires replaying all events (can be slow). Storage grows over time. Some queries become complex.

**6.1** Explain this idea in simple words, as if to a friend who is not from computer science. Use an everyday example different from bank accounts.

**6.2** Give two real-life situations (not banking) where storing "what happened" instead of "current state" would be useful. Explain why.

**6.3** What parts of this idea are still unclear to you? What questions would you want answered?

**6.4** The catering business from Section 1 currently stores "Customer X owes ₹5000." If they used event sourcing instead, what events would they store? How would this help with the problems described (forgotten changes, mixed-up lists)?

---

## Section 7 — Reflection

### Time: 15 minutes

**7.1** Which section felt easiest for you? Why? What about your thinking made it easier?

**7.2** Which section felt hardest? Why? What specifically did you find difficult?

**7.3** In Section 1, you had to figure out the structure of how the catering business works. Describe your thinking process — how did you decide what the "pieces" were and how they connected?

**7.4** If you had to attempt this paper again, what would you change in your approach? Be specific.

---

## End of Test

**Before submitting:** Review your answers for clarity. Can someone else understand your reasoning?
