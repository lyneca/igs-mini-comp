# IGS Zero Robotics Mini Competition

## Competition
 
 - SpySpheres 2D
 - [Game Manual Link](http://static.zerorobotics.mit.edu/docs/hs/3DManualZRHS2015.pdf)

## Dates

Event | Date
---|---
Competition Start | 2018-08-10
First Round | 2018-08-31
Final Round | 2018-08-07

## Code

### Get Attitude To Target

```c
// getAttToTarget(array, myPos, targetPos);
// api.setAttitudeTarget(array);
void getAttToTarget(float returnArray[], float me[], float target[]) {
    mathVecSubtract(returnArray, target, me, 2);
    mathVecNormalize(returnArray, 2);
}
```

### Multiply a vector by a scalar
```c
void mathVecScalarMult(float ret[3], float a[3], float s, int n) {
    for (int i = 0; i < n; i++) {
        ret[i] = a[i] * s;
    }
}
```

### Get Distance Between Points

```c
float distance(float a[3], float b[3]) {
    float ret[3];
    mathVecSubtract(ret, a, b, 3);
    return mathVecMagnitude(ret, 3);
}
```

### Get the midpoint of two positions

```c
void mathVecMiddle(float ret[3], float a[3], float b[3], int n) {
    mathVecSubtract(ret, a, b, 3);
    mathVecScalarMult(ret, ret, 0.5f, n);
}
```


## Teams

### Team: Death by Stalkery

 - Perri
 - Tom
 - India
 - Nick
 - Tilli

### Team: /kill @e[name=!commandBlock]

 - Luke O
 - Jake
 - The other Jake
 - Emil
 - Donovan
 - Louis
 - Max

## Scores

Team              | Round 1 | Round 2 | Round 3 | Total
---               | ---     | ---     | ---     | ---
`/kill`           | 4.909   | 0.340   | 0.370   | 5.619
Death By Stalkery | 0.110   | 2.388   | 2.586   | 5.084



