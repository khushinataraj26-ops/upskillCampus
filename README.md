# upskillCampus
void setup() {
  // Use INPUT_PULLUP to prevent "floating" pin issues
  pinMode(2, INPUT_PULLUP); 
  pinMode(13, OUTPUT);
}

void loop() {
  // With INPUT_PULLUP, the logic is reversed:
  // LOW = Button Pressed | HIGH = Button Released
  if (digitalRead(2) == LOW) { 
    digitalWrite(13, HIGH); // LED On
  } else {
    digitalWrite(13, LOW);  // LED Off
  }
}
