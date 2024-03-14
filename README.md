# RBXUtils v1.1
RBXUtils is a versatile Lua module for Roblox, offering a range of utility functions to help do scripting tasks. From simplifying common operations to providing specialized tools for game mechanics, user interfaces, and more, it enables developers to accelerate game creation. RBXUtils serves as a time-saving toolkit, allowing developers to easily use built-in functions, without needing to make custom ones that would use more time to make.

| [Get Model on Roblox](https://create.roblox.com/store/asset/16656051786) | [Get Model on Github](https://github.com/ApparentlyJamesGH/RBXScript/releases/latest) |
| ------------- | ------------- |

Made by [ApparentlyJames](https://apparentlyjames.carrd.co/)

## Requiring the module
Before you start, you need to require the module as any other. To do that, simply use ```require()``` and put the path to RBXScript inside the brackets.
```lua
local RBXUtils = ... -- Path to RBXUtils
local RBX = require(RBXUtils)
```

> [!NOTE]
> Importing the RBXUtils module manually is not mandatory, if you wish, you can just replace the `require()` function argument like this: `require(16656051786)`. (Using the ID instead of the ModuleScript keeps it always up-to-date)

## Using categories
After requiring the module, you can use one of the function libraries built-in:

| Built-in Using Categories |
| ------------- |
| Vector |
| Random |
| UI |
| Object |
| Animator |
| World |
| Math |

```lua
Vector = RBX.Using.Vector
```

> [!IMPORTANT]
> Make sure to include this `Using` part, otherwise Roblox will throw an error

> [!TIP]
> Below is a full list of functions and their descriptions.

## Function References

### Using.Vector
| Function | Description |
| ------------- | ------------- |
| `.distance(position0, position1)`: number | *Returns distance between 2 positions* |
| `.pathDistance(position0, position1, (optional) agentOptions)`: number | *Returns distance between 2 positions (using PathfindingService)* |
| `.direction(position0, position1)`: Vector3 | *Returns the direction from position0 to position1* |
| `.limit(xPosition, minPosition, maxPosition)`: Vector3 | *Limits the XYZ position values similairly to using math.clamp* |

### Using.Random
| Function | Description |
| ------------- | ------------- |
| `.range(min, max, (optional) seed)`: number | *Returns a random number between min and max* |
| `.object(objectsList, (optional) recursive)`: Instance | *Returns a random object from given objectsList* |

### Using.Object
| Function | Description |
| ------------- | ------------- |
| `.findAll(name, searchIn)`: Instance | *Finds all instances with input name* |
| `.findAllFromClass(class, searchIn)`: Instance | *Finds all instances from input class* |
| `.findAllWithTag(tag, searchIn)`: Instance | *Finds all instances with input tag* |
| `.findAllWithAttribute(attribute, searchIn, (optional) attributeValue)`: Instance | *Finds all instances with input attribute (and their value optionally)* |
| `.find(name, searchIn)`: Instance | *Finds instance with input name* |
| `.findFromClass(class, searchIn)`: Instance | *Finds instance from input class* |
| `.findWithTag(tag, searchIn)`: Instance | *Finds instance with input tag* |
| `.findWithAttribute(attribute, searchIn, (optional) attributeValue)`: Instance | *Finds instance with input attribute (and their value optionally)* |
| `.destroy(object, (optional) destroyAfter)`: nil | *Destroys object (after x seconds)* |

### Using.UI
| Function | Description |
| ------------- | ------------- |
| `.getScreenSize()`: Vector2 | *Returns screen viewport size (can be used as 'proportions' argument)* |
| `.offsetToScale(offset, proportions)`: Vector2 | *Returns the UI offset as scale* |
| `.scaleToOffset(scale, proportions)`: Vector2 | *Returns the UI scale as offset* |
| `.vec2UDim(vector2, inScale)`: UDim2 | *Returns converted UDim2 from Vector2* |
| `.notify(title, text, duration, icon)`: nil | *Sends a Roblox Core notification to client* |

### Using.Animator
| Function | Description |
| ------------- | ------------- |
| `.getRigAnimator()`: Animator | *Returns animator* |
| `.createRigAnimator(rig)`: Animator | *Returns created animator* |
| `.loadPlay(animator, animation, (optional) ...)`: Animation | *Returns loaded animationTrack (also plays it)* |
| `.load(animator, animation)`: Animation | *Returns loaded animationTrack* |

### Using.World
| Function | Description |
| ------------- | ------------- |
| `.getMousePositionData()`: RaycastResult | *Returns RaycastResult of mousePosition in 3D space* |
| `.snapToRelative(modelToSnap, snapAnchor, targetPosition)`: Vector3 | *Moves model to targetPosition (relative to snapAnchor, instead of PrimaryPart)* |
| `.randomString(length, includeCapitals)`: string | *Returns a randomized string from given length* |
| `.cframeOrientation(cframe)`: Vector3 | *Returns the XYZ orienation of a CFrame value* |
| `.match(list, partial)`: array | *Returns name matches from a given list, using the partial argument* |

### Using.Math
| Function | Description |
| ------------- | ------------- |
| `.withinRange(x, min, max)`: boolean | *Returns if x is within min and max* |
| `.lerp(x0, x1, a)`: number | *Returns the lerped value of x0 to x1* |
