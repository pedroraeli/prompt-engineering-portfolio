# Prompt Engineering Quick Reference

## The 5 Essential Elements

Every good prompt should have:

1. **Role/Context:** Who is the AI? What's the situation?
2. **Task:** What exactly needs to be done?
3. **Constraints:** Length, format, tone requirements
4. **Examples:** Show, don't just tell (when helpful)
5. **Output Format:** How should the response be structured?

## Common Patterns

### Chain-of-Thought
"Solve this step-by-step: [problem]"

### Few-Shot Learning
"Example 1: [input] → [output]
Example 2: [input] → [output]
Now do: [new input]"

### Structured Output
"Respond in JSON format:
{
  \"field1\": \"value\",
  \"field2\": \"value\"
}"

## Troubleshooting

| Problem | Solution |
|---------|----------|
| Inconsistent outputs | Add more constraints and examples |
| Too generic | Specify role, audience, tone |
| Wrong format | Use explicit format specification |
| Misses key info | List required elements explicitly |
| Too long/short | Set word/character limits |