# Short Responses

For this short response assignment, aim to write a response with the following
qualities (your instructor will give you feedback on these areas):

- [ ] Addresses all parts of the prompt
- [ ] Accurately uses relevant technical terminology
- [ ] Is free of grammar and spelling mistakes (double check with Grammarly!)
- [ ] Uses markdown to enhance readability (preview in VS Code with
      Command/Control + Shift + V)
- [ ] Is easy to comprehend

Write your response in the space provided. Make sure to preview your markdown
to check how it is rendered before submitting.

## Question 1

A study app gives every new student the same starter checklist, then lets them
tick items off their own copy. It keeps a list of student records, and gives
each record the starter checklist.

```py
STARTER_TASKS = ["read syllabus", "set up laptop"]
students = [
    {"name": "Ada"},
    {"name": "Zo"},
]

# Add a "tasks" key with starter tasks to each student
for student in students:
    student["tasks"] = STARTER_TASKS

# Add a task to Ada's list
students[0]["tasks"].append("join study group")

# Print out Zo's list
print(students[1]["tasks"])
```

A student reports that tasks they never added keep appearing on their list.
Running the program prints:

```
['read syllabus', 'set up laptop', 'join study group']
```

### Prompt 1

Use these terms correctly within your response:

- **reference**
- **alias**
- **record** or **lookup table** (whichever is relevant)

Explain what went wrong, and what the author believed was happening instead.

Cover all four:

- What `student["tasks"] = STARTER_TASKS` actually does.
- Why adding a task to Ada's list changed Zo's list. Reference specific code
  that contributed to this behavior.
- How you would fix the loop, and how your fix gives each student a list of
  their own.
- One situation where you would _want_ two names pointing at the same list.
  This behavior is not a flaw in Python, so say what it is for.

That last part is the most important one. Every behavior or rule in Python has
scenarios where it is the correct choice, even if it isn't right for the current
one. Being able to discern when to use each rule is the key to mastering a
language.

### Response 1

Your response here...
