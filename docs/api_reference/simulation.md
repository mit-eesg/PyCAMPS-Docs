::: pycamps.simulation.power_system.PowerSystem
    options:
        filters:
            - "!produce_g_matrix"
Example:
```python
    from pycamps.simulation import PowerSystem
    from pycamps.modules import ShortLine, SMOneAxis, PQLoad
    # Create modules like you normally would    
    modules = [ShortLine(...), SMOneAxis(...), PQLoad(...)]
    # Create and connect buses using the following format:
    # [[(non-wire1), (wire1, 'terminal')],
    #  [(non-wire2), (wire1, 'other_terminal')]]
    buses = [[(modules[0], 'L'), (modules[1])],
     [(modules[0], 'R'), (modules[2])]]
    ps = PowerSystem("MyPowerSystem", modules, buses)
    print(ps.StateSpaceEquations)
```

::: pycamps.simulation.dynamics.Dynamics
Example:
```python
    from pycamps.simulation import PowerSystem, Dynamics
    ps = PowerSystem(...) # Create power system like normal
    dynamics = Dynamics(ps)
    print(dynamics.get_required_parameters())
    dynamics.load_new_params(params_directory='path/to/params/')
    equilibrium = dynamics.solve_equilibrium()
    time, states = dynamics.simulate_trajectory()
    A, sub_pf, states = dynamics.linearized_analysis()
```

::: pycamps.simulation.state_space.StateSpace
Example:
```python
    from pycamps.simulation import StateSpace, PowerSystem
    ps = PowerSystem(...) # Create power system like normal
    ss = StateSpace.from_power_system(ps)
    ss.print_equations()
```