## Lesson 1: Install VEXcode IQ
* https://www.vexrobotics.com/vexcode/install/iq
  
![image](https://github.com/ions29/cpp-reading-material/assets/127531384/24811db4-2bf7-43a8-bd1d-f620f6cb0581)


If you are having issues installing this on your laptop, we can use the online Interactive Development Environment (IDE) instead.
* https://codeiq.vex.com/

## Lesson 2: Console Screen

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

