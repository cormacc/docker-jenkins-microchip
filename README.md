# jenkins-microchip #

This extends the jenkins LTS docker image to facilitate cross-compilation using Microchip XC16.

It installs _gcc-multilib_, the latest version of the Microchip XC16 compiler and ruby with the _rake_ and _ceedling_ gems for TDD (see http://throwtheswitch.org for more info on C TDD).

Command sequence for download and unattended installation of XC16 stolen shamelessly from https://github.com/mmitchel/docker-xc16 - thanks mmitchel!

This image should allow unit tests to be run natively using 64-bit and 32-bit gcc as well as cross-compiled using xc16 and run on the microchip simulator.
For further information on Microchip cross-compilation, see here: https://github.com/ThrowTheSwitch/CeedlingExample_Microchip
