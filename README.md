
***Algorithm to move the Servo Motor as the Robot legs***
1. Serial Communication Setup
   - Open the serial port at a baud rate of 9600.

2. Define Motor Movement Function
```ruby
   - Start function move_motor(motor_number, angle)
{
   This function sends the motor num and the angle
}
```
3. Define Walking Step Function
```ruby
   - Start function walk()
{
     - Move the front leg -> Call move_motor(1, 90)
     - Delay for 0.5 seconds.
     - Return the front leg to the original position -> Call move_motor(1, 30) // Return front leg backward.
     - Delay for 0.5 seconds.
}
```
5. Main Loop
```ruby
   - While true:
   - Call walk()  repeatedly.
```
