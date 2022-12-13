# Matrix-Vector-Multipliction-Benchmark
This repository will showcase a space(Memory Usage) and time complexity benchmark of a matrix multiplication.
# Run
and before running the code make sure to do this first
```
make clear
```
this code is just to make sure that the extra .o files inside the folder is "Clear" so that you can follow this tutorial smoothly.

After that, run this code. as this code will basically create a main.o, main.out, utils.o file
```
make main
```
and after running the code above you will now be able to run this on the terminal
```
./main.out
```
The program will generate random integers with the given matrix size and the results will look similiarly like this(although it is random, but it should look as shown below).
```
M=[
2,      4,      4,
2,      2,      1,
1,      1,      1,      ]
v=[
3,
3,
1,      ]
b=[
22,
13,
7,      ]
```
# Time complexity Benchmark
From the looks of it these codes will describe the amount of time it takes for the machine to run the code.
To see the time complexity benchmark, do this first
```
make time
./time.out
```
it will ask for the user to input a number
```
Input N:
```
It will generate random integers and run from the matrix size of N to N*100. Furhtermore it ill add increment of N after the program finishes calculatin gthe previous size.

And then the program will create a file on the folder to show the results of each N called "timelist.dat"(results may be varied.)

If N = 10:
```
(10,0.000001),(20,0.000001),(30,0.000002),(40,0.000003),(50,0.000005),(60,0.000007),(70,0.000011),(80,0.000015),(90,0.000024),(100,0.000026),(110,0.000033),(120,0.000030),(130,0.000035),(140,0.000041),(150,0.000050),(160,0.000057),(170,0.000064),(180,0.000072),(190,0.000101),(200,0.000096),(210,0.000107),(220,0.000117),(230,0.000128),(240,0.000139),(250,0.000151),(260,0.000145),(270,0.000153),(280,0.000164),(290,0.000176),(300,0.000188),(310,0.000201),(320,0.000215),(330,0.000227),(340,0.000242),(350,0.000257),(360,0.000272),(370,0.000287),(380,0.000311),(390,0.000356),(400,0.000337),(410,0.000353),(420,0.000372),(430,0.000391),(440,0.000409),(450,0.000428),(460,0.000449),(470,0.000471),(480,0.000491),(490,0.000514),(500,0.000535),(510,0.000553),(520,0.000577),(530,0.000602),(540,0.000625),(550,0.000659),(560,0.000708),(570,0.000694),(580,0.000734),(590,0.000741),(600,0.000768),(610,0.000808),(620,0.000819),(630,0.000845),(640,0.000871),(650,0.000909),(660,0.000927),(670,0.000955),(680,0.000991),(690,0.001026),(700,0.001042),(710,0.001082),(720,0.001137),(730,0.001136),(740,0.001165),(750,0.001203),(760,0.001090),(770,0.001139),(780,0.001183),(790,0.001184),(800,0.001220),(810,0.001268),(820,0.001285),(830,0.001320),(840,0.001355),(850,0.001439),(860,0.001459),(870,0.001465),(880,0.001501),(890,0.001573),(900,0.001586),(910,0.001623),(920,0.001694),(930,0.001708),(940,0.001791),(950,0.001797),(960,0.001823),(970,0.001864),(980,0.001960),(990,0.001950),(1000,0.002012),
```

If N = 100
```
(100,0.000028),(200,0.000085),(300,0.000189),(400,0.000364),(500,0.000683),(600,0.000763),(700,0.001082),(800,0.001728),(900,0.001723),(1000,0.002267),(1100,0.003412),(1200,0.003434),(1300,0.003511),(1400,0.003874),(1500,0.004240),(1600,0.004938),(1700,0.005468),(1800,0.006083),(1900,0.006859),(2000,0.007618),(2100,0.008537),(2200,0.009617),(2300,0.009938),(2400,0.010893),(2500,0.011772),(2600,0.012712),(2700,0.013647),(2800,0.014722),(2900,0.015792),(3000,0.017040),(3100,0.018174),(3200,0.019445),(3300,0.021560),(3400,0.022949),(3500,0.024171),(3600,0.024571),(3700,0.026345),(3800,0.027741),(3900,0.028866),(4000,0.030868),(4100,0.032555),(4200,0.034142),(4300,0.034651),(4400,0.036999),(4500,0.038335),(4600,0.040503),(4700,0.043156),(4800,0.042975),(4900,0.044762),(5000,0.046879),(5100,0.048821),(5200,0.050766),(5300,0.052005),(5400,0.055038),(5500,0.070587),(5600,0.088769),(5700,0.086628),(5800,0.089681),(5900,0.093466),(6000,0.089137),(6100,0.069485),(6200,0.071665),(6300,0.074588),(6400,0.076608),(6500,0.080631),(6600,0.081330),(6700,0.084150),(6800,0.086385),(6900,0.089086),(7000,0.091325),(7100,0.094323),(7200,0.096818),(7300,0.099376),(7400,0.102118),(7500,0.104809),(7600,0.107912),(7700,0.112069),(7800,0.114958),(7900,0.117341),(8000,0.120423),(8100,0.123097),(8200,0.126072),(8300,0.129176),(8400,0.132227),(8500,0.136009),(8600,0.171191),(8700,0.179215),(8800,0.144053),(8900,0.147412),(9000,0.150532),(9100,0.154129),(9200,0.157552),(9300,0.161069),(9400,0.164972),(9500,0.169192),(9600,0.172545),(9700,0.178931),(9800,0.181137),(9900,0.185739),(10000,0.234539),
```
To put it simply, For N = 10 or 100,200,300,. . . it means the Matrix N size.
while the 0.000028, 0.000085 and 0.000189 mean how long the program will finish calculating the matrix.

