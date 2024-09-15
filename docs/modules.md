# `Modules`

::: pycamps.modules.Module

::: pycamps.modules.InfBus
    options:
        filters:
            - "!dynamics"
Example:
```python
    from sympy import symbols
    from pycamps.modules import InfBus
    inf_bus = InfBus('Bus1', RefFrameAngle=symbols('phi'), RefFrameSpeed=symbols('dphidt'), BaseSpeed=377)
```

::: pycamps.modules.LongLine
    options:
        filters:
            - "!dynamics"
Example:
```python
    from sympy import symbols
    from pycamps.modules import LongLine
    long_line = LongLine('TL_1_2', RefFrameAngle=symbols('phi'), RefFrameSpeed=symbols('dphidt'), BaseSpeed=377)
```

::: pycamps.modules.PQLoad
    options:
        filters:
            - "!dynamics"
Example:
```python
    from sympy import symbols
    from pycamps.modules import PQLoad
    load = PQLoad('L1', RefFrameAngle=symbols('phi'), RefFrameSpeed=symbols('dphidt'), BaseSpeed=377)
```

::: pycamps.modules.PVSOAControl
    options:
        filters:
            - "!dynamics"
Example:
```python
    from sympy import symbols
    from pycamps.modules import PVSOAControl
    pv = PVSOAControl('PV1', RefFrameAngle=symbols('phi'), RefFrameSpeed=symbols('dphidt'), BaseSpeed=377)
```

::: pycamps.modules.SolarPV_v2_SOAControl
    options:
        filters:
            - "!dynamics"
Example:
```python
    from sympy import symbols
    from pycamps.modules import SolarPV_v2_SOAControl
    pv = SolarPV_v2_SOAControl('PV1', RefFrameAngle=symbols('phi'), RefFrameSpeed=symbols('dphidt'), BaseSpeed=377)
```

::: pycamps.modules.RLLoad
    options:
        filters:
            - "!dynamics"
Example:
```python
    from sympy import symbols
    from pycamps.modules import RLLoad
    load = RLLoad('L1', RefFrameAngle=symbols('phi'), RefFrameSpeed=symbols('dphidt'), BaseSpeed=377)
```

::: pycamps.modules.ShortLine
    options:
        filters:
            - "!dynamics"
Example:
```python
    from sympy import symbols
    from pycamps.modules import ShortLine
    line = ShortLine('TL_1_2', RefFrameAngle=symbols('phi'), RefFrameSpeed=symbols('dphidt'), BaseSpeed=377)
```

::: pycamps.modules.SMOneAxis
    options:
        filters:
            - "!dynamics"
Example:
```python
    from sympy import symbols
    from pycamps.modules import SMOneAxis
    sm = SMOneAxis('G1', RefFrameAngle=symbols('phi'), RefFrameSpeed=symbols('dphidt'), BaseSpeed=377)
```

::: pycamps.modules.Type4_1
    options:
        filters:
            - "!dynamics"
Example:
```python
    from sympy import symbols
    from pycamps.modules import Type4_1
    sm = Type4_1('G1', RefFrameAngle=symbols('phi'), RefFrameSpeed=symbols('dphidt'), BaseSpeed=377)
```

::: pycamps.modules.Type4_1Gc
    options:
        filters:
            - "!dynamics"
Example:
```python
    from sympy import symbols
    from pycamps.modules import Type4_1Gc
    sm = Type4_1Gc('G1', RefFrameAngle=symbols('phi'), RefFrameSpeed=symbols('dphidt'), BaseSpeed=377)
```

::: pycamps.modules.Type4_2
    options:
        filters:
            - "!dynamics"
Example:
```python
    from sympy import symbols
    from pycamps.modules import Type4_2
    sm = Type4_2('G1', RefFrameAngle=symbols('phi'), RefFrameSpeed=symbols('dphidt'), BaseSpeed=377)
```

::: pycamps.modules.Type4_2Ec
    options:
        filters:
            - "!dynamics"
Example:
```python
    from sympy import symbols
    from pycamps.modules import Type4_2Ec
    sm = Type4_2Ec('G1', RefFrameAngle=symbols('phi'), RefFrameSpeed=symbols('dphidt'), BaseSpeed=377)
```