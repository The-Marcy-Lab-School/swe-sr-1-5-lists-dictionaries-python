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
tick items off their own copy.

```py
STARTER_TASKS = ["read syllabus", "set up laptop"]

def new_student(name):
    tasks = STARTER_TASKS
    return {"name": name, "tasks": tasks}

ada = new_student("Ada")
zo = new_student("Zo")

ada["tasks"].append("join study group")

print(zo["tasks"])
```

A student reports that tasks they never added keep appearing on their list.
Running the program prints:

```
['read syllabus', 'set up laptop', 'join study group']
```

### Prompt 1

Explain what went wrong, and what the author believed was happening instead.

Cover all four:

- What `tasks = STARTER_TASKS` actually does, and why it is not a copy.
- Why Ada's `append` changed Zo's list, in terms of what both names point at.
- How you would fix `new_student`, and how your fix gives each student a list
  of their own.
- One situation where you would _want_ two names pointing at the same list.
  This behavior is not a flaw in Python, so say what it is for.

That last part is the one that matters. Anyone can memorize "copy your lists".
Knowing when not to is what tells you whether somebody understands references
or has just been burned once.

### Response 1

Your response here...
