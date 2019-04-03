# `Ecosystem/backend`

`backend` will process all the data behind the scenes. Adjustments will be made here.

## Tech Stack

* Node
* Express
* Postgres

`or`

* Firebase (undecided)

## Attributes

Properties of each element in the ecosystem. Every organism will have their own unique property.

### Map
```javascript
let root = {
  coordinates: [[]],
  timeInDays: "",
  numOfPlants: "",
  numOfEggs: "",
  numOfAnimals: "",
}
```
**coordinates**: 36x36 map.\
**timeInDays**: Days change every 5 seconds.

### Plant
Unique property: A plant will be able to reproduce on its own.
```javascript
let plant = {
  position: [],
  age: "",
  nutrients: "",
  speed: 0,
  skill: [],
}
```
**position**: Position of element in the map.\
**nutrients**: Amount of nutrients when someone consumes this element (100-10). *Unique to animals*: at hunger level of 0, their nutrients will start depleting.\
**speed**: Plant doesn't move so it's set to 0. Animals will have a faster speed when evolving but will start to decrease as they age.\
**skill**: Random skill when spawns. Might not have a skill.

### Egg
Unique property: Eggs are hard to find.
```javascript
let egg = {
  position: [],
  type: "",
  age: "",
  nutrients: "",
  speed: 0,
  skill: [],
}
```
**type**: Carnivore, Herbivore or Omnivore.

### Animal
Unique property: Animals can increase their speed when they evolve at a certain age. But the speed will start to decrease if they are hungry or if they are aging on final evolution.
```javascript
let herbivore = {
  position: [],
  type: "",
  age: "",
  gender: "",
  nutrients: "",
  metabolism: "",
  hunger: "",
  direction: "",
  speed: "",
  skill: [],
}
```
**metabolism**: Rate of change of animal's hunger.\
**hunger**: Hunger level (100-0).\
**direction**: Direction in which the element is facing.
