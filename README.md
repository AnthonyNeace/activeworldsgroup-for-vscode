# activeworldsgroup-for-vscode

ActiveWorlds Group for VSCode is a vscode extension that adds language support for ActiveWorlds Group (.awg) files, which are tokenized based on the Active Worlds propdump format.

![image](https://user-images.githubusercontent.com/1206482/151717260-8b993351-144e-4a82-9ee3-c38dc25d176b.png)

## Tokens

AWG/propdump tokens are delimited by spaces and defined as follows:

* 1: Active Worlds Citizen Number
* 2: Object creation timestamp
* 3: Position (X)
* 4: Position (Y)
* 5: Position (Z)
* 6: Orientation (YAW)
* 7: Orientation (TILT)
* 8: Orientation (ROLL)
* 9: Object Type (0: Object; 1: Camera; 2: Zone; 3: Particle Emitter; 4: Mover)
* 10: Length of model name string
* 11: Length of description string
* 12: Length of action string
* 13: Length of object data string
* 14: A single concatenated string of data for tokens 10-13 above

This extension attempts to tokenize model name, description, and action based on contextual word boundaries.  There is currently no support for tokenizing the 'object data' string.

## Resources

* https://marketplace.visualstudio.com/items?itemName=AnthonyNeace.awg-for-vscode - VSCode Marketplace
* http://wiki.activeworlds.com/index.php?title=AWG - ActiveWiki - AWG
* http://wiki.activeworlds.com/index.php?title=Propdump - ActiveWiki - Propdump
