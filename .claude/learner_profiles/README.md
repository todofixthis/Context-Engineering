# Learner Profiles

This directory contains learner progress profiles for the Context Engineering course tutoring system.

## Overview

Each learner has a JSON profile file that tracks:
- **Progress**: Current module, completed topics, mastery levels
- **Learning Preferences**: Which teaching approaches work best
- **Understanding Patterns**: Strengths, challenges, and breakthroughs
- **Personality Insights**: Cognitive style, motivation patterns, communication preferences

## Profile Structure

Profiles are stored as `{learner_id}.json` and include:

```json
{
  "learner_id": "unique_identifier",
  "identity": {
    "name": "optional",
    "started_date": "YYYY-MM-DD",
    "last_session_date": "YYYY-MM-DD"
  },
  "progress": {
    "current_module": "module_name",
    "completed_topics": ["topic_1", "topic_2"],
    "topics_mastered": ["topic_1"],
    "topics_to_revisit": ["topic_3"]
  },
  "learning_preferences": {
    "effective_approaches": [
      {
        "approach": "visual_diagrams",
        "effectiveness_score": 0.9,
        "context": "When explaining system architecture"
      }
    ]
  },
  "personality_insights": {
    "cognitive_style": "Descriptive, supportive insights",
    "motivation_style": "Supportive observations",
    "challenge_response": "Empathetic understanding"
  }
}
```

## Privacy & Ethics

- Profiles are stored locally and never transmitted
- All insights are written in supportive, empathetic language
- Learners can view and modify their profiles at any time
- Profiles help the tutor adapt to individual learning styles

## Usage

The `/tutor` command automatically creates and updates these profiles. Learners can:

```bash
# Start tutoring (creates profile if needed)
/tutor learn topic_name

# Review progress
/tutor review progress

# View your profile
/tutor show profile

# Reset progress on a topic
/tutor reset topic_name
```

## Files

Each file represents one learner's journey through the course. The tutor uses these profiles to:
- Remember what approaches work best for each learner
- Track which topics have been mastered
- Ensure prerequisites are met before advancing
- Celebrate specific breakthroughs and insights
- Provide personalized, adaptive teaching

---

*Profiles are tools for better learning, written with care and respect for each learner's unique journey.*
