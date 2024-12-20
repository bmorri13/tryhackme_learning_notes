# Advent of Cyber 2024

## Game hacking with Frida

- Frida intercepts requests to the API and then allows ua to analyze, modify and, interact with running applications

### Room Example

- Using Frida, we were able to find the functions that he game was calling when we interacted with various charcters within the game
- We then added logging statement to get out the various items to progress and pass the stages to get out codes, change the args that are looked at for your wallet currently to but the expensitve item and then finally, we were able to update the code to pass the last biometric check to get all the necessary flags
