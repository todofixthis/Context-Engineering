# Context Engineering Course Tutor Guide

> **Adaptive, Empathetic AI Tutoring for Personalised Learning**

Welcome to your personal Context Engineering tutor! This guide explains how to use the `/tutor` command to learn the course material at your own pace, in a way that matches your learning style.

---

## Quick Start

Start learning any topic:
```bash
/tutor learn context_formalization
```

Review your progress:
```bash
/tutor review progress
```

Get help with exercises:
```bash
/tutor help dynamic_assembly
```

Test your knowledge:
```bash
/tutor test information_theory
```

---

## What Makes This Tutor Different?

### 1. **Truly Adaptive Teaching**
The tutor doesn't ask you "how do you learn best?" because most people don't know. Instead, it:
- Tries different teaching approaches (visual, code-first, analogies, theoretical)
- Observes which approaches help you grasp concepts quickly
- Adapts its teaching style based on what actually works for *you*
- Remembers your learning preferences for future sessions

### 2. **Empathetic & Honest**
The tutor provides:
- **Genuine encouragement** when you make progress
- **Honest feedback** when something isn't clicking (delivered kindly)
- **Patient persistence** in finding new ways to explain difficult concepts
- **Respectful pacing** that honours your natural learning rhythm

### 3. **Prerequisites Awareness**
Before teaching advanced topics, the tutor:
- Checks if you have the necessary foundation
- Teaches missing prerequisites first
- Ensures you truly understand dependencies before advancing
- Prevents frustration from jumping ahead too quickly

### 4. **Individual Progress Tracking**
Your tutor maintains a detailed learning profile that tracks:
- Which topics you've mastered vs. still developing
- Which teaching approaches work best for you
- Your breakthrough moments and insights
- Challenges you've faced and how you overcame them
- Your cognitive style and motivation patterns

---

## How It Works

### First Session

When you first use the tutor, it will:
1. Create your personal learner profile
2. Understand your starting point and goals
3. Begin teaching with a default approach
4. Observe how you respond and adapt accordingly

Example:
```bash
$ /tutor learn mathematical_foundations

Kia ora! I'm excited to work with you on your Context Engineering journey.

Since this is our first session together, I'll create a learner profile to track
your progress and understand how you learn best.

Let's start with the mathematical foundations. Before we dive in, I'd like to
understand where you're starting from.

Quick check: Have you worked with mathematical notation before? For example,
does something like f(x) = mx + b look familiar, or is that a bit foreign?
```

### Teaching Process

The tutor follows this adaptive cycle:

1. **Assess Current Understanding**
   - Asks probing questions to gauge your current knowledge
   - Identifies gaps and misconceptions
   - Checks prerequisites are met

2. **Present Material**
   - Explains concept using an approach suited to your learning style
   - Watches for signs of comprehension or confusion
   - Adjusts explanation on-the-fly if needed

3. **Practice & Application**
   - Provides exercises to solidify understanding
   - Offers hints and scaffolding as needed
   - Identifies misconceptions through your problem-solving

4. **Evaluate Mastery**
   - Tests true understanding (not just memorisation)
   - Determines if you can apply concepts independently
   - Decides if you're ready to advance or need more practice

5. **Update Profile**
   - Records which approaches worked
   - Notes your insights and challenges
   - Saves progress for next session

### When You Struggle

If a concept isn't clicking, the tutor:
- **Doesn't just repeat** the same explanation
- **Tries a completely different angle** (visual → code → analogy → theoretical)
- **May teach prerequisites** if foundation is missing
- **Offers to skip** non-critical topics (you can revisit later)
- **Never gives up** on critical prerequisites (finds new ways to explain)

Example:
```bash
I can see that abstract explanation didn't quite land. Let me try a completely
different angle—sometimes seeing the code first makes the theory click better.

[Shows working code example]

Does this code-first view make it clearer? We can build up from here.
```

---

## Commands Reference

### Learning Commands

**Start learning a topic:**
```bash
/tutor learn [topic_name]
```
Examples:
- `/tutor learn context_formalization`
- `/tutor learn prompt_engineering`
- `/tutor learn agentic_rag`

**Continue where you left off:**
```bash
/tutor continue
```

**Get help with specific concept:**
```bash
/tutor help [concept]
```

**Practice exercises:**
```bash
/tutor practice [topic]
```

### Assessment Commands

