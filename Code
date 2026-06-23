/*
 Smart Temperature Controlled Fan
 Author: Rama Tulasi
*/

int temp_value;        // raw sensor value
float temperature;     // converted temperature

void setup() {
    pinMode(9, OUTPUT);      // PWM pin for fan
    Serial.begin(9600);      // for monitoring
}

void loop() {

    temp_value = analogRead(A0);   // read LM35 sensor

    temperature = temp_value * 0.488;   // convert to °C

    Serial.print("Temperature: ");
    Serial.println(temperature);

    if (temperature < 25) {
        analogWrite(9, 0);       // Fan OFF
    }
    else if (temperature < 35) {
        analogWrite(9, 120);     // Medium speed
    }
    else {
        analogWrite(9, 255);     // Full speed
    }

    delay(1000);   // 1 second delay
}
