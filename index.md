# IGS Zero Robotics Mini Competition

## Competition
 
 - SpySpheres 2D
 - [Game Manual Link](https://goo.gl/igu9Bx)

## Dates

Event | Date
---|---
Competition Start | 2018-08-10
First Round | 2018-08-24
Second Round | 2018-08-31
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

### Get Distance Between Points

```c
float distance(float a[], float b[]) {
    float tmpArray[3];
    mathVecSubtract(tmpArray, a, b, 2);
    mathVecNormalize(tmpArray, 2);
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


