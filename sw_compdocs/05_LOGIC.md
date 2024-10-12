# Logic

## Abs

Outputs the absolute value of a number input.

Negative numbers are converted to positive numbers, whilst positive numbers are unchanged.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x2x1
- Cost: $20
- Tags: 
- File: gate_float_abs.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| number | Input Number | The number to get the absolute value of. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Absolute Value | The absolute value of the input. |

## Add

Takes two number inputs, adds them together, and outputs the result.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 2x2x1
- Cost: $20
- Tags: 
- File: gate_float_add.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| number | A | The first value to be added. |
| number | B | The second value to be added. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | A + B | Outputs the result of A + B. |

## And

A logic gate that outputs the logical AND of two input signals.

The output will only be switched on if both inputs are on.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 2x2x1
- Cost: $20
- Tags: 
- File: gate_bool_and.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | A | The first value to perform the logical AND on. |
| on/off | B | The second value to perform the logical AND on. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | A AND B | Outputs an on signal when both A and B are on, and an off signal if either one is off. |

## Blinker

The blinker outputs a value that blinks between on and off at a set rate.

You can set the duration that the signal should stay on and off for by selecting it with the select tool. A control signal determines whether or not the blinker should output anything. If the control signal is off, the blinker's output will be off. The internal blink timer is reset every time the control signal is switched off.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x2x1
- Cost: $20
- Tags: 
- File: gate_bool_blink.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Control Signal | Controls whether or not the blinker should output anything at all. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Blinking Signal | Outputs a signal that blinks between on and off at the set rate when the control signal is on. Outputs off if the control signal is off. |

## Capacitor

Charges up when receiving an on signal, then discharges over a period of time.

The charge and discharge times can be configured by selecting this component with the select tool. Once charged, inputting a new signal will reset the discharge timer.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x2x1
- Cost: $20
- Tags: 
- File: gate_bool_capacitor.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Charge | Charges the capacitor when on, discharges when off. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Stored Charge | The capacitor's stored charge. |

## Clamp

The clamp takes a number input and clamps it to a set range.

The upper and lower values to clamp to can be configured by selecting this component with the select tool.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x2x1
- Cost: $20
- Tags: 
- File: gate_float_clamp.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| number | Number to Clamp | The value to clamp within the upper and lower bounds. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Clamped Number | The input after being clamped within the upper and lower bounds. |

## Constant Number

Outputs a constant numerical value.

The number that is being outputted can be configured by selecting this component with the select tool.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $20
- Tags: 
- File: gate_float_constant.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Constant Number | The selected output number. |

## Constant On Signal

A simple logic component that continuously outputs an on signal.

This is useful for creating logic circuits that are permanently switched on.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $20
- Tags: 
- File: gate_bool_constant.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | On | Outputs a constant on signal. |

## Counter

A counter which increases with a set speed.

Stores and constantly outputs a value which increases by an input amount.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x2x1
- Cost: $20
- Tags: 
- File: gate_float_counter.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| number | Speed | The speed the count rises by. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Count | The current count. |

## Counter (Ping Pong)

A counter which oscillates between -1 and +1 with a set speed.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x2x1
- Cost: $20
- Tags: 
- File: gate_float_counter_ping_pong.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| number | Speed | The speed the count changes by. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Count | The current count. |

## Delay

This component stores an input on/off signal, and then outputs it after a delay.

The delay time can be configured by selecting the component with the select tool. The internal delay timer is reset whenever the input signal changes.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x2x1
- Cost: $20
- Tags: 
- File: gate_bool_delay.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Signal to Delay | Can be an on or off signal. Changing this will reset the delay's timer. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Delayed Signal | The input signal that has been delayed. |

## Divide

Takes two number inputs, divides one by the other, and outputs the result.

If a division by 0 occurs, an on signal will be produced and the output number value will be set to 0.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 2x2x1
- Cost: $20
- Tags: 
- File: gate_float_divide.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| number | A | The number to divide. |
| number | B | The number to divide by. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Error | Outputs true when a division by 0 occurs. |
| number | A / B | The result of A divided by B, or 0 attempting to divide by 0. |

## Exponent

Outputs its input raised to the power of a selected exponent.

The exponent can be changed by selecting this component with the select tool.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x2x1
- Cost: $20
- Tags: square,cube,root,sqrt,pow
- File: gate_float_exponent.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| number | Input Number | The number to exponentiate. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Powered Number | The input raised to the power of the selected exponent. |

## Function (1 input)

Evaluates a mathematical function with 1 variable inputs

The function can be entered by selecting this component with the select tool. A full list of valid operations are also visible in the component's selection menu.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x2x1
- Cost: $80
- Tags: 
- File: gate_function_small.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| number | Input 1 (x) | X input to the function. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | f(x) | Outputs the evaluation of the entered function. |

## Function (3 inputs)

Evaluates a mathematical function with up to 3 variable inputs.

