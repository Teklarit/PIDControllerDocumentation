# UE плагин

!> Убедитесь, что ```PIDController``` плагин включён.

![](../img/UE_PluginCheck.png ':size=50%')

## Использование
### C++

1. Добавить "PIDController" в файл Build.cs (PublicDependencyModuleNames или PrivateDependencyModuleNames).
2. Подключить PIDCore.h:
```unrealscript
#include "PIDCore.h"
```
3. Создать и инициализировать переменную:
```unrealscript
FPIDCore PID;
PID.Init(3.0f, 1.0f, 2.5f);
// или
FPIDCore PID(3.0f, 1.0f, 2.5f);
```
4. Функции и составляющие:
```unrealscript
PID.Tick(Difference, Dt);
PID.GetSignalValue();
PID.Reset();
PID.Kp;
PID.Ki;
PID.Kd;
```
### Блупринты
#### PID компонента и PID обьект
Функции и интерфейс для PID компоненты и PID обьекта:

![](../img/UE_PID_BP_Overview.png ':size=50%')

#### PID переменная

1. Создать переменную с типом `PIDCore`.

![](../img/PID_Variable.png ':size=50%')

2. Использвать функции с блупринт библиотеки:

![](../img/PID_Variable_Overview.png ':size=50%')

[filename](./Links.md ':include')
