## Intro Lesson

Using the Blockly Interface
* https://codrone.robolink.com/edu/blockly/

<pre>
# This code is generated in Python as you drag the blocks from the left tab.
  
import time
from codrone_edu.drone import *

drone = Drone()
drone.open()

drone.drone_buzzer(Note.C3, 1000)
drone.takeoff()
drone.land()

drone.close()
  
</pre>

![image](https://github.com/ions29/cpp-reading-material/assets/127531384/5a3ffc9b-edfd-49d0-9480-b9c4e0ee7eb8)