# Space Complexity Benchmark
this will indicate the total space or memory taken by the algorithmn with respect to the input size.

And thus run these codes to be able to do the space complexity benchmark:
```
make space
./space.out
```
the Program will then ask the user
```
Input N:10
CTRL+C to interrupt the process 
```
to put it simply the N that is being inputted by the user is the size of matrix. the program will calculate the matrix vector non-stop until it's interrupted(which in this case it is done by pressing Ctrl + C on the keyboard.)

while the program is still running create another WSL Terminal and type this command.
```
ps Aux
```
The results may be varied, and this is what i got on my machine.
```
USER       PID %CPU %MEM    VSZ   RSS TTY      STAT START   TIME COMMAND
root         1  0.0  0.0   1884  1252 ?        Sl   12:19   0:00 /init
root        15  0.0  0.0   1972   168 ?        Ss   12:19   0:00 /init
root        16  0.0  0.0   1972   168 ?        S    12:19   0:00 /init
emirben     17  0.0  0.0   2884   952 pts/0    Ss+  12:19   0:00 sh -c "$VSCODE_WSL_EXT_LOCATION/scripts/wslServ
emirben     18  0.0  0.0   2884   960 pts/0    S+   12:19   0:00 sh /mnt/c/Users/Emir Ben/.vscode/extensions/ms-
emirben     23  0.0  0.0   2884   936 pts/0    S+   12:19   0:00 sh /home/emirben/.vscode-server/bin/5235c6bb189
emirben     27  0.3  1.3 947884 94032 pts/0    Rl+  12:19   0:15 /home/emirben/.vscode-server/bin/5235c6bb189b60
emirben     38  0.1  0.9 701236 64060 pts/0    Rl+  12:19   0:07 /home/emirben/.vscode-server/bin/5235c6bb189b60
root        47  0.0  0.0   1972   168 ?        Ss   12:19   0:00 /init
root        48  0.0  0.0   1972   168 ?        S    12:19   0:00 /init
emirben     49  0.0  0.6 589176 44252 pts/1    Ssl+ 12:19   0:01 /home/emirben/.vscode-server/bin/5235c6bb189b60
root        96  0.0  0.0   1972   168 ?        Ss   12:19   0:00 /init
root        97  0.0  0.0   1972   168 ?        S    12:19   0:00 /init
emirben     98  0.0  0.6 590604 48356 pts/2    Ssl+ 12:19   0:01 /home/emirben/.vscode-server/bin/5235c6bb189b60
emirben    105  0.0  0.6 966544 47904 pts/0    Sl+  12:19   0:01 /home/emirben/.vscode-server/bin/5235c6bb189b60
emirben    112  0.3  1.9 995720 135208 pts/0   Sl+  12:19   0:16 /home/emirben/.vscode-server/bin/5235c6bb189b60
emirben    183  0.0  0.5 2480608 41752 pts/0   Sl+  12:19   0:03 /home/emirben/.vscode-server/extensions/ms-vsco
emirben    230  0.0  0.0   6232  5204 pts/4    Ss   12:19   0:00 /usr/bin/bash --init-file /home/emirben/.vscode
emirben    419  0.0  0.2 5836028 20280 pts/0   Sl+  12:20   0:00 /home/emirben/.vscode-server/extensions/ms-vsco
emirben   1610  0.0  0.3 5836028 23160 pts/0   Sl+  12:42   0:00 /home/emirben/.vscode-server/extensions/ms-vsco
emirben   3379 90.8  0.0   2768  1108 pts/4    R+   13:31   0:12 ./space.out
emirben   3425  0.4  0.0   6232  5200 pts/3    Ss   13:31   0:00 /usr/bin/bash --init-file /home/emirben/.vscode
emirben   3477  0.0  0.0   7476  3148 pts/3    R+   13:31   0:00 ps aux
```
After that, you need to find the PID of space.out, and in here the ./space.out is 2153.

