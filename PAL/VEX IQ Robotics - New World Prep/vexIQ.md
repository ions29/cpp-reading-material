## Lesson 1: Install VEXcode IQ
* https://www.vexrobotics.com/vexcode/install/iq
  
![image](https://github.com/ions29/cpp-reading-material/assets/127531384/24811db4-2bf7-43a8-bd1d-f620f6cb0581)


If you are having issues installing this on your laptop, we can use the online Interactive Development Environment (IDE) instead.
* https://codeiq.vex.com/


## Lesson 6: Coverting the Project to Text


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

![image](https://github.com/ions29/cpp-reading-material/assets/127531384/ed1b35ef-3970-47e7-a811-b47fbc465974)





![image](https://github.com/ions29/cpp-reading-material/assets/127531384/5902a463-cd98-4be3-9e3f-6897d3bef825)

