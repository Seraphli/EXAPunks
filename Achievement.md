# Achievement Guide

## PIZZA_PARTY

**Level:** Euclid's Pizza

**Solution:**

```
NOTE XA
LINK 800
LINK 800
LINK 805
@REP 10
COPY 0 #POWR
COPY 1 #POWR
@END
```

## DISC_READ_ERROR

**Level:** Sawayama Wonderdisc

**Solution:**

```
NOTE XA
GRAB 300
COPY F X
DROP
LINK 800
COPY 8 #AUTH
COPY 0 #AUTH
COPY 3 #AUTH
COPY 2 #AUTH
COPY 7 #AUTH
COPY 1 #AUTH
COPY 0 #AUTH
COPY 4 #AUTH
COPY 9 #AUTH
COPY 5 #AUTH
COPY 1 #AUTH
COPY 2 #AUTH
COPY 5 #AUTH
COPY 2 #AUTH
COPY 6 #AUTH

MARK L
REPL C
VOID M
REPL C2
JUMP L

MARK C
MODE
COPY #TRAK T
LINK 801
GRAB T
REPL FILE
MARK L1
COPY F M
TEST EOF
FJMP L1
COPY -1 M

MARK FILE
MAKE
MARK L2
COPY M F
SEEK -1
TEST F > 0
TJMP L2
SEEK -1
TEST F = -1
TJMP END
SEEK -1
COPY X F
JUMP L2
MARK END
SEEK -1
VOID F
LINK -1
LINK 800
MODE
COPY 1 M
HALT

MARK C2
LINK 800
KILL
```

## HOME_RUN

**Level:** Xtreme League Baseball

**Solution:**

```
LINK 800
LINK 799
@REP 4
LINK 800
@END
```

## TONER_LOW

**Level:** Zebros Copies

**Solution:**

```
LINK 800
LINK 800
@REP 4
REPL C@{1,1}
@END

@REP 4
MARK C@{1,1}
LINK 80@{0,1}
JUMP L
@END
MARK L
COPY 1 #COPY
JUMP L
```

**Note:** You have to keep running this code until you unlock the achievement. Start over if you reach the maximum cycles.

## KLEPTOMANCER

**Level:** Kings Ransom Online

**Solution:**

```
GRAB 300
WIPE
LINK 800
COPY 6 T
MARK L1
SUBI T 1 T
REPL C
TJMP L1
@REP 5
NOOP
@END
COPY 6 T
MARK L2
SUBI T 1 T
REPL C1
TJMP L2
HALT

MARK C
ADDI 800 T T
LINK T
KILL
KILL
KILL
HALT

MARK C1
ADDI 800 T T
LINK T
COPY 201 X
COPY 99 T
MARK C1L
MODI -1 T T
REPL C2
JUMP C1L
HALT

MARK C2
ADDI X T X
GRAB X
SEEK 1
TEST F > 0
FJMP C2E
LINK -1
LINK -1
MARK C2E
```

## BLACKOUT

**Level:** Allience Power And Light

**Solution:**

```
LINK 800
MARK L
COPY 2 T
REPL C1
REPL C2
COPY 1 T
REPL C1
REPL C2
REPL CHECK
LINK 801
JUMP L

MARK C1
LINK 800
SUBI T 1 T
TJMP C1
JUMP CHECK

MARK C2
LINK 802
SUBI T 1 T
TJMP C2
JUMP CHECK

MARK CHECK
COPY 0 #POWR
```

## RITE_OF_PASSAGE

**Level:** TEC Redshift

**Solution:**

```
LINK 800
REPL LOOP
ADDI X 1 X
NOOP
NOOP

MARK LOOP
SWIZ X 1 #PASS
SWIZ X 2 #PASS
SWIZ X 3 #PASS
REPL J
ADDI X 2 X
TEST MRD
TJMP END
JUMP LOOP

MARK J
LINK 800
GRAB 220
SEEK 9999
SEEK -3
COPY F X
SEEK 1
COPY X F

MARK END
```

## DRIVING_TEST

**Level:** Motor Vehicle Administration

**Solution:**

```
LINK 800
LINK 799
@REP 6
LINK 800
@END
LINK 801
LINK -1
LINK 800
LINK -1
```

