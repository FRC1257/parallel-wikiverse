# PID Tuning
In order to tune each of our PID controllers, we need to obtain the P, I, and D constants respectively. Below is a detailed procedure for how we tune our controllers using Test Mode for our robot:

## Procedure
1. Start by setting the P, I, and D constants to 0.4 (or 1), 0, and 0 respectively. We start by tuning P first.
    1. Set some arbitrary setpoint value (say 90° or 100”) and test how effective the P coefficient is. With a start value of 1, the robot will likely oscillate a lot.
        1. If our start coefficient is too high, we proceed with a binary search from the 1 to 0. 
            1. If a given value for P is too high and causes too much oscillation, we decrease the P by testing the midpoint between the current value and lowest known working value.
                1. Ex. Let’s say that we know that a constant of 0.4 is too high and a value of 0.2 is too low. We would test the midpoint between them (0.3). If that P is too high again, we test the midpoint of 0.3 and 0.2 (0.25). If the P is too low, we test the midpoint between 0.4 and 0.3 (0.35).
        2. If the start coefficient is too low, we continually increase it by a factor of 2 or 10 until we find a coefficient that is too high. Then, we continue to refine our coefficient using a binary search technique detailed above
        3. This process continues until we’ve found a P that gets us to our setpoint with minimal oscillation. We want to ensure that our robot at least reaches the setpoint (and doesn’t stop before the desired one with a steady-state error)
2. Next, we try to minimize overshoot and oscillations by tuning the D constant. We use the previous value for P and start with D at 1.
    1. We use the same procedure to tune P on the coefficient for D (using a binary search).
        1. A D term that is too high is characterized by very frequent and small oscillations
        2. A D term that is too small will not decrease rise time enough
    2. After tuning the D term, our controller should be pretty will function with minimal rise time/overshoot. However, a steady state error may still remain.
3. If there is a steady state error in the controller, we need to tune the I term. 
    1. Start with the previously obtained P and D terms, set I to a lower value (typically 0.1), and proceed with a binary search as described above.
    1. A properly tuned I term should eliminate any small steady-state error still present in the controller.
