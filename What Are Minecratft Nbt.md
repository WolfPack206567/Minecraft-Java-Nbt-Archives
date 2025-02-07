##################
Nbt Meaning:
#################

The Named Binary Tag (NBT) is a tree data structure used by Minecraft in many save files to store arbitrary data. The format is comprised of a handful of tags
These NBT objects are also stored into game's save files as NBT files when the game quits or automatically saves, the same ones used in game's save files

#################
Short form: 
#################

Nbt aka (Named Binary Tag) is used to save/modify data from a entity/block which was not never in the original and it stores all of that in game save files Aka (The Worlds Files)

#################
NBT object:
#################

When the game is running, entities and block entities in loading chunks are stored in the memory. They are not stored with NBT, instead, they are just programmatic objects.
When processing NBT operations, the game needs to generate programmatic NBT object from entities/block entities, parse SNBT into NBT object, modify entities/blocks based on provided NBT object, or convert NBT object into SNBT.

#################
Short form:
#################

When the game is running (Open) entities and block entities are loading into chunks that is stored in the memory, Nbt is not stored they just objects.
Just saiding the nbt operation used nbt objects from entities/block and turns them SNBT into NBT object

#################
SNBT format:
#################

SNBT, also known as a data tag, is often used in commands in Java Edition. It can be described starting with key-value pairs enclosed in curly braces. An example of SNBT is specifying complex data for entities with commands.

#################
Short Form: 
#################

Just known as a data tag used at the end of a command with curly braces, often used with commands and specifying complex data for entites with commands

#################
Data types:	     
#################

[Byte] Byte	A signed 8-bit integer, ranging from -128 to 127 
SNBT Format/option: (inclusive).	<number>b or <number>B
SNBT Example: 34B, -20b

[Boolean]	NBT has no boolean data type, but byte value 0 and 1 can be represented as true, false. When a byte field is used as a boolean value.
SNBT Format/option: true, false
SNBT Example: true

[Short]	A signed 16-bit integer, ranging from -32,768 to 32,767 (inclusive).	
SNBT Format/option: <number>s or <number>S	
SNBT Example: 31415s, -27183s

[Int]	A signed 32-bit integer, ranging from -2,147,483,648 and 2,147,483,647 (inclusive).	
SNBT Format/option: <integer_number>	
SNBT Example: 31415926


#################
JSON and NBT:
#################

JSON as a format is very different from NBT. NBT is a data structure which can be represented as a binary stream or as text, while JSON is a text-only format designed for data-interchange,
There are only six data types in JSON: JsonString, JsonNumber, JsonBoolean, JsonNull, JsonObject, and JsonArray. In NBT, there are multiple numeric types, and there are no null and boolean data types. Arrays in NBT must be homogeneous; they cannot contain elements of different types. 
However, in JSON, the elements of a JsonArray may be of any type. The keys of tags in SNBT are allowed to be unquoted, while the keys of name-value pairs in JSON must be double-quoted.
Due to the differences between the two formats, conversion from NBT to JSON may result in a loss of information and precision. However, this conversion is still used in Java Edition on occasion, currently only for the ambient particles of custom biomes and the rule processor type of processor lists.

#################
Short form:
#################

Json and nbt are diffent but can be used as the same thing


Most Information is used from minecraft.wiki if you want to learn more about nbt here the full url https://minecraft.wiki/w/NBT_format#NBT_object  
