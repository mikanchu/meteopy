# Installation Requirements
* Conda environment
* Import conda environment
` conda env env_name -f requirements/0_conda_envoronment.yml`
* Import pip requirement
` pip install -r requirements/1_pip_requirements.txt`

# Hardware
* Raspberry Pi 3 V2
* Arduino/Genuino Uno
* Protoboards
* Displays
* Sensor LM35

# Cases

## four step motor

For the 4 step motor, we used `Step motor 28BYJ-48`.

We connected it on the following ports.

| Arduino port | Controller port|
|:------------:|:--------------:|
| Digital 9    | IN1            |
| Digital 10   | IN2            |
| Digital 11   | IN3            |
| Digital 12   | IN4            |

The controller accepts an input of 5 or 12V. We chose to use 5V and have it plugged directly to the board.

The code can be found in the `arduinosrc`

## Variation of 4 step motor

- Checks data from the serial
- If the data is different from the current status, plays the intro of Mario from the buzzer and turns the motor

Maybe it would be nice to play the imperial march instead when the status changes...

*NOTE*: In order to keep the health of your buzzer, a resistance of 220Ω is needed for the input
