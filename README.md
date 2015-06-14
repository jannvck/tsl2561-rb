# tsl2561-rb
TAOS TSL2561 lightsensor ruby library

Straightforward to use:

```
lightSensor = LightSensor.new("/dev/i2c-1")
lightSensor.turnOn
sleep(0.420)
luminosity = lightSensor.getLuminosity
puts "lux=#{luminosity.calcLux}"
lightSensor.turnOff
```