# automatic-irrigation-system
it deals with automatic watering of plants without any manual requirement
int a =10;
void setup()
{
  pinMode(led,OUTPUT);
  Serial.begin(9600);
}
void loop()
{
 int sensorValue= analogRead(A0);
 Serial.println(sensorValue);
 delay(200);
 if(sensorValue <=500)
  digitalWrite(a,HIGH);
 else
  digitalWrite(a,LOW);
  
   
}
 
