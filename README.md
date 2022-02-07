# Space Bunnies

**Space Bunnies** Space Bunnies is a shoot ‘em up arcade style game that will take players on a laser blasting’ journey
through space to defeat vicious alien invaders and bring the hostage kits to safety.

Created by: **Isabel Silva**
## How to play the game: 
The player avatar will have the tasks to save all kits that the enemy hold hostage and after the kits are
either saved or die the player will need to defeat the boss. Both must be done before the timer runs out.
To save the kits the player must use their laser to shoot down the enemy holding the bunny kit. Once
the enemy holding the bunny kit dies the bunny kit falls; the player will have to catch/collide with the
bunny kit before the bunny kit falls out of display. If the player catch the bunny kit in time the player
must take it pass the shield that will pop up once the player has the kit, one the bunny is past the shield
the bunny is considered saved. If the bunny reaches the end of display before the player can catch it the
bunny is pronounced dead. The more bunnies you save the more points the player gets, the more
enemies that are killed the more points the player gets. Killing the boss before the time ends gives a
player 1000 points. The goal is to get the most points as possible and be the highest score.
## Rules

1. Player must wait five seconds for enemies to align themselves to position before the game
starts.
2. Player can pause the game anytime the game is running (except in the 5 seconds entry time at
the start).
3. Player can turn sound on and off anytime during the game or while in pause or menu screen.
4. Player must save the bunnies and beat the boss within the time allowed.
5. Player must first kill the enemy holding the bunny kit before being able to catch/collide with the
bunny.
6. Bunny must be caught by the player before the shield pops up.
7. When player avatar is holding bunny the player speed is reduced by 5.
8. Player must take the bunny caught pass the shield before bunny can be marked as saved and
gain bunny saved points.
9. Enemies can not pass shield when shield is up.
3
10. If bunny kit falls off screen before the player can capture the bunny, the bunny is considered
dead and player loses bunny death points.
11. Boss enemy only appears when there are no more bunnies to save.
12. Boss can only attack player when player is in range.
13. Player lasers must hit Boss to lower the Boss’s health.
14. Boss’s health must be zero for Boss’s to be marked as defeated.
15. If Boss or enemy collide with player, the player will lose health points.
16. Player gains 1000-win points to total score only when there are no more bunnies to save AND
boss is defeated (Boss health is zero) AND timer is greater than zero.
17. If game timer reaches zero before the bunnies are saved or Boss is defeated the game will be
considered as game over. Points acquired at the time will be the last score.
18. Player can not gain more health than the max capacity (no infinity health).

## Design
Game States
1. Menu State – player start off at this state to continue to the next state the player must click the
start button
2. Setup State – the player waits for the enemies to align themselves
3. Run Game State – the player avatar, game score, bunnies saved, game timer appear on display
and game commences this state is true only when setup state completes
4. Pause State – player can access this state while run game state is on, access to this state turns
off the previous run game state, the player can restart the game which goes to the second state
(setup state) and commences from there or resume the current game turning the run game
state back on
5. Game Over State or Game Win State-- player loses when either the timer runs out or the player
loses all health, they have access to restart back to the setup state; player wins when they
defeat the final boss before the timer runs out player then has the option to continue on to the
next level (not in this game version)
Points, Health, Game Duration System
• Enemy kill: player gains 50 points.
• Kit saved; player gains 75 points.
• Kit dies; player loses 100 points.
• Player is hit by enemy/boss player loses 1 health point.
• Boss is hit by laser boss losses 10 health points.
• Player eats carrot, player gains 10 health points, max gain is max player start health.
• Boss eats carrot, boss gains 10 health points.
• Player wins the game player gains 1000 points.
• Player loses the game, player gains/lose zero points.
• Player will have 30 seconds to complete the level in game

## Video Walkthrough

Here's a demonstration of full game:

[![Win video demo](https://github.com/isabel2296/Space-Bunnies/blob/main/assets/images/space-bunnies-main.png)](https://www.youtube.com/watch?v=H1F_hmXV3FY&feature=youtu.be)

## Notes
Time frame given for this game was three weeks and languages used are a combination of HTML, CSS,
and JavaScript with p5.js/p5.js.sound libraries. One of requirements for this game was to create a bunny
NPC of any kind. For this game, the bunny NPC will be the game objects the player must save from the
enemies. This is version three of the game, each week had its own version.

## License

    Copyright [2019] [Isabel Silva]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
