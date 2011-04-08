Static analyzer for Diffusion Equation
========================

1. Compilation
--------------

1.1. *nix:

	g++ -o dists/out base/Exception.cpp main.cpp models/Analyzer.cpp models/Coloring.cpp models/Diff.cpp

1.2. Windows:

	g++ -o dists\out.exe base\ExceptionWin.cpp main.cpp models\Analyzer.cpp models\ColoringWin.cpp models\Diff.cpp

1.3. Windows (libs build in):

	g++ -static-libstdc++ -static-libgcc -o dists\out.exe base\ExceptionWin.cpp main.cpp models\Analyzer.cpp models\ColoringWin.cpp models\Diff.cpp

1.4. Arm (libs build in):
     See this http://android-dls.com/wiki/index.php?title=Compiling_for_Android

	arm-linux-gnueabi-g++ -static-libgcc -o dists/out_arm base/Exception.cpp main.cpp models/Analyzer.cpp models/Coloring.cpp models/Diff.cpp

	or

	arm-linux-gnueabi-g++ -static -o dists/out_arm base/Exception.cpp main.cpp models/Analyzer.cpp models/Coloring.cpp models/Diff.cpp


Difference between 1.2 and 1.3 is: 1.2 - worked only on windows, where installed MinGW, and 1.3 worked on any compatible windows system (libraries build in binary file)

The binary file is in "out"


2. Debug
--------------
	2.1. File "main.h"
		All after text "// debug moments"
\\ 2. Debug

3. E.t.c.
--------------
	3.1 Model Diff is not realy need in this project (write it firstly - and then don`t wont delete)