The function can be entered by selecting this component with the select tool. A full list of valid operations are also visible in the component's selection menu.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 2x2x1
- Cost: $100
- Tags: 
- File: gate_function_large.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| number | Input 1 (x) | X input to the function. |
| number | Input 2 (y) | Y input to the function. |
| number | Input 3 (z) | Z input to the function. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | f(x,y,z) | Outputs the evaluation of the entered function. |

## Greater-than

Compares two numerical values.

Outputs an on signal if the first input is greater than the second, and outputs an off signal if the first input is less than or equal to the second.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 2x2x1
- Cost: $20
- Tags: 
- File: gate_float_greater_than.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| number | A | The value to compare. |
| number | B | The value to be compared to. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | A GREATER THAN B | Outputs an on signal if A is greater than B. Outputs an off signal if A is less than or equal to B. |

## JK Flip-Flop

A JK flip-flop that can be set and reset using two on/off inputs.

When both inputs are off, there is no change in state. If both Set and Reset are set to on, the state will be toggled.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 2x2x1
- Cost: $20
- Tags: 
- File: gate_jk_flipflop.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Set | Sets the output to on. |
| on/off | Reset | Sets the output to off. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Output | The internal state of the flip-flop. |
| on/off | NOT Output | The inverse of the internal state of the flip-flop. |

## Less-Than

Compares two numerical values.

Outputs an on signal if the first input is less than the second, and outputs an off signal if the first input is greater than or equal to the second.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 2x2x1
- Cost: $20
- Tags: 
- File: gate_float_less_than.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| number | A | The value to compare. |
| number | B | The value to be compared to. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | A LESS THAN B | Outputs an on signal if A is less than B. Outputs an off signal if A is greater than or equal to B. |

## Memory Register

A memory register that can store a number value.

The number input will be stored when an on signal is received. A secondary on/off signal can be used to clear the stored value, resetting it to the configured value set using the select tool.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 2x2x1
- Cost: $20
- Tags: 
- File: gate_float_register.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| number | Value to Store | The value that will be stored when receiving an on signal. |
| on/off | Set | Stores the input value when receiving an on signal. |
| on/off | Clear | Resets the stored value to 0. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Stored Value | The value that is stored in the memory. |

## Microprocessor

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $100
- Tags: 
- File: microprocessor.xml

## Modulo

Takes two number inputs, outputs the remainder after dividing the first by the second.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 2x2x1
- Cost: $20
- Tags: 
- File: gate_float_modulo.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| number | A | The value to modulo. |
| number | B | The value to modulo A by. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | A % B | Outputs the remainder when A is divided by B. |

## Multiply

Takes two number inputs, multiplies them together, and outputs the result.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 2x2x1
- Cost: $20
- Tags: 
- File: gate_float_multiply.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| number | A | The value to be multiplied. |
| number | B | The value to multiply by. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | A x B | Outputs the result of multiplying A by B. |

## Not

A logic gate that outputs the logical NOT of its input signal.

The output will always be the opposite of the input.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x2x1
- Cost: $20
- Tags: 
- File: gate_bool_not.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | A | The signal to invert. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | NOT A | The logical NOT of input A. This output will always be the opposite of the input. |

## Numerical Inverter

The inverter takes a number as input, multiplies it by -1, and outputs the result.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x2x1
- Cost: $20
- Tags: 
- File: gate_float_invert.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| number | Number to Invert | The number that will be inverted. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Inverted Number | The inverse of the input. This is equivalent to multiplying the input by -1. |

## Numerical Junction

Acts as a junction for two number signals.

The junction can be switched using an on/off signal. When the signal is on, the number is passed through to the first output and a value of 0 is passed to the second. When the signal is off, the number is passed through to the second output with the first being set to 0.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 2x2x1
- Cost: $20
- Tags: 
- File: gate_float_switch.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Switch Signal | Controls which of the two output paths the input value will be sent to. |
| number | Value to Pass Through | The value to pass through the junction. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | On Path | Receives the input value when the switch signal is set to on. |
| number | Off Path | Receives the input value when the switch signal is set to off. |

## Numerical Switchbox

Acts as a switchbox for two number signals.

Which of the two inputs is sent to the output is determined by the on/off switch signal. When the signal is on, the first value is sent to the output. When it is off, the second output is sent.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 2x2x1
- Cost: $20
- Tags: 
- File: gate_float_switch_input.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Switch Signal | Controls which of the two input values will be sent to the output. |
| number | First Value (On) | The value to output when the switch signal is on. |
| number | Second Value (Off) | The value to output when the switch signal is off. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Switched Value | Outputs the first value when the switch signal is on, and the second value when it is off. |

## Or

A logic gate that outputs the logical OR of two input signals.

The output will be switched on if either of the inputs is on, and off if neither are on.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 2x2x1
- Cost: $20
- Tags: 
- File: gate_bool_or.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | A | The first value to perform the logical OR on. |
| on/off | B | The second value to perform the logical OR on. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | A OR B | Outputs an on signal when either A or B are on, and an off signal if neither are on. |