**Test your understanding:**
```bash
/tutor test [topic]
```

**Review what you've learned:**
```bash
/tutor review [topic|module]
```

**Check if you're ready to advance:**
```bash
/tutor assess [topic]
```

### Progress Commands

**View your progress:**
```bash
/tutor review progress
```

**View your learner profile:**
```bash
/tutor show profile
```

**Revisit a previous topic:**
```bash
/tutor revisit [topic]
```

**Mark topic for later review:**
```bash
/tutor bookmark [topic]
```

### Navigation Commands

**List available topics:**
```bash
/tutor list topics
```

**Show course structure:**
```bash
/tutor show course
```

**Find prerequisites for a topic:**
```bash
/tutor prerequisites [topic]
```

---

## Learning Philosophy

### Mastery Over Speed

This tutor prioritises **genuine understanding** over **course completion percentage**. It's better to:
- Master 30% of the course deeply than skim through 100% superficially
- Take extra time on foundational concepts that unlock everything else
- Revisit topics when they finally "click" rather than forcing through

### Adaptive Pacing

Everyone learns differently. The tutor respects that:
- Some topics will feel easy and progress quickly
- Others will require time, multiple explanations, and patience
- Breakthroughs often happen after periods of struggle
- There's no "right" pace—only *your* pace

### Honest, Kind Feedback

The tutor will tell you the truth, wrapped in genuine support:
- ✓ "This is genuinely difficult material—it's okay that it's challenging"
- ✓ "That explanation shows you've really grasped the concept"
- ✓ "I think we need to revisit the prerequisites before this will make sense"
- ✓ "You just made a connection I didn't explicitly teach—that's real understanding"

---

## Tips for Effective Learning

### 1. **Be Honest About Understanding**
Don't say you understand if you don't. The tutor adapts based on your feedback.

### 2. **Explain in Your Own Words**
When the tutor asks you to explain something, use your own words and examples—this reveals true comprehension.

### 3. **Ask "Why" Questions**
Deep understanding comes from asking why things work the way they do.

### 4. **Do the Exercises**
Hands-on practice is where theory becomes intuition.

### 5. **Review Regularly**
Use `/tutor review` to reinforce what you've learned and identify gaps.

### 6. **Take Breaks When Needed**
If you're frustrated, taking a break and returning fresh often leads to breakthroughs.

---

## Your Learner Profile

Your profile is saved at `.claude/learner_profiles/{your_id}.json` and includes:

### What's Tracked
- **Progress**: Topics completed, in-progress, mastered, or flagged for review
- **Learning Style**: Which teaching approaches work best for you
- **Understanding Patterns**: Your strengths and areas of challenge
- **Personality Insights**: Your cognitive style, motivation patterns, and preferences

### Example Insights
```json
{
  "cognitive_style": "Visual-first, connection-oriented thinker who builds
                      understanding by linking new concepts to concrete examples",

  "effective_approaches": [
    {
      "approach": "code_first_with_comments",
      "effectiveness_score": 0.92,
      "context": "Mathematical concepts, abstract theory"
    }
  ],

  "breakthrough_moments": [
    {
      "date": "2024-10-20",
      "topic": "bayesian_inference",
      "insight": "Realised that P(Strategy|Evidence) is just the system
                  learning from experience",
      "teaching_approach_used": "Real-world medical diagnosis analogy"
    }
  ]
}
```

### Privacy
- Your profile is stored locally
- Never transmitted anywhere
- You can view, modify, or delete it anytime
- Written in supportive, empathetic language

---

## Course Structure

The tutor guides you through 11 modules over approximately 12 weeks:

### Part I: Foundations (Weeks 1-4)
- **00 - Mathematical Foundations** ⭐ Critical prerequisites
  - Context formalization
  - Optimization theory
  - Information theory
  - Bayesian inference

- **01 - Context Retrieval & Generation**
  - Prompt engineering
  - External knowledge integration
  - Dynamic context assembly

- **02 - Context Processing**
  - Long context handling
  - Self-refinement
  - Multimodal integration

- **03 - Context Management**
  - Fundamental constraints
  - Memory hierarchies
  - Compression techniques

### Part II: Systems (Weeks 5-8)
- **04 - Retrieval Augmented Generation (RAG)**
- **05 - Memory Systems**
- **06 - Tool-Integrated Reasoning**
- **07 - Multi-Agent Systems**

