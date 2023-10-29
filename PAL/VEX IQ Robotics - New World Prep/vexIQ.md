## Lesson 1: Install VEXcode IQ
* https://www.vexrobotics.com/vexcode/install/iq
  
![image](https://github.com/ions29/cpp-reading-material/assets/127531384/24811db4-2bf7-43a8-bd1d-f620f6cb0581)


If you are having issues installing this on your laptop, we can use the online Interactive Development Environment (IDE) instead.
* https://codeiq.vex.com/


You can follow the program in either C++ or Python - just let me know what version you choose!

## Lesson 2: Console Screen [ Done in C++ ]

<pre>
int Brain_precision = 0, Console_precision = 0;

float myVariable;

// "when started" hat block
int whenStarted1() {
  Brain.playSound(wrench);
  return 0;
}

// "when buttonDown released" hat block
void onevent_buttonDown_released_0() {
  Brain.playSound(tada);
  Brain.playNote(3, 0, 500);
  Brain.Screen.print("YourName");
  Brain.Screen.newLine();
}


int main() {
  // Calibrate the Drivetrain Gyro
  calibrateDrivetrain();

  // register event handlers
  Brain.buttonDown.released(onevent_buttonDown_released_0);

  wait(15, msec);
  whenStarted1();
}
  
</pre>

![image](https://github.com/ions29/cpp-reading-material/assets/127531384/3f865396-05dc-4754-9b97-5f4c44ae2adc)


## Lesson 2: Console Screen [Done in Python]

<pre> 
vexcode_brain_precision = 0
vexcode_console_precision = 0
myVariable = 0

def when_started1():
    global myVariable, vexcode_brain_precision, vexcode_console_precision
    brain.play_sound(SoundType.WRENCH)

def onevent_buttonRight_released_0():
    global myVariable, vexcode_brain_precision, vexcode_console_precision
    brain.play_sound(SoundType.TADA)
    brain.play_note(3, 0, 500)
    brain.screen.print("YourName")
    brain.screen.next_row()

def onevent_buttonLeft_pressed_0():
    global myVariable, vexcode_brain_precision, vexcode_console_precision
    brain.screen.clear_screen()
    brain.screen.draw_line(0, 0, 10, 10)

# Calibrate the Drivetrain Gyro
calibrate_drivetrain()

# system event handlers
brain.buttonRight.released(onevent_buttonRight_released_0)
brain.buttonLeft.pressed(onevent_buttonLeft_pressed_0)
# add 15ms delay to make sure events are registered correctly.
wait(15, MSEC)

when_started1()


</pre>

![image](https://github.com/ions29/cpp-reading-material/assets/127531384/18d93fbc-cdaf-4663-9d8a-92403e9a03da)


## Lesson 3: Drivetrain Configuration

Left Motor Port Configuration

![image](https://github.com/ions29/cpp-reading-material/assets/127531384/6af83706-18ac-4989-a030-5155755fb08d)

Right Motor Port Configuration
![image](https://github.com/ions29/cpp-reading-material/assets/127531384/108f6eee-769d-478e-b243-4c696a077839)

Gyro Configuration (if you have a drone that uses a gyro)
![image](https://github.com/ions29/cpp-reading-material/assets/127531384/036e08a3-a896-4083-a932-e1dee68f5ed1)






## Lesson 6: Coverting the Project to Text

<pre>
// "when started" hat block
int whenStarted1() {
  Brain.playSound(siren);
  wait(1.0, seconds);
  Brain.playNote(3, 0, 1000);
  return 0;
}


int main() {
  // Calibrate the Drivetrain Gyro
  calibrateDrivetrain();

  whenStarted1();
}
</pre>
![image](https://github.com/ions29/cpp-reading-material/assets/127531384/ed1b35ef-3970-47e7-a811-b47fbc465974)