## PID Controller

A control loop feedback mechanism that measures and corrects the error in a system over time.

It takes the current measured output of a system or sensor, and a desired target measurement. It outputs a value that can be used as an input to the system to gradually correct its error. For example, the controller could input to an engine's throttle to maintain a desired speed or altitude. The control terms (proportional, integral and derivative) can be set by selecting the component with the select tool. The control terms must be carefully tuned for optimal output.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 2x2x1
- Cost: $100
- Tags: 
- File: gate_pid_controller.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Active | Sets whether or not the controller is active. When inactive, stored values are reset. |
| number | Process Variable | The current measured value of the system. |
| number | Setpoint | The desired value to correct the process variable to. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Control Output | The output computed by the controller. |

## Push to Toggle

This component has an internal on/off switch that is toggled every time a new on signal is sent to its input.

This can allow regular push buttons to act as toggle buttons.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x2x1
- Cost: $20
- Tags: 
- File: gate_push_to_toggle.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Toggle Signal | An on signal toggles the internal on/off switch. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Internal State | The output of the internal on/off switch. |

## SR Latch

An SR latch that can be set and reset using two on/off inputs.

When both inputs are off, there is no change in state. If both Set and Reset are set to on, Reset will take precedence.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 2x2x1
- Cost: $20
- Tags: 
- File: gate_sr_latch.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Set | Sets the output to on. |
| on/off | Reset | Sets the output to off. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Output | The internal state of the latch. |
| on/off | NOT Output | The inverse of the internal state of the latch. |

## Subtract

Takes two number inputs, subtracts the second from first, and outputs the result.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 2x2x1
- Cost: $20
- Tags: 
- File: gate_float_subtract.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| number | A | The value to subtract from. |
| number | B | The value to subtract. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | A - B | Outputs the result of subtracting B from A. |

## Threshold Gate

Takes a value and compares it to a set threshold.

A lower and upper bound to the threshold must be set. The output is set to on if the input value is less than or equal to the upper bound, and greater than or equal to the lower bound. If it is outside this range, the output is set to off. The threshold bounds can be configured by selecting this component with the select tool.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x2x1
- Cost: $20
- Tags: 
- File: gate_float_threshold.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| number | Value to Test | The value to test within the threshold. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Within Threshold | Outputs an on signal when the input value is within the set threshold. |

## Trigonometry

Provides a set of basic trigonometry functions.

The available functions are sin, cos, tan, asin, acos and atan. If an invalid number is input, the output will be 0. Sin, cos and tan accept inputs measured in turns. Asin, acos and atan output values measured in turns. The function can be set by selecting this component with the select tool.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x2x1
- Cost: $20
- Tags: sine,cosine,tangent,asin,atan,acos,inverse,function
- File: gate_float_sin.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| number | Input Number | The input to the function. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | f(x) | f(x), where f is the selected function and x is the input. |

## Up/Down

This component uses two on/off signals to move an internal value between -1 and 1.

The up input moves the value towards 1, and the down input moves it towards -1. This component can be used for converting on/off button presses into a standard number value that can be used to control any mechanical components that accept a standard number input.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 2x2x1
- Cost: $20
- Tags: 
- File: gate_up_down.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Up | Moves the internal value towards 1. |
| on/off | Down | Moves the internal value towards -1. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Up/Down Value | The internally stored value between -1 an 1. |

## Xor

A logic gate that outputs the logical XOR of two input signals.

The output will be switched on if only one of the signals are on. The output will be switched off if the two signals are the same.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 2x2x1
- Cost: $20
- Tags: 
- File: gate_bool_xor.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | A | The first value to perform the logical XOR on. |
| on/off | B | The first value to perform the logical XOR on. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | A XOR B | Outputs an on signal if only A is on, or only B is on. The output is off if A and B are both on or off. |

## Power Add (Deprecated)

> [!WARNING]
> This component is deprecated.

Combines the outputs of two engines, allowing you to connect multiple engines to the same input.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 2x2x1
- Cost: $20
- Tags: 
- File: gate_torque_add.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| power | Combined Power | Outputs the combined power of engine 1 and 2. |

## Power Meter (Deprecated)

> [!WARNING]
> This component is deprecated.

The power meter allows you to take a measurement of how much power is being output from an engine to a specific component.

To prevent a loss of power, it should be connected in series between the engine and its receiving component.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 2x2x1
- Cost: $20
- Tags: 
- File: gate_torque_multimeter.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| power | Relay | Relays the power received from an engine. |

## Train Junction Controller (Deprecated)

> [!WARNING]
> This component is deprecated.

This component has an internal on/off switch that is toggled every time a new on signal is sent to its input.

This can allow regular push buttons to act as toggle buttons.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x2x1
- Cost: $20
- Tags: 
- File: gate_train_junction.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Toggle Signal | An on signal toggles the internal on/off switch. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Internal State | The output of the internal on/off switch. |
