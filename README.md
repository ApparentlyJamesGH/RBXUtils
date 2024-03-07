# RBXScript v1
RBXScript is a versatile Lua module for Roblox, offering a range of utility functions to help do scripting tasks. From simplifying common operations to providing specialized tools for game mechanics, user interfaces, and more, it enables developers to accelerate game creation. RBXScript serves as a time-saving toolkit, allowing developers to easily use built-in functions, without needing to make custom ones that would use more time to make.

| Get the model here |
Made by [ApparentlyJames](https://apparentlyjames.carrd.co/)

## Requiring the module
Before you start, you need to require the module as any other. To do that, simply use ```require()``` and put the path to RBXScript inside the brackets.
```lua
local RBXScript = ... -- Path to RBXScript,
local RBX = require(RBXScript or 16656051786)
```

## Using categories
After requiring the module, you can use one of the function libraries built-in:

| Built-in Using Categories |
| ------------- |
| Vector |
| Random |
| UI |
| Object |
| Animator |

```lua
Vector = RBX.Using.Vector
```

## Function References

| Using.Vector |
| ------------- |
| `.distance(position0, position1)`: number |
| `.pathDistance(position0, position1, (optional) agentOptions)`: number |
| `.direction(position0, position1)`: Vector3 |
| `.limit(xPosition, minPosition, maxPosition)`: Vector3 |

| Using.Random |
| ------------- |
| `.range(min, max, (optional) seed)`: number |

| Using.Object |
| ------------- |
| `.findAll(name, searchIn)`: Instance |
| `.findAllFromClass(class, searchIn)`: Instance |
| `.findAllWithTag(tag, searchIn)`: Instance |
| `.findAllWithAttribute(attribute, searchIn, (optional) attributeValue)`: Instance |
| `.find(name, searchIn)`: Instance |
| `.findFromClass(class, searchIn)`: Instance |
| `.findWithTag(tag, searchIn)`: Instance |
| `.findWithAttribute(attribute, searchIn, (optional) attributeValue)`: Instance |
| `.destroy(object, (optional) destroyAfter)`: nil |

| Using.UI |
| ------------- |
| `.getScreenSize()`: Vector2 |
| `.offsetToScale(scale, proportions)`: Vector2 |
| `.scaleToOffset(offset, proportions)`: Vector2 |
| `.vec2UDim(vector2, inScale)`: UDim2 |

| Using.Animator |
| ------------- |
| `.getRigAnimator()`: Animator |
| `.createRigAnimator(rig)`: Animator |
| `.loadPlay(animator, animation, (optional) ...)`: Animation |
| `.load(animator, animation)`: Animation |
