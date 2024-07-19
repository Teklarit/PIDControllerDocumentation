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

!> Some features (PID variable) will be aviable in version 1.1! **WorkInProgress**
1. Create variable with the `PIDCore` type.

![](./img/PID_Variable.png ':size=50%')

2. Use functions from BlueprintLibrary:

![](./img/PID_Variable_Overview.png ':size=50%')

## Links:
### UE plugin:

- [PIDController (UE plugin) - Github](https://github.com/Teklarit/PIDController.git)
- [PIDController (UE plugin) - Marketplace](https://www.unrealengine.com/marketplace/en-US/product/pid-controller-01)

### Examples:

- Tank turret rotation with PID controller
    - [Overview - Youtube](https://youtu.be/8oIjRFTFtcQ)
    - [Example project - Github](https://github.com/Teklarit/TankTurretPIDExample.git)