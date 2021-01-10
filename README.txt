Author: Dimitrios Kanoulas (d.kanoulas@ucl.ac.uk)
Description: This package implements some sample code for COMP0129-S21:
1. rocore testing
2. Talker-Listener implementation
3. Server-Client (add two numbers) implementation
4. Static TF publishing
-------------------------------------------------------------------------------


===============================================================================
Question 1
===============================================================================
Compilation
---------------------------------------
No need to compile anything

-------------------------------------------------------------------------------

Execution
---------------------------------------
Terminal 1:
> roscore

Terminal 2:
> rostopic list


===============================================================================
Question 2
===============================================================================

Compilation
---------------------------------------
Terminal 1:
> cd sample
> catkin_make -DCMAKE_BUILD_TYPE=Release


Execution
---------------------------------------
Terminal 1:
> roscore

Terminal 2:
> cd sample
> source devel/setup.bash
> rosrun sample sample_talker

Terminal 3:
> cd sample
> source devel/setup.bash
> rosrun sample sample_listener


===============================================================================
Question 3
===============================================================================
Compilation:
---------------------------------------
Terminal 1:
> cd sample
> catkin_make -DCMAKE_BUILD_TYPE=Release


Execution
---------------------------------------
Terminal 1:
> roscore

Terminal 2:
> cd Lab1
> source devel/setup.bash
> rosrun sample sample_server
> rosrun sample sample_client 1 2


===============================================================================
Question 4
===============================================================================
Compilation:
---------------------------------------
Terminal 1:
> cd sample
> catkin_make -DCMAKE_BUILD_TYPE=Release


Execution
---------------------------------------
> roslaunch sample sample.launch


LICENSE: GPL.  See LICENSE.txt

DISCLAIMER:

THIS INFORMATION AND/OR SOFTWARE IS PROVIDED BY THE AUTHOR "AS IS" AND ANY
EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
DISCLAIMED. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY DIRECT, INDIRECT,
INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR
PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS INFORMATION AND/OR
SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.

Copyright (C) 2021 Dimitrios Kanoulas except where specified

