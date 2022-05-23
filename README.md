# ArmoredPatrol
An Infinite Wave-Based Incremental Top-Down Shooter

Created by Samuel Nguyen (2013)

This was made in middle school mainly to experiment with OpenGL in Java. It's surprisingly good for a middle schooler. The changelog has no dates provided, and the source code is completely gone; it was on my old laptop, which died. Only these executables were saved on my USB.

# BASICS

You have to survive wave after wave for the longest time possible.
Enemies will spawn every wave, and the amount of enemies depends on the wave.
You regain health every 5 waves.
On some waves, special bosses will spawn.
You will need to upgrade your weapon to be able to survive in the hard waves.
To upgrade your weapon, you spend cash at the store.
To get cash, you need to kill enemies.
If you die, you will have to start all over again.

# CONTROLS

Move Around | W,A,S,D
Shoot/Interact | Left Mouse Button
Open Shop | P
Exit Shop | Space Bar
Restart When Die | Space Bar
Main Menu | Esc

# ENEMY STATS

Rifleman | Damage: 5 | Speed: 2 | Health: 50 | Cash Given: 5 | Chance to Spawn: 25% |

Assassin | Damage: 10 | Speed: 5 | Health: 30 | Cash Given: 10 | Chance to Spawn: 10% |

Grenadier | Damage: 5*8 | Speed: 2 | Health: 60 | Cash Given: 20 | Chance to Spawn: 21% |

Cannoneer | Damage: 30 | Speed: 1 | Health: 130 | Cash Given: 20 | Chance to Spawn: 30% |

Light Tank | Damage: 80 | Speed: 4 | Health: 250 | Cash Given: 75 | Chance to Spawn: 3% |

Tank | Damage: 80 | Speed: 3 | Health: 500 | Cash Given: 150 | Chance to Spawn: 3% |

Heavy Tank | Damage: 80 | Speed: 2 | Health: 750 | Cash Given: 250 | Chance to Spawn: 3% |

Helicopter | Damage: 20 | Speed: 6 | Health: 600 | Cash Given: 250 | Chance to Spawn: 3% |

Lazer Gunner | Damage: 25 | Speed: 8 | Health: 1500 | Cash Given: 1000 | Chance to Spawn: 100% on wave 20 |

Grenadier Station | Damage: 5*5*8 | Speed: 0 | Health: 10000 | Cash Given: 7500 | Chance to Spawn: 100% on wave 35 |

R_A_I_N | Damage: 20 | Speed: 8 | Health: 5000 | Cash Given: 10000000 | Chance to Spawn: 100% on wave 50 |

# NOTES

This game has two versions: 64-bit and 32-bit.
If you have a 32-bit computer, you have to use the 32-bit version.
If you have a 64-bit computer, you can use either the 32-bit or 64-bit, but 64-bit is less laggier.

Only works with Java SE 1.7 and up

Windows 7 and up only

Because I can't put text in the game itself, I put text in the bar at the top.
So when you put your mouse on a button on the shop or the menu, all the info about it is at the top.

Also, I suggest putting the game in a seperate folder, as it makes the save file in the folder, not in the jar file itself.

