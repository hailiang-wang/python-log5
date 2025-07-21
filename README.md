# Python log5
https://github.com/hailiang-wang/python-log5

```
pip install -U log5
```

Usage:

```
import env3
ENV = env3.load_env(os.path.join(os.getcwd(), ".env")) # set LOG_LEVEL and LOG_FILE in .env

import log5
logger = log5.get_logger(log5.LN(__name__), output_mode=log5.OUTPUT_STDOUT)
logger.debug('bar')
logger.info('foo')

log5.set_log_level(log5.ERROR)
logger.info('foo2')
```

# Config

## output_mode

output_mode = `log5.OUTPUT_STDOUT(default) | log5.OUTPUT_FILE | log5.OUTPUT_BOTH`

## Environment Variables

LOG_LEVEL=`CRITICAL|ERROR|WARNING|INFO|DEBUG`, default is INFO

LOG_FILE=`A FILE PATH TO WRITE LOG`, default is `os.path.join(os.getcwd(), 'default.log')`

# Package deps

Get details in [setup](https://github.com/hailiang-wang/python-log5/blob/master/setup.py).

# License
[LICENSE](./LICENSE)