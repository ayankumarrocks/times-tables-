// C++ code
//
int i = 0;

int multiplier = 0;

int product = 0;

int j = 0;

void setup()
{
  Serial.begin(9600);

  for (i = 1; i <= 10000000000000000; i += 1) {
    for (multiplier = 1; multiplier <= 10; multiplier += 1) {
      Serial.print(i);
      Serial.print("*");
      Serial.print(multiplier);
      Serial.print("=");
      product = (i * multiplier);
      Serial.println(product);
      delay(1); // Wait for 1 millisecond(s)
    }
  }
}

void loop()
{
  delay(10); // Delay a little bit to improve simulation performance
}
