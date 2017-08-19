# DnD Character Sheets on Github Pages

Drop a markdown file the respective folder, either `_characters` or `_monsters`, and all the layouts will automatically be set. The home page will ever generate all the links to all of the characters and monsters you have.

## Template usage

Here is template for all the minimal required fields to properly render everything.

```
---
name: "Some awesome name"
class: monk
race: half-elf
---
```

List of all character fields

Field | Description
:--- | :---:
name | Creature's name
class | Creature's class
level | Current creatures level
hp | Creature's hit points
sex | Creature's gender
race | Creature's race. This is set to "human" if no value is provided.
alignment | Creature's alignment
ac | Armour Class
str | The Strength attribute associated with this creature. This is set to 10 if no value is provided.
dex | The Dexterity attribute associated with this creature. This is set to 10 if no value is provided.
con | The Constitution attribute associated with this creature. This is set to 10 if no value is provided.
int | The Intelligence attribute associated with this creature. This is set to 10 if no value is provided.
wis | The Wisdom attribute associated with this creature. This is set to 10 if no value is provided.
chr | The Charisma attribute associated with this creature. This is set to 10 if no value is provided.

list of all monster fields

Field | Description
:--- | :---:
name | Creature's name
class | Creature's class
level | Current creatures level
hp | Creature's hit points
sex | Creature's gender
race | Creature's race
alignment | Creature's alignment
ac | Armour Class
str | The Strength attribute associated with this creature. This is set to 8 if no value is provided.
dex | The Dexterity attribute associated with this creature. This is set to 8 if no value is provided.
con | The Constitution attribute associated with this creature. This is set to 8 if no value is provided.
int | The Intelligence attribute associated with this creature. This is set to 8 if no value is provided.
wis | The Wisdom attribute associated with this creature. This is set to 8 if no value is provided.
chr | The Charisma attribute associated with this creature. This is set to 8 if no value is provided.

## Docker Development

Included is a Docker Compose file to make setup of a development environment as easy as `docker-compose up`. The image that used is one that was built to do development on Github Pages sites easy, [jekyll-website](https://hub.docker.com/r/raveious/jekyll-website/).
