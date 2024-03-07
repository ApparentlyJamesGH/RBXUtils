# RBXScript v1
RBXScript is a versatile Lua module for Roblox, offering a range of utility functions to help do scripting tasks. From simplifying common operations to providing specialized tools for game mechanics, user interfaces, and more, it enables developers to accelerate game creation. RBXScript serves as a time-saving toolkit, allowing developers to easily use built-in functions, without needing to make custom ones that would use more time to make.

## Requiring the module
Before you start, you need to require the module as any other. To do that, simply use ```require()``` and put the path to RBXScript inside the brackets.
```lua
local RBXScript = ... -- Path to RBXScript
local RBX = require(RBXScript)
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
| .distance(position0, position1): Vector3 |

| Using.Random |
| ------------- |
| .range(min, max, (optional) seed): number |

| Using.Object |
| ------------- |
| .findAll(name, searchIn): Instance |
| .findAllFromClass(class, searchIn): Instance |
