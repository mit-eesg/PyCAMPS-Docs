# `Miscellaneous`

::: pycamps.logger.configure_logging
Example:
```python
    import os
    os.environ['LOG_LEVEL'] = 'DEBUG'
    configure_logging(log_to_console=True, log_to_file=True)
    logger.debug("Test")
```