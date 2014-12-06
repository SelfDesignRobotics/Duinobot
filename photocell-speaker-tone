/*
Modified from Adafruit Arduino - Lesson 10. Pseudo Thermin
Demonstrates assiging pin 22 or using the predefined SPEAKER constant which is mapped to pin 22 in order to access built-in speaker (piezo element).
*/

int photocellPin = A0; // Attach Multiplo photocell sensor to SO. (analog 0)
int speakerPin = 22; // uncomment this line to use speakerPin variable instead of SPEAKER

void setup()
{
Serial.begin(57600);
}

void loop()
{
  int reading = analogRead(photocellPin);
  int pitch = 110 + reading / 2;
  tone(speakerPin, pitch, 0); // uncomment this line to use speakerPin variable instead of SPEAKER
  //tone(SPEAKER, pitch, 0); // uncomment this line to use predefined SPEAKER constant
  delay(20);

  Serial.println(reading);
  delay(50);
}