Then, you can use the pmap command on the terminal to find the memory usage.
```
pmap <pid>
#For Example
pmap 3379
```
And the Results(as usual it may varied)
if N = 10
```
3379:   ./space.out
0000560bc6b9a000      4K r---- space.out
0000560bc6b9b000      4K r-x-- space.out
0000560bc6b9c000      4K r---- space.out
0000560bc6b9d000      4K r---- space.out
0000560bc6b9e000      4K rw--- space.out
0000560bc76aa000    132K rw---   [ anon ]
00007f5af4d13000     12K rw---   [ anon ]
00007f5af4d16000    160K r---- libc.so.6
00007f5af4d3e000   1620K r-x-- libc.so.6
00007f5af4ed3000    352K r---- libc.so.6
00007f5af4f2b000     16K r---- libc.so.6
00007f5af4f2f000      8K rw--- libc.so.6
00007f5af4f31000     52K rw---   [ anon ]
00007f5af4f44000      8K rw---   [ anon ]
00007f5af4f46000      8K r---- ld-linux-x86-64.so.2
00007f5af4f48000    168K r-x-- ld-linux-x86-64.so.2
00007f5af4f72000     44K r---- ld-linux-x86-64.so.2
00007f5af4f7e000      8K r---- ld-linux-x86-64.so.2
00007f5af4f80000      8K rw--- ld-linux-x86-64.so.2
00007ffea0e42000    132K rw---   [ stack ]
00007ffea0f11000     16K r----   [ anon ]
00007ffea0f15000      4K r-x--   [ anon ]
 total             2768K
```
if N = 1000000(i tried n 100 but it has no difference whatsoever so i increased the zeros, machine specs matters!) 
```
3919:   ./space.out
000055e38faa0000      4K r---- space.out
000055e38faa1000      4K r-x-- space.out
000055e38faa2000      4K r---- space.out
000055e38faa3000      4K r---- space.out
000055e38faa4000      4K rw--- space.out
000055e391877000   7944K rw---   [ anon ]
00007f2bf1d30000     12K rw---   [ anon ]
00007f2bf1d33000    160K r---- libc.so.6
00007f2bf1d5b000   1620K r-x-- libc.so.6
00007f2bf1ef0000    352K r---- libc.so.6
00007f2bf1f48000     16K r---- libc.so.6
00007f2bf1f4c000      8K rw--- libc.so.6
00007f2bf1f4e000     52K rw---   [ anon ]
00007f2bf1f61000      8K rw---   [ anon ]
00007f2bf1f63000      8K r---- ld-linux-x86-64.so.2
00007f2bf1f65000    168K r-x-- ld-linux-x86-64.so.2
00007f2bf1f8f000     44K r---- ld-linux-x86-64.so.2
00007f2bf1f9b000      8K r---- ld-linux-x86-64.so.2
00007f2bf1f9d000      8K rw--- ld-linux-x86-64.so.2
00007fffd61b9000    132K rw---   [ stack ]
00007fffd61e4000     16K r----   [ anon ]
00007fffd61e8000      4K r-x--   [ anon ]
 total            10580K
```
the Total indicaes the memory usage of the program.

# GRAPHS!!!
This is The graph for the time complexity N = 10
<img width="866" alt="image" src="https://user-images.githubusercontent.com/114371873/207251547-f92065b2-fc83-4973-884d-bbc454b157c9.png">

And this is If N = 100
<img width="1198" alt="image" src="https://user-images.githubusercontent.com/114371873/207256775-cf926c63-3bac-46ee-8fc9-3006c4e460d3.png">

the X axis indicates the N(matrix Size of N) while the Y axis indicates the time in taken in seconds.

And finally this is the graph of the space complexity benchmark.
<img width="1280" alt="image" src="https://user-images.githubusercontent.com/114371873/207266256-89dd2e55-5c3c-406d-8a85-12227ba01618.png">

The y axis indicates the value of K in the program benchmark with the pmap <pip> one, the X axis indicates the size of Matrix N.
