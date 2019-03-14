# `Ecosystem/backend`

`backend` will process all the data behind the scenes. Adjustments will be made here.

## Attributes

Properties of each element in the ecosystem.

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
**coordinates**: 36x36 map
**timeInDays**: Days change every 5 seconds

### Plant
```javascript
let plant = {
  position: [],
  age: "",
  nutrients: "",
  speed: 0,
  skill: [],
}
```
**position**: Position of element in the map
**speed**: Plant doesn't move so it's set to 0
**skill**: Random skill when spawns. Might not have a skill
**nutrients**: Amount of nutrients when someone consumes this element.

### Egg
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
**type**: Carnivore, Herbivore or Omnivore

### Animal
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
**metabolism**: Rate of change of animal's hunger
**hunger**: Hunger level
**direction**: Direction in which the element is facing
