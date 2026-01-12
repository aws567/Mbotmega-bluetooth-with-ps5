#include <MeMegaPi.h>

// Define motors
MeMegaPiDCMotor m1(PORT1A);
MeMegaPiDCMotor m2(PORT1B);
MeMegaPiDCMotor m3(PORT2A);
MeMegaPiDCMotor m4(PORT2B);

void setup() {
  Serial.begin(9600); // Listen to Python commands
}

void loop() {
  if (Serial.available()) {
    char cmd = Serial.read();
    switch (cmd) {
      case 'F': // Forward
        m1.run(150);
        m2.run(-150);
        m3.run(150);
        m4.run(-150);
        break;
      case 'B': // Backward
        m1.run(-150);
        m2.run(150);
        m3.run(-150);
        m4.run(150);
        break;
      case 'L': // Turn left
        m1.run(-150);
        m2.run(-150);
        m3.run(-150);
        m4.run(-150);
        break;
      case 'R': // Turn right
        m1.run(150);
        m2.run(150);
        m3.run(150);
        m4.run(150);
        break;
      case 'S': // Stop
        m1.run(0);
        m2.run(0);
        m3.run(0);
        m4.run(0);
        break;
    }
  }
}
