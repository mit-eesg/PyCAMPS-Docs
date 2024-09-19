Modules are the building blocks of PyCAMPS. They are used to represent different components of a power system, such as buses, lines, and generators.
Each module can be classified as a generator, load, wire, renewable, storage, or other system element.

::: pycamps.modules.Module

## Generators
::: pycamps.modules.SMOneAxis
    options:
        filters:
            - "!dynamics"
Example:
```python
    from sympy import symbols
    from pycamps.modules import SMOneAxis
    sm = SMOneAxis('G1', BaseSpeed=377)
```

::: pycamps.modules.Type4_1
    options:
        filters:
            - "!dynamics"
Example:
```python
    from sympy import symbols
    from pycamps.modules import Type4_1
    sm = Type4_1('G1', BaseSpeed=377)
```

::: pycamps.modules.Type4_1Gc
    options:
        filters:
            - "!dynamics"
Example:
```python
    from sympy import symbols
    from pycamps.modules import Type4_1Gc
    sm = Type4_1Gc('G1', BaseSpeed=377)
```

::: pycamps.modules.Type4_2
    options:
        filters:
            - "!dynamics"
Example:
```python
    from sympy import symbols
    from pycamps.modules import Type4_2
    sm = Type4_2('G1', BaseSpeed=377)
```

::: pycamps.modules.Type4_2Ec
    options:
        filters:
            - "!dynamics"
Example:
```python
    from sympy import symbols
    from pycamps.modules import Type4_2Ec
    sm = Type4_2Ec('G1', BaseSpeed=377)
```

::: pycamps.modules.SM7StateControl
    options:
        filters:
            - "!dynamics"
Example:
```python
    from sympy import symbols
    from pycamps.modules import SM7StateControl
    sm = SM7StateControl('G22', BaseSpeed=377)
```

## Loads
::: pycamps.modules.PQLoad
    options:
        filters:
            - "!dynamics"
Example:
```python
    from sympy import symbols
    from pycamps.modules import PQLoad
    load = PQLoad('L1', BaseSpeed=377)
```

::: pycamps.modules.RLLoad
    options:
        filters:
            - "!dynamics"
Example:
```python
    from sympy import symbols
    from pycamps.modules import RLLoad
    load = RLLoad('L1', BaseSpeed=377)
```

## Wires
::: pycamps.modules.LongLine
    options:
        filters:
            - "!dynamics"
Example:
```python
    from sympy import symbols
    from pycamps.modules import LongLine
    long_line = LongLine('TL_1_2', BaseSpeed=377)
```

::: pycamps.modules.ShortLine
    options:
        filters:
            - "!dynamics"
Example:
```python
    from sympy import symbols
    from pycamps.modules import ShortLine
    line = ShortLine('TL_1_2', BaseSpeed=377)
```

## Renewables

::: pycamps.modules.PVSOAControl
    options:
        filters:
            - "!dynamics"
Example:
```python
    from sympy import symbols
    from pycamps.modules import PVSOAControl
    pv = PVSOAControl('PV1', BaseSpeed=377)
```

::: pycamps.modules.PVSOAControlV2
    options:
        filters:
            - "!dynamics"
Example:
```python
    from sympy import symbols
    from pycamps.modules import PVSOAControlV2
    pv = PVSOAControlV2('PV1', BaseSpeed=377)
```

## Storage
Coming soon!

## System Elements
::: pycamps.modules.InfBus
    options:
        filters:
            - "!dynamics"
Example:
```python
    from sympy import symbols
    from pycamps.modules import InfBus
    inf_bus = InfBus('Bus1', BaseSpeed=377)
```