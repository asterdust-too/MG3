# MG3
## Devlog
### Prompt Answers
-What are the default values for floats, ints, bools, and strings? To find out, try adding one variable of each type as a member variable to the Timer class, and     see what default value for each variable shows up in the Inspector.
-How does the Update method get called- is your code supposed to call it in this assignment, or does it get called some other way?
-Explain how either the KickWeapon or TimerText class use the timer. Mention the Update() method.

1. The default values for floats and integers are similar, only floats can use decimals. The default for both is 0, since they use numbers. For booleans, it is a false checkbox that must be checked in order to make it true. For strings, it is an empty text box. This is because there was no information given regarding what the string should say, so it allows for anything. This is useful if you need to edit text within the Unity editor and not having to go to the code every time to change it.
2. The Update method is called by Unity itself, and runs every frame. Since its return type is void, it doesn't return anything, but can be hooked into other code to check any new states. My analogy for it would be a pulse repeater powering an Observer every tick in Minecraft.
3. TimerText uses the timer but checking every frame for when it goes past 0. The code is set for the timer to start at 30, and every frame it goes down. After 30 seconds, the timer will hit 0 and start going into negatives. At this point, the GameOver method will activate and freeze the player control. The _gameTimer will run until it finished using the timer's maxTime to start, and Update() checks when it finishes, and the _gameTimer will then call GameOver.

## Open-Source assets
- [Cat fighter spritesheet](https://opengameart.org/content/cat-fighter-sprite-sheet)
- [Food sprites](https://rcpstd.itch.io/pixel-food-pack)
