# `Simulation Tools`

::: pycamps.simulation.PowerSystem
    options:
        filters:
            - "!produce_g_matrix"
Example:
```python
    from pycamps.simulation import PowerSystem
    from pycamps.modules import ShortLine, SMOneAxis, PQLoad
    modules = [ShortLine(...), SMOneAxis(...), PQLoad(...)]
    buses = [[(modules[0], 'L'), (modules[1])], [(modules[0], 'R'), (modules[2])]]
    ps = PowerSystem("MyPowerSystem", modules, buses)
    print(ps.StateSpaceEquations)
```

::: pycamps.simulation.Dynamics
Example:
```python
    from pycamps.simulation import PowerSystem, Dynamics
    ps = PowerSystem(...)
    dynamics = Dynamics(ps)
    print(dynamics.get_required_parameters())
    dynamics.load_new_params(params_directory='params/')
    equilibrium = dynamics.solve_equilibrium()
    time, states = dynamics.simulate_trajectory()
    sub_pf, states = dynamics.linearized_analysis()
```

::: pycamps.simulation.StateSpace
Example:
```python
    from pycamps.simulation import StateSpace, PowerSystem
    ps = PowerSystem(...)
    ss = StateSpace.from_power_system(ps)
    ss.print_equations()
```