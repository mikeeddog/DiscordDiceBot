# DiscordDiceBot
Simple dice bot for discord servers. 

## Current functions:
  roll: 
        > Randomly generates dice rolls for any amount of dice with any amount of sides.
        > Input is in a #d# format and you can add or subtract a modifier by using the format #d#+# or #d#-#.
        > Entering in just (prefix)roll will roll a single d20.
        > Entering in advantage after (prefix)roll will roll two d20 and return only the highest amount.
        > Entering in disadvantage after (prefix)roll will roll two d20 and return only the lowest amount.
        > Output is in the format ">>>@sender Total: (total of rolls) Rolls: (each roll individually seperated by ,)".
        
  fate: Rolls dice using the fate dice rolling system. 
        Input is a number and you can add a modifier by adding +# or -#. 
        Output is in the format ">>>@sender Total: (total of rolls) Rolls: (each roll individually seperated by ,)".
        The total is automatically calculated in terms of +, -, or 0 and the rolls are shown as either +, -, or 0.
        
  chad: Chad dice are a joke within my dnd group. If you know WyrmWood, its based off of their run of high variance dice.
        High variance dice have the save mean roll as normal dice, the dice's values are just changed so there are less middle numbers.
        Ex. the sides on the d4 are 1, 1, 4, and 4. I won't write out all 20 sides of the d20 but it has three sides that are 1's and three sides that are 20's
        Chad dice currently only takes in inputs in the format of #d# with the option to add or subtract a modifier.
        
  help: Sends a message explaining the bot's different functions.
  
## RollerHelperVars.csv variable meanings:
  Column 1: If you wish to run this bot on your own server, this is where you will put the bot code generated by discord.
            Here is what I followed to discord bot. https://discordpy.readthedocs.io/en/stable/discord.html
            
  Column 2: This is the prefix the bot listens for. Currently it is # so if you wish to call one of the bot's functions, you do it as #roll.
  
  Column 3: This is the MAX_ROLL variable. This sets the maximum number of dice and number of sides of a dice roll. 
            It is currently set to 200 because I found if set it higher, the output message would be too long for discord to send.
            
  Column 4: This is the MAX_MOD variable. This sets the maximum size that a modifier can be.
  
## Other small features:
  Prints to console "Bot is ready" when the bot comes online.
  
  While the bot is online, it shows the bot as playing "(prefix)roll | (prefix)help".
  
