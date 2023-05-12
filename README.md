# Whack_A_Mole_game
Whack A Mole Game


The game is essentially the bare bones of the very famous Whack-A-Mole game. The idea of this game is to be able to Whack a Mole and make it go back into its burrows. However, whenever you whack one down another pops up. This game incorporates that idea and switches out the moles for LEDs and the hammer for push-button switches; as you press the push-button switch the corresponding LED will turn off and another one will take its place.

To start the game, the user must first flash the game to the memory of their F103RB and then press the black button to start the code. The game is coded in different stages that the user sees. Although, in the code there are multiple levels to the code, I will describe only the ones that the user is able to see. I will divide these stages up in order to make it easier to understand.

Stage 1: Waiting for user to start the game. In this stage the game flashes all the LEDs really fast, indicating to the user that it is waiting for an input from the user to start the game. To enter in an input any of the push button switches can be pressed.

Stage 2: The game begins. When the user has pressed a push button switch, all the LEDs go dark. During this time the user is allowed to ready themselves for the actual gameplay.

Stage 3: Gameplay. When the wait timer has run out the game begins. A random LED will be turned on. The user will have to press the corresponding switch to turn off the LED. When this has successfully been done the user will move onto the next level. As the user ascends levels more random LEDs will turn on and the user will have to turn them off. However, at the same time the time to react to press the button to switch off the LED is also decreased. As a result, in the later levels the user will have to act faster or they will lose the game.

Stage 4: Win. When the user successfully completes all the stages, all 4 LEDs will begin to flash slowly, indicating to the user that they have won the game. After a certain period the game will restart and go back into flashing 4 LEDs really fast.

Stage 5: Lose. If the user loses mid game, by either pressing the wrong button or pressing the button too late. åThe game will blink the users score in binary on the LEDs to let the user know that they have lost and display their score.

COMPONENTS USED
NAME	DESCRIPTION
STM32 F103-RB Microcontroller	Microcontroller programmed by ARM Assembly
SIP Resistor Network	Use for multip case scenarios
Push Button Switch	Switch with a push button mechanism
Multiple LEDs	LEDs used to visualize the game
3.3V Power Supply, Supplied by Microcontroller	Power supply to power circuit
