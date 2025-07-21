---
description: AI rules derived by SpecStory from the project AI interaction history
globs: *
---

## <headers/>

## TECH STACK

## PROJECT DOCUMENTATION & CONTEXT SYSTEM

## CODING STANDARDS

## WORKFLOW & RELEASE RULES

## DEBUGGING

When debugging dynamic loading of JSON files for quizzes:

1. Add debug prints to the `loadQuestionsFromDirectory` function to check file detection.
2. Add debugging to the file loading part to trace the loading process.
3. When debugging, check the browser's developer console (F12) for detailed logs. Look for debug messages that use emojis (🔍, 📡, ✅, ❌) to identify issues. The debug output should help determine if the directory listing is working, which files are found, and whether the JSON files have the correct format.
4. The debug output will tell you exactly:
    - Whether the directory listing is working
    - Which files are found vs. not found
    - Whether the JSON files have the correct format
    - Where in the process it's failing