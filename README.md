# Digital-Signal-Processing--Correlation
## AIM:
To generate discrete auto correlation and cross correlation of signals using MATLAB.
## APPARATUS REQUIRED:
MATLAB R2012.
## ALGORITHM:
Step 1: Open matlab. Write the program.

Step 2: Read the input sequence 1 and input sequence 2 sequence.

Step 3: Perform auto correlation and cross correlation for both the sequences. 

Step 4: Plot the output sequence with x-label and y-label with suitable title.

Step 5: Terminate the program.


## PROGRAM: 
```
clc; % clear screen
clear all; % clear screen
close all; % close all figure windows
% INPUT SIGNAL-1
a=input('enter the starting x(n)');
x=input('Enter the x(n) sequence');
n=a:1:length(x)+a-1;
figure(1)
stem(n,x)
xlabel('Time')
ylabel('Amplitude')
title('Input Signal-1')
% INPUT SIGNAL 2
b=input('enter the starting y(n)');
y=input('Enter the y(n) sequence');
m=input('enter the ending y(n)');
n1=b:1:length(y)+b-1;
figure(2)
stem(n1,y)
xlabel('time')
ylabel('amplitude')
title('input signal-2')
%discrete auto correlated signal 
out1=xcorr(x,x)
n2=a-m:1:length(out1)+a-m-1;
figure(3)
stem(n2,out1)
xlabel('time')
ylabel('amplitude')
title('discrete auto correlated waveform')
%discrete cross correlated signal
out2=xcorr(x,y)
n3=a-m:1:length(out2)+a-m-1;
figure(4)
stem(n3,out2)
xlabel('time')
ylabel('amplitude')
title('discrete cross correlated waveform')
```

## OUTPUT:

![WhatsApp Image 2026-03-29 at 9 06 35 AM (1)](https://github.com/user-attachments/assets/5d020a9e-8e0a-41da-813a-9eeea44cb620)

![WhatsApp Image 2026-03-29 at 9 06 36 AM](https://github.com/user-attachments/assets/ca529b79-8a5b-4596-8edc-57651a4fd8d1)

![WhatsApp Image 2026-03-29 at 9 06 36 AM (1)](https://github.com/user-attachments/assets/d94e5cad-321e-4021-9c68-d736e1059faf)

![WhatsApp Image 2026-03-29 at 9 06 35 AM](https://github.com/user-attachments/assets/e8c6002e-04cf-41c2-9642-ed7eab7a7eca)


## RESULT:

