# 📅 Weekday Interview Scheduling Framework

🔥 **High-Volume Ops Case Study** | ⚙️ **Systems-First Design** | 🎯 **SLA-Focused Execution**

A systems-driven interview scheduling framework designed to achieve **80% interview booking within 24 hours** using only **two college interns** while handling **500+ daily scheduling requests** from **100 partner companies**.

This project was created as a Product & Operations Design case study for Weekday's scheduling assignment.

## 🚩 Problem Statement

Weekday receives over 500 interview scheduling requests daily from partner companies. Companies provide a Calendly link and expect Weekday to manage scheduling end-to-end.

The challenge:

- 📩 500+ requests per day
- 👥 Only 2 scheduling interns available
- 🤷 Candidates may ignore messages, miss emails, forget to schedule, or face technical issues
- 🔀 Multiple communication channels and edge cases create operational complexity
- ⏱️ 80% of requests must be scheduled within 24 hours

The objective was to design a scheduling system that interns could follow almost blindly while consistently achieving the SLA target.

## ❓ Key Questions Explored

- 🧠 How can 2 interns realistically process 500 requests in a single day?
- 🎯 What are the highest-impact failure points in interview scheduling?
- 💬 How can communication workflows be optimized for maximum conversion?
- 🧩 How should edge cases be categorized and handled?
- 🔄 How can the system continuously improve over time?

## 🧩 Solution Overview

The final framework combines:

### 1\. 📊 Capacity Planning

A math-backed operational model validating whether two interns can realistically achieve the target SLA.

Includes:

- 🧮 Workload estimation
- 🔻 Conversion funnel modeling
- ⚡ Throughput calculations
- 🌦️ Best-case, base-case, and worst-case scenarios

### 2\. 🔒 Slot-Lock Scheduling Architecture

Instead of asking candidates to browse and choose interview slots:

- 📌 A slot is pre-assigned
- ✅ Candidate only needs to confirm or request changes
- 🧠 Reduces decision fatigue
- 🚀 Creates urgency
- 📈 Improves first-touch conversion

### 3\. 📡 Signal-Based Communication System

Moves beyond time-based follow-ups.

Examples:

- 📱 WhatsApp delivered but unread → call
- 📧 Email opened but no action → WhatsApp nudge
- 🚫 Message undelivered → alternative channel

This reduces response cycles and increases scheduling efficiency.

### 4\. 🧱 Tiered Edge-Case Framework

30+ operational edge cases were categorized into:

#### Tier 1 - ✅ Must Handle

Examples:

- 👻 No response
- 🔗 Broken Calendly link
- ♻️ Duplicate requests
- ❌ Wrong slot booked
- 📵 Communication failures

#### Tier 2 - ⚠️ Conditional Escalation

Examples:

- 🕒 Candidate unavailable
- 🔄 Intent changes
- 🪑 Limited interview slots
- 📉 Booking cancellations

#### Tier 3 - 🚨 Escalate & Move On

Examples:

- 🙅 Explicit candidate decline
- 🌍 Impossible timezone overlap
- 🛑 System outages
- 📭 Recruiter unresponsiveness

### 5\. 🌳 Decision Tree Workflow

A complete scheduling workflow mapping every possible candidate state:

📥 Request → 🧪 Validation → 📣 Outreach → 🧭 Response Handling → 📅 Booking → ✅ Confirmation → 🧾 Logging

The goal was to eliminate intern decision-making and create a repeatable process.

### 6\. 🔁 Continuous Improvement Flywheel

Every failed scheduling attempt is tagged across three dimensions:

- 👤 Who caused the failure?
- 💥 What failed?
- 🧱 At which stage?

Daily reviews identify the largest failure pattern and introduce one improvement at a time.

This converts the system from a static SOP into a self-improving operational framework.

## 📦 Deliverables

### 📘 Interview Scheduling Framework

- 🏗️ System architecture
- 📊 Capacity model
- 🧑‍🤝‍🧑 Work allocation
- 🎯 SLA calculations
- ⚙️ Optimization strategies

### 🌲 Decision Tree Workflow

- 🛣️ End-to-end scheduling process
- 🚨 Escalation paths
- 🩹 Recovery flows
- 🧭 Ownership mapping

### 🗂️ Edge Case Taxonomy

- 🧱 Tier 1, Tier 2, Tier 3 categorization
- 🛠️ Resolution protocols
- 📌 Escalation guidelines

### 📝 Problem Decomposition Document

- 🔍 Assumptions
- 📉 Capacity analysis
- 🧠 Design rationale
- 🧭 Product thinking process

## 📈 Results

### 🧮 Base Case Projection

| Metric            | Result  |
| ----------------- | ------- |
| Daily Requests    | 500     |
| Booked Interviews | 414     |
| Scheduling SLA    | 82.8%   |
| Intern Count      | 2       |
| Working Hours     | 8 Hours |

Expected operating range:

- 🟡 Base case: 83%
- 🟢 Best case: 89%
- 🔴 Worst case: 68-78%

## 💡 Product Thinking Demonstrated

This project showcases:

- 🏭 Operations Design
- 🧠 Systems Thinking
- 🔧 Workflow Optimization
- 📊 Capacity Planning
- 🤖 Process Automation Design
- 🧱 Edge Case Management
- 🌲 Decision Tree Modeling
- 🔁 Continuous Improvement Systems
- 🧭 Service Operations Strategy

## 🗃️ Repository Structure

├── README.md  
├── Interview Scheduling Framework.pdf  
├── Weekday Scheduling Workflow.pdf  
├── Tiered Edge Cases Framework.pdf  
└── Thought Process & Problem Decomposition.pdf

## 🔍 Key Insight

> ✨ **Framing shift:** from outreach volume to conversion reliability.

The core insight from this project is that the challenge was not:

"How do we contact 500 candidates?"

but rather:

"How do we create a system that reliably converts 500 scheduling requests into confirmed interview bookings?"

This shift in framing led to the design of a scalable scheduling architecture focused on conversion, operational efficiency, and continuous improvement.