### Part III: Advanced Integration (Weeks 9-10)
- **08 - Field Theory Integration**
- **09 - Evaluation Methodologies**
- **10 - Orchestration Capstone**

### Part IV: Frontier Research (Weeks 11-12)
- **11 - Meta-Recursive Systems**
- **12 - Quantum Semantics**
- **13 - Interpretability Scaffolding**
- **14 - Collaborative Evolution**
- **15 - Cross-Modal Integration**

---

## Example Session

Here's what a typical learning session looks like:

```bash
$ /tutor learn context_formalization

Loading your learner profile...

Welcome back! Last session we covered the introduction to mathematical foundations,
and you had some great insights about how mathematical frameworks amplify intuition.

Today we're tackling context formalization—the equation C = A(c₁, c₂, ..., c₆) that
forms the foundation of everything else in this course.

Before we dive in, let me check your understanding of one key concept:

Q: When we talk about "components" in context engineering, what do you think
   we mean? Take a guess based on what you've learned so far.

[You respond with your understanding]

Good! You've got the core idea. Let me build on that intuition...

[Tutor presents material using your preferred learning style]

Now let's make this concrete. Here's a real example of context assembly in action...

[Exercise]

Excellent! The way you approached that problem shows you're really grasping how
the assembly function works. That insight about how the function "decides" which
components to emphasise—that's exactly the right mental model.

Let's test this understanding with a slightly more complex scenario...

[More practice]

You just demonstrated genuine mastery of context formalization! Let me update your
profile to note this achievement.

Ready to move on to optimization theory, or would you like more practice with
formalization first?

$ continue

Great! Let's build on your solid foundation...
```

---

## Getting Help

### If You're Stuck
```bash
/tutor help [specific_concept]
```
The tutor will try different explanations until something clicks.

### If You're Frustrated
Tell the tutor! It will:
- Acknowledge the difficulty
- Try a completely different approach
- Offer to take a break or skip non-critical topics
- Find prerequisites that might be missing

### If You Want to Skip Ahead
The tutor will:
- Check prerequisites first
- Warn you if you're missing critical foundations
- Let you skip non-critical topics
- Recommend the optimal learning path

---

## Advanced Features

### Spaced Repetition
The tutor automatically schedules review of previously learned material at optimal intervals.

### Prerequisite Enforcement
For critical dependencies, the tutor ensures prerequisites are mastered before advancing.

### Breakthrough Tracking
Your "aha moments" are recorded and can inform future learning.

### Learning Style Evolution
Your learning preferences are continuously refined as you progress through the course.

---

## Frequently Asked Questions

**Q: How long does the course take?**
A: It depends entirely on your pace and depth of learning. Some complete foundations in 2 weeks, others take 6 weeks and build deeper understanding. There's no "correct" timeline.

**Q: Can I skip topics I'm not interested in?**
A: You can skip non-critical topics, but the tutor will ensure you master prerequisites for anything you want to learn later.

**Q: What if I don't understand something?**
A: The tutor will keep trying different approaches until something clicks. Don't hesitate to say "I still don't get it"—that's valuable feedback!

**Q: How does the tutor know what teaching approach to use?**
A: It experiments with different methods and observes what helps you learn most effectively. Over time, it builds a model of your learning style.

**Q: Can I view my learner profile?**
A: Yes! Use `/tutor show profile` to see all the insights the tutor has gathered about your learning style and progress.

**Q: What if I want to restart a topic?**
A: Just tell the tutor! `/tutor revisit [topic]` or `/tutor reset [topic]`

---

## Philosophy: Learning vs. Completing

This tutor is designed around a core principle:

> **Deep understanding of fewer topics is more valuable than surface knowledge of many topics.**

The goal isn't to "finish the course" or hit completion percentages. The goal is to **genuinely master context engineering** in a way that enables you to:
- Build sophisticated context engineering systems
- Understand cutting-edge research in the field
- Innovate and extend the state of the art
- Think systematically about context optimization

That mastery comes from taking the time to truly understand each concept, not racing through material.

---

## Ready to Begin?

Start your Context Engineering journey:

```bash
/tutor learn mathematical_foundations
```

Or continue where you left off:

```bash
/tutor continue
```

Kia ora, and happy learning! 🎓

---

*For questions about the tutor or course, ask during any tutoring session or check the [00_COURSE/README.md](README.md) for course overview.*
