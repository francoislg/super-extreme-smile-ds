/* Diary 
		June 28th 2010 : Yeah. Starting a new project to enter the Neo Compo contest again.
				2 days ago I started thinking about doing another game, a full one this time.
				Yesterday I read lot and lot of things about Libnds. I'll use this instead of Palib.
				I got an idea today and thought it would be cool. Here it is :
					You would have a static ball in the middle. Camera follows it. You have to get to the end of the level.
					(it's a platformer). To move you have to flip the background using your stylus. You could get "Powerups" such as
					stylus sliding Kirby Canvas Curse Style. There would be user-created content with an in-game tiles editor.
				My friend found a name : Super Extreme Smile. I found it cool, so I'll do a smile that rolls over as your character.
				Guess it's the name now ^^. I'm currently showing the ball, and it rotates pretty well thanks to DS functionnalities.
				I will try to do kind of collisions now with a sample background.
		July 4th 2010 : Been discussing with Zeromus on libnds forums. I wanted to have per-color collision. After a few days, he managed
					to explain me that color is not the way to do, that I should stick with tiles. 
				My idea was to have real-time rotation, but I decided to screw this. So I did it today.
				I currently have a background, 64x64 tiled maped, with some tiles. I have 4 ways. 0,90,180,270 degrees to rotate.
				It's pretty nice, time freezes when you pressed on the screen and rotating is pretty smooth.
				I've done 4 kinds of tiles. 0- Invisible (black). 1- Normal. 2- Triangle like this /|. 3- Triangle like this |\.
				Working very good, even with rotation. Trying to write a program in C# to create maps easily, but failed, I'll stick with the in-game editor...
				I'll do some tests concerning loading and unloading stuff to DMA. Then I'll go to bed, continuing tomorrow.
		July 5th 2010 : It WORKS ! Finally managed to get map loading from file working. 
				Now I'll work on an editor so I can start right now saving maps, and stuff ^^
				Saving works, loading too. I've done a simple saving system with numbers so I can have multiple saves.
				Did new tiles. One-Direction-Pass-through for all 4 directions. Pink tile which rebound. Boosters for each direction. Total : +10.
		July 13th 2010 : Back from a trip ! Pretty cool. Thought of a lot of new ideas. Will try to do some kind of gui for map editor on top screen...
				Did some changes I thought of, but second screen isn't working =/
				Managed to get a sprite show to sub screen. Managed to get the console at the same time ( USEFUL !!!! :D ) Now trying to change the sprite, :(
				Yeah, it works now. I really don't know if I'm doing it the good way... but hey, it works.
		July 14th 2010 : Tried something better. Hope it works :) I implemented a background already so it will be easier later. And I can see black on it.
				IT WORKS ! Yeah, now I feel it's the good way. I've picked Tiles DIRECTLY, no need for sprite. This is awesome.
				I've added function for screen swapping so it's easier to control while creating a map. It's wonderful ^^
				Added a zoom function in the editor to make it easier to create maps.
				Tried a lot of thing concerning the mini-map on top screen.. Problems with palette and stuff...
				Still a lot of problems... didn't know it was that hard =/ Can't manage to get the minimap properly.
		July 15th 2010 : FINALLY !!!!! WOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOO !
				I had an idea for palette thing, and it worked. So now there is a mini-map. Scrolling :P
				Added a lot of tiles. Teleporter entrances and Exit, switch, 2 walls (on/off) for the switch, a mine that kills you, and will now do other corners.
				Corners done. I did a checkpoint flag and brown tile, which slows you when on it. I've done enough for today ^^.
		July 16th 2010 : I will do coins now. You can pick up coins and then unlock a tile when you have enough. More gameplay possibilities !
				You can pick up 1 coin now. There are doors for 5-10-25-50-100 coins. I will do a red coin too, which value 5.
				I did a Silver coin which gives 10 coins. And a coin eraser when you pass over it. Could be useful for some maps. Total : 35 Tiles
				I'm having problem with the palette on the sub screen. I guess I'll have to use the external palette, I just don't know how.
		July 19th 2010 : I had some pretty good ideas for the game. For now I'll try to have my sprite move a bit more.
				Decided to add an external ball which moves as your character.
				PROBLEM ! Didn't think that sprites didn't have a point which the sprite can rotate around.
		July 20th 2010 : Still working on the rotating problem. I have to rotate the external ball around a specific point. I never learned that o,O.
				Really can't managed to get it working... I think I'll just forget this idea.... Yeah.
				I'll do a second teleporter. Then STATES !
				States work. Red and Blue state help you pass through Red and Blue tiles.
		July 21th 2010 : Will start working on sound and music. I'm in the mood for it.
				I'm impressed by the power of Maxmod. Music event will probably be a really cool thing for the background.
				I did something cool with graphics. When moving the screen it does like a screenshot and everything turn black and white. Great Effect ^^.
		July 22th 2010 : Will do a new state which protects the player from mines. Will do better handling for mines too.
				And now, music events :D --- Wow. It's awesome. It works as intended. It can have 14 sprites (cause of rotsets) according to music event.
					It does a greeeeaaaaat effect. I don't need a background with this ^^
		July 25th 2010 : Did some bug fixing, and some more collisions with corners that I haven't done before.
				Did brief tile description to help map editing ^^
		July 27th 2010 : Still no Starcraft 2 retail copy, damn... I'll try to do some things with loading and saving under other names.
		July 28th 2010 : Loading with whatever filename is almost done. Had hard time with some stuff, but it's a necessesary implementation.
				I think 300 maps is ok...? :P
		July 29th 2010 : Still working on loading.... Now it works. You can load whatever name your map is in the Smile folder ^^
				Now, SAVING ! With custom names... Works. Kinda. Keyboard is just reallllly ugly. Palette problem ?
				UPGRADE, COMPLETE ! YEAH ! Saving and loading ! Woo ! I'll now do preparations for multiple languages.
		July 30th 2010 : Did some cleaning. Will add more language stuff. Then will change graphical things. Added a new State, Sticky. And it's Tile.
				Changed the music-background effect to not be randomly placed, but where the sprite is, and is moving in a random position. Even more cool.
				SO COOL ! HAHAHA ! 70 Sprites, 5 each music event. Pure Awesomeness .... Now I'll work back on collision. I'm not satisfied with the current one.
				There. Corners collision alllll right. I found a lot that I never thought of before. Corners are a pain to collision xD.
				Now... what to do...... Take a break......... I haven't took a break. I thought of fixing collision again... Reduce sprite size to 8x8 ?.... Nah.
					Maybe change every collision line with a macro so it would detect the down sprite and part of the corners... Yeah... *sigh*
				Hard work, but from now, everything is fixed :D
				What I have to do : Corner like this / and this \ with left & right collision. I won't do corners ever again. EVER !
				My friend gave me an idea for a tile : A blackhole. I'm doing it. With No-Gravity Tile. Total : 47
				It's worth mentioning that it's Midnight and I've been up since 9 o'clock this morning. I stopped 4-5 to play a game of SC original, else I programmed...
					Time to go to bed soon :P
		July 31th 2010 : Will probably release the game so people can find bugs I didn't find. And give me ideas of what could be better, and everything.
		Aug. 3th 2010 : 17 days before the contest ends. I should start making menus... I've done some tests with menu loading, seems to work.
				Kinda working, still have a lot of work to do. ...... Cool. Primary things are done. Loading stuff doesn't corrupt anything now.
				It means I can start working on the full menu. I plan on having an option menu (accessible in-game too), achievements, campaign, custom.
					Custom sub-menus would be load a map, create a map. Options would have language, things like that. Now, time to go to bed !
		Aug. 4th 2010 : Main menu now. And I will do some stages to include in, and saving functions. But first, some code cleaning, haha.
				It's done, now sub-menus. But I'll do options before. DAMN ! DIDN'T NOTICE SAVING KEYBOARD IS SCREWED UP ! FIX SOON !
				Finaly, it was pretty easy. Just changed a background number... phew... ... Can't managed to get the custom font working... sigh... Will see later.
		Aug. 5th 2010 : Doing some work on options.
		Aug. 7th 2010 : Again.
		Aug. 8th 2010 : Still... Will add 2 new tiles I thought of. Keys and doors. 1 key opens 1 door. Changed some collisions things to have better collisions sometimes.
		Aug. 9th 2010 : Will add 4 color keys, which will be optainable 1 time, and will open every door of it's color. Bug fixing after.
				Now adding more sizes when painting. Can do a square of 1x1, 3x3, 4x4, ect.
		Aug. 10th 2010 : Did a lot of bug fixing. Changed some sticky-related fixes. Will now add Neo Compo Splash Screen.
		Aug. 12th 2010 : Working on saving for options. .... I had a cool idea. Load during splash screen ! :D
				Now doing graphics for keys and coins. And then, achievements ? Well, I've done bug fixing again. And added the current time.
				Now ACHIEVEMENTS ! Finally hehe. Saving works too. I've got used to this technique :P
*/
