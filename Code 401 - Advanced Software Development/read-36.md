# The Advice: Communicate

The best piece of technical interview advice I have received and can impart upon you is to communicate, communicate, communicate! This may seem like an anti-climactic piece of advice, but I hope to be able to demonstrate to you that it’s actually the most important skill to prepare prior to an interview.

- Note: as I discuss examples in the rest of this article, they will have a software engineering slant as it is the most familiar domain to me. Despite that slant, you can apply these skills to any whiteboard-style interview.

## What Do You Mean Communicate?

Let’s say you are in the interview and your interviewers throw you a whiteboard question. Do you step up to the whiteboard and feverishly start solving the problem?

That tends to be everyone’s instinct, but it’s definitely not the right way to go. Even if you think you understand the problem, you should take some very important steps before moving forward.

- First, Restate the Question
- Do you understand what they’re asking you to do? Prove it. Restate the question for them and seek affirmation. You might actually be surprised to find you don’t fully understand what they’re asking for — perhaps the question is similar, but not the same, as a practice problem you have completed in the past. Using the tried-and-true fizz-buzz example, you could restate the problem as follows:

“So I’d like to restate the problem to you to make sure I understand what you’re looking for. The sole parameter for my function will be an integer. The sole output of my function will be an incrementing array, starting from the number 1 and ending at the input number.
If a number is a multiple of 3, the output will instead be `fizz`. If a number is a multiple of 5, the output will instead be `buzz`. However, if the output is a multiple of both 3 and 5, the output will instead be `fizzbuzz`. Is my understanding correct?”
The interview should give you affirmation or, perhaps, your understanding is incorrect and they will help you understand. There is no situation in which restating the problem will hurt you — it shows you can articulate a problem and gives you time to think it through a bit while you discuss. Furthermore, starting the discussion this way will help quell some nerves that might otherwise manifest while trying to solve the actual challenge.

## Ask About Edge Cases

It’s still not time to dive right into coding the solution. Think for a bit about the inputs and expected output and think about potential edge cases to the problem. Ask about them. In many cases, the interviewer hasn’t even thought about edge cases and will make something up. That’s great — it shows you’re analytical and will work hard to try to prevent bugs (which often crop up due to edge cases).

Let’s use the fizz-buzz example. After successfully restating the problem, a valid way to ask about edge cases would be as follows:

“Now that I confirmed my understanding of the problem, I’d like to ask about some potential edge cases. Is it possible that the input would be a type other than a number? If so, what should the function do? Can the input be 0 or negative? Again, if so, what should the function do?”

## Ask About Test Cases

This is free and you should take advantage of it. Simply ask if there are any test cases that the function should pass. Your interviewer might be expecting you to ask this question, so it might be necessary. But it’s also possible the interviewer was not expecting the question and will think “ah, this candidate knows about testing!”

## Write Pseudocode and Ask If It Makes Sense

(Write Pseudocode and Check Your Logic)

- Again, you don’t actually want to start writing code in an actual language. You’ll find yourself constrained by trying to remember the methods or other idiosyncrasies of the language rather than trying to come up with the correct logic. Instead, let your interviewer know you’re going to start by writing pseudocode and fill in the actual code later. (Coincidentally, this is a reasonable way to write actual code as well).
