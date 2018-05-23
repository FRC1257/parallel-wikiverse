The Talon SRX has interesting behavior for current limiting, and is described using the following:

https://www.chiefdelphi.com/forums/showthread.php?threadid=163500

> Assuming all 3 are configured, based on the online docs, I understand that current limiting will be enabled whenever you exceed the continuous value for longer than peak_duration, if you exceed the peak value..... but this doesn't jive with the comment in their code sample.

> Part of this is a question to CTRE about what exactly the current limiting mechanism is... A brownout-style bang-bang where output is dropped to zero instantaneously for some period of time? or a more controlled approach until the input current reaches the threshold?

> FWIW, we attempted to use SRX-based current limiting this year on our drivetrain. After a few hours of playing with it and being unable to remove brownouts, we went back to our 2016 limiting method that we knew more about how to work with. It's still not perfect, but seems to be preventing brownouts without degrading performance too much.

> In all it's glorious asciiart format, here's basically what I'd hope for:

```
Current (current limiting enabled whenever motor current exceeds the limit)
^
|
|      ________ <- Peak Limit
|      |      |
|      |      |
|      |      |
|      |      |
|      |  ^   |
|______| / \  |_______________________________  <- Continuous Limit
|       /   \_________________________________  <- Actual Motor Current (happy motor)
|______/
|
+------+------+----------------------------------> time
       t=0    t=Peak Duration```
       
Note: this is not what I know for sure actually happens, just what I would hope for.
```

> In a nutshell - the peak limit allows for the motor current to jump high for a short period of time (ex when it experiences rapid acceleration), but otherwise limits to the continuous limit setting. Peak limit is still in place to ensure a short circuit or brownout-inducing current draw will immediately be squashed. Continuous limiting will keep the current draw acceptable in a slower ramp up, such as in a pushing match. /$0.02
