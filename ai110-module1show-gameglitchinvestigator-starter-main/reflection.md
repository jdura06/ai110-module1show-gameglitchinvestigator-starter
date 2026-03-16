# 💭 Reflection: Game Glitch Investigator

Answer each question in 3 to 5 sentences. Be specific and honest about what actually happened while you worked. This is about your process, not trying to sound perfect.

## 1. What was broken when you started?

- What did the game look like the first time you ran it?
- List at least two concrete bugs you noticed at the start  
  (for example: "the secret number kept changing" or "the hints were backwards").

---
What was broken at first glance was that the hint button did not display the hint after clicking it on again. It should display the hint and hide it on every click. The second bug is that the hints are backwards. When the secret guess is lower it actually says go higher, and vice versa. Another bug is that the restart button does not work. What is expected is that you can replay the game from start each time you click the button.

## 2. How did you use AI as a teammate?

- Which AI tools did you use on this project (for example: ChatGPT, Gemini, Copilot)?
- Give one example of an AI suggestion that was correct (including what the AI suggested and how you verified the result).
- Give one example of an AI suggestion that was incorrect or misleading (including what the AI suggested and how you verified the result).

---

For this project, I worked exclusively with the Copilot agent. An AI suggestion that was correct was
fixing the logic behind the hint box. It suggested that the hint only displayed after submitting a guess, so if it was turned off, it would only turn back on for the next guess. It suggested to move the hint logic outside the submission box. I manually verified the result by making a guess and clicking on the checkbox. The bug was completely fixed.

## 3. Debugging and testing your fixes

- How did you decide whether a bug was really fixed?
- Describe at least one test you ran (manual or using pytest)  
  and what it showed you about your code.
- Did AI help you design or understand any tests? How?

---

The way I decided a bug was fixed was by first identifying the bug, then deciding what the actual function should be, then testing after fix to make sure the feature did what it was supposed to do. One of the manual tests I ran was making sure the hint checkbox worked. I entered a guess and tested the fix. AI helped design a few tests for the guessing feature, to make sure the hints were as expected.

## 4. What did you learn about Streamlit and state?

- In your own words, explain why the secret number kept changing in the original app.
- How would you explain Streamlit "reruns" and session state to a friend who has never used Streamlit?
- What change did you make that finally gave the game a stable secret number?

---

The original changed because the script kept rerunning every time the user entered a guess. Reruns are the script running again after each input. Session state stores important things that need to be saved after each rerun. The secret is stored in the session state to ahve a stable secret number.

## 5. Looking ahead: your developer habits

- What is one habit or strategy from this project that you want to reuse in future labs or projects?
  - This could be a testing habit, a prompting strategy, or a way you used Git.
- What is one thing you would do differently next time you work with AI on a coding task?
- In one or two sentences, describe how this project changed the way you think about AI generated code.

---

I want to reuse the way I used git in this project. I was not strongly familiar with it, and I want to keep learning how to use it. One thing I would do differently is taking a deeper look at each action the agent makes. I now realized how powerful AI and agents are at helping with code. It can make tasks very easy and quick, but also make fatal mistakes. It needs constant monitoring, but AI is an undeniably useful tool.
