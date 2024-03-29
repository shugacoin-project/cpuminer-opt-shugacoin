This file is included in the Windows binary package. Compile instructions
for Linux and Windows can be found in RELEASE_NOTES.

cpuminer is a console program that is executed from a DOS command prompt.
There is no GUI and no mouse support.

Miner programs are often flagged as malware by antivirus programs. This is
a false positive, they are flagged simply because they are cryptocurrency 
miners. The source code is open for anyone to inspect. If you don't trust
the software, don't use it.

Choose the exe that best matches you CPU's features or use trial and
error to find the fastest one that doesn't crash. Pay attention to
the features listed at cpuminer startup to ensure you are mining at
optimum speed using all the available features.

Architecture names and compile options used are only provided for Intel
Core series. Pentium and Celeron often have fewer features.

AMD CPUs older than Piledriver, including Athlon x2 and Phenom II x4, are not
supported by cpuminer-opt due to an incompatible implementation of SSE2 on
these CPUs. Some algos may crash the miner with an invalid instruction.
Users are recommended to use an unoptimized miner such as cpuminer-multi.
Changes in v3.8.4 may have improved compatibility with some of these CPUs.


Exe name                Compile flags            Arch name

cpuminer-sse2.exe      "-msse2"                  Core2, Nehalem   
cpuminer-aes-sse42.exe "-march=westmere"         Westmere, Sandy-Ivybridge
cpuminer-avx.exe       "-march=corei7-avx"       Sandy-Ivybridge
cpuminer-avx2.exe      "-march=core-avx2"        Haswell, Sky-Kaby-Coffeelake
cpuminer-avx2-sha.exe  "-march=core-avx2 -msha"  Ryzen

If you like this software feel free to donate:

 BTC: bc1qha3e7mzckctq0ejh3z5gvzes8jftj04j96gjfl (dev)  
 SHUGA: shuga1q8mpwgsk0zjr30a7xxhftt7wn9scsav9cpsdwgl (dev)  
