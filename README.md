# Lit Stopwatch
A simple stopwatch for [Luvit](https://luvit.io)

## Install
```sh
$ lit install ravener/stopwatch
```

## Usage
```lua
local stopwatch = require("stopwatch")

-- Create a stopwatch (it is immediately started)
-- Argument is decimal precision for tostring() (defaults to 2)
local timer = stopwatch(2)

-- Stop the timer.
timer:stop()

-- Start the timer.
timer:start()

-- Restart the timer from zero.
timer:restart()

-- Stop and reset the timer.
timer:reset()

-- The duration of the stopwatch in milliseconds.
print(timer.duration)

-- Whether the stopwatch is running.
print(timer.running)

-- Get a human readable string of the duration.
tostring(timer)
print(timer)
```

## License
[MIT License](LICENSE)