# Changelog
/*
 * 0.0.1 Alpha
 *   Create main class
 *   Take code from my 2D game template
 *   Clean up unwanted code
 * 
 * 0.1.0 Alpha
 *   Create basic file writing and reading system
 * 
 * 0.1.1 Alpha
 *   Create Enemy class, to be extended on in later updates
 *   
 * 0.1.2 Alpha
 *   Organize Files
 *   
 * 0.2.0 Alpha
 *   Added rifleman
 *   Riflemen now have guns
 *   
 * 0.2.1 Alpha
 *   Added compatability for multiple enemies
 *   
 * 0.2.2 Alpha
 *   Added compatability for multiple ammo types
 *   
 * 0.2.3 Alpha
 *   Player now can shoot
 *   
 * 0.3.0 Alpha
 *   Added health bars
 *   
 * 0.3.5 Alpha
 *   Added waves
 *     Enemies per wave is wave * 2
 *     
 * 0.3.7 Alpha
 *   Added Cannoneer
 *   Added Cannonball
 *   Made rotating more efficient
 *   Enemies don't fire simutaneously anymore
 *  
 * 0.3.8 Alpha
 *   You regain health every 5 waves
 *   Enemies now have a spawning area of 2366x1768 pixels
 *   
 * 0.4.0 Beta
 *   Added upgrade system
 *   Added shop
 *   
 * 0.4.1 Beta
 *   Added Tank
 *     Tank has 500 health, does 80 damage, and gives you 100 cash when you kill it
 *    
 * 0.4.2 Beta
 *   Nerfed Tank
 *   Speed upgrade now affects bullet speed
 *   
 * 0.4.3 Beta
 *   Added Starburst upgrade
 *     Costs 1200 cash
 *       One time purchase
 *     Starburst bullets split into 4 regular bullets after 1.5 seconds
 *     If a starburst bullets hits an enemy before splitting, it does 4 times the damage of a regular one
 *     Speed upgrade does not affect starburst bullets
 *     Starburst bullets are blue instead of black
 *     
 * 0.4.5 Beta
 *   Tweeked Starburst upgrade
 *     Now costs 1500 cash
 *     Splits into 8 instead of 4
 *     Direction of splitting is now random
 *     Instead of doing 4 times the damage, it now does only 2
 *     Now cancels out 5 speed upgrades
 *     
 * 1.0.0
 *   Added Saving System
 *   Added Main Menu
 *   
 * 1.1.0
 *   Tweeked Starburst upgrade
 *     Now takes 1.5 seconds to split instead of 1
 *     Now only cancels out 4 speed upgrades
 *   Tweeked Starburst bullets
 *     Splitting is more efficient
 *   Added lifedrain upgrade
 *     Works with starburst
 *     Amount of life gained depends on damage upgrade
 *     Identified by the color yellow
 *     Costs 4000 cash
 *       One time purchase
 *     Starburst bullets will split into these if lifedrain is on
 *     Starburst bullets will NOT give you health if you kill an enemy before the bullet is split
 *     Cancels out 1 speed upgrade
 *   Added an easter egg that is practically impossible to see unless you have a VERY slow computer
 *     (Or if you manage to obtain the source code)
 *   Tweeked saving and loading
 *     More efficient
 *     Fixed a bug with loading starburst upgrade
 *   Tweeked shop
 *     More efficient
 *     Changed Starburst upgrade description
 *     
 * 1.1.1
 *   Fixed bug in shop where you could not see the life drain upgrade
 *   
 * 1.1.2
 *   Armored Patrol now works with all screen resolutions
 *   Fixed bug where you could not click on buttons in the shop and menu.
 *   
 * 1.1.5
 *   Added a boss that spawns at wave 20
 *     Called Lazer Gunner
 *     Drops 1000 cash when killed
 *     Has 1500 health (3 times the health of a tank)
 *     He is the size of a cannoneer
 *     He has half the range of a cannoneer
 *     He is twice as fast as you, so you will never be able to run away
 *     Shoots lasers at an insane rate (to make it look like a constant beam)
 *     Does 25 damage
 *     Beam is faster than a tank's shell
 *   Bullets now rotate depending on what direction they are going in
 *   
 * 1.2.0
 *   Enemy creation system much more efficient
 *   Removed unnecessary toCartesian function
 *   Added 5 more enemies and corresponding bullet types
 *     Heavy Tank
 *       Shoots same bullet as normal tank
 *       Shoots faster than normal tank
 *       Has 750 health
 *       Has 900 range
 *       Speed 2
 *       Bigger than normal tank
 *       Drops 250 cash
 *     Light Tank
 *       Shoots same bullet as normal tank
 *       Shoots slower than normal tank
 *       Has 250 health
 *       Has 500 range
 *       Speed 4
 *       Smaller than normal tank
 *       Drops 75 cash
 *     Helicopter
 *       Fires "Heli Bullets"
 *         As fast as a Tank Shell
 *         As small as a Rifleman's bullet
 *         Does 20 damage
 *       Shoots a little faster than a rifleman
 *       Has 600 health
 *       Has 500 range
 *       Speed 6
 *       Wide as Normal, long as Heavy Tank
 *       Drops 250 cash
 *     Grenadier
 *       Fires grenades
 *         Slower than the player
 *         Does no damage
 *         Splits into 8 "Frags" after 1 second
 *           Frags do 5 damage
 *           As fast as a cannonball
 *           As big as a Heli_Bullet
 *           Are sent flying in random directions
 *       Shoots 1 grenade a second
 *       Has 60 health
 *       Has 120 range
 *       Speed 2
 *       As big as rifleman
 *       Drops 20 cash
 *     Assassin
 *       Fires "stabs"
 *         As fast as a cannonball
 *         Does not have a size
 *         Is invisible
 *         Does 10 damage
 *       Stabs 2 times a second
 *       Has 30 health
 *       Has 10 range
 *       Speed 6
 *       As big as rifleman
 *       Drops 10 cash
 *       
 * 1.2.5
 *   Fixed bug with 2 Lazer Gunners spawning on wave 20
 *   All enemies now look better
 *   Player also looks better
 *   Fixed bug with not being able to buy an upgrade if you have the exact money as the cost
 *   Raised price of upgrades significantly
 *   
 * 1.2.7
 *   Shop now displays correct numbers
 *   Fixed bug with life leech upgrade not buying
 *   Added 2 new bosses
 *     Grenadier Station
 *       Spawns on wave 35
 *       Shoots 5 grenades in random directions every second
 *       Has 10000 health
 *       Does not move
 *       Has range of 1000
 *       Gives 7500 cash
 *     R_A_I_N (Ruthless Armored Invisible Nuisance)
 *       Spawns on wave 50
 *       Shoots S_T_O_R_M_S (Stick That Ominously Renders Maliciously Susceptible) at a fast rate
 *       Invisible
 *       Has 5000 health
 *       When you beat him, you (technically) win the game. After this, you can still go on with higher waves (Waves 50 and up)
 *       Moves as fast as a Lazer Gunner
 *       Has range of 200
 *       Gives 10000000 cash
 *       
 * 1.2.9
 *   One word: SOUNDS
 */