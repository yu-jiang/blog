---
title: "Matlab Coder Tutorial"
date: 2022-01-12T23:16:05-05:00
draft: true
toc: false
images:
tags:
  - untagged
---

Hello, friends

Today I wanted to give a quick tutorial on matlab coder.

As prerequists, I will be using MATLAB R2021a. The compiler I have is Miscrosft Visual C++ 2017 (c). To check your compiler installation, run
```
>> mex -setup
```
If you don't have a compiler, please refer to [this page](https://www.mathworks.com/support/requirements/supported-compilers.html)


First, let's find a matlab function based off which we would like to generate C/C++ code. The one I pick is the function [```img2txt```](https://www.mathworks.com/matlabcentral/fileexchange/4732-ascii-text-image-generator), which converts an image to a matrix of ASCII code.

I have also prepared this sample picture ```Doraemon_2005.png``` ![Doraemon](/img/Doraemon_2005.png)

If we run the function in MATLAB
```
>> img2txt(`Doraemon_2005·png`）
```

It will then create a txt file ```Doraemon_2005.png.txt``` in the same folder. Opening the file and zoom out, we will see
![doraemon_ascii](/img/Doraemon_2005_txt.png)

Now, we wanted to operate this outside of MATLAB. For that, we are going to generate an executable.

To start, let us open the MATLAB Coder UI
```
>> coder
```
In the GUI, enter the name of the entry point function and hit the enter button. Then, hit next.
![step1](/img/coder_demo_step_1.png)

In the new view, give MATLAB a runnable example of how to run the function
![step1](/img/coder_demo_step_2.png)
to help the UI automatically determine the datatype of the inputs. Manually change the length of the first argument from 17 to Inf.



