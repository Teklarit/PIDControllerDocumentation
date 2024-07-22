# UE plugin

!> Make sure the  ```PIDController``` plugin is enabled.

![](./img/UE_PluginCheck.png ':size=50%')

## Usage
### C++

1. Add "PIDController" to Build.cs file (PublicDependencyModuleNames or PrivateDependencyModuleNames).
2. Include PIDCore.h:
```unrealscript
#include "PIDCore.h"
```
3. Construction:
```unrealscript
FPIDCore PID;
PID.Init(3.0f, 1.0f, 2.5f);
// or
FPIDCore PID(3.0f, 1.0f, 2.5f);
```
4. Functions and variables:
```unrealscript
PID.Tick(Difference, Dt);
PID.GetSignalValue();
PID.Reset();
PID.Kp;
PID.Ki;
PID.Kd;
```

### Blueprints
#### PID Component & PID Object
PID Component and PID Object use functions from interface:

![](./img/UE_PID_BP_Overview.png ':size=50%')

#### PID Variable

1. Create variable with the `PIDCore` type.

![](./img/PID_Variable.png ':size=50%')

2. Use functions from BlueprintLibrary:

![](./img/PID_Variable_Overview.png ':size=50%')

[filename](./Links.md ':include')
