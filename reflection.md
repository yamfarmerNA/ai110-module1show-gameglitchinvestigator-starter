# 💭 Reflection: Game Glitch Investigator

Answer each question in 3 to 5 sentences. Be specific and honest about what actually happened while you worked. This is about your process, not trying to sound perfect.

## 1. What was broken when you started?

- What did the game look like the first time you ran it? Initially, it took a long time for the input feature to load. 
- List at least two concrete bugs you noticed at the start 
  (for example: "the secret number kept changing" or "the hints were backwards").
  It kept telling me to guess higher even when i guessed 99 and it ended up being 3. 
  When I clicked new game to restart the game, the gameover box did not go away and when I submitted new guesses, the number of guesses left didn't change

---

## 2. How did you use AI as a teammate?

- Which AI tools did you use on this project (for example: ChatGPT, Gemini, Copilot)? I ended up using copilot for this project
- Give one example of an AI suggestion that was correct (including what the AI suggested and how you verified the result). Switchin g up the ranges for the difficulties
- Give one example of an AI suggestion that was incorrect or misleading (including what the AI suggested and how you verified the result).
The AI tried to change the check_guess return output , but it got the format wrong and crashed the entire program

---

## 3. Debugging and testing your fixes

- How did you decide whether a bug was really fixed?
Run the program to see if bug was rresolved
- Describe at least one test you ran (manual or using pytest)  
  and what it showed you about your code. 
  Ran test to see if changes made using live
- Did AI help you design or understand any tests? How?
Yes. The AI developed the test
---

## 4. What did you learn about Streamlit and state?

- In your own words, explain why the secret number kept changing in the original app.
Issue with state management
- How would you explain Streamlit "reruns" and session state to a friend who has never used Streamlit? 
Everytime a change is made in the code, it automatically changes in the live web app
- What change did you make that finally gave the game a stable secret number?
st.session_state.secret
---

## 5. Looking ahead: your developer habits

- What is one habit or strategy from this project that you want to reuse in future labs or projects?
  - Planning and setting fixme before anything
- What is one thing you would do differently next time you work with AI on a coding task?
Do a better job of managing the states
- In one or two sentences, describe how this project changed the way you think about AI generated code.
This projects was my introduction to using AI to debug and program, especially using github copilot. Going forward, I will be using AI more methodically. 