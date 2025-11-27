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
n1=b: 1:length(y)+b-1;
figure(2)
stem(n1,y)
xlabel('Time')
ylabel('Amplitude')
title('Input signal-2')

% DISCRETE AUTO CORRELATED SIGNAL
out1=xcorr(x,x)
n2=a-m:1:length(out1)+a-m-1;
figure(3)
stem(n2,out1)
xlabel('Time')
ylabel('Amplitude')
title(' Discrete auto correlated waveform')

% DISCRETE CROSS CORRELATED SIGNAL
Out2=xcorr(x,y);
n3=a-m:1:length(Out2)+a-m-1;
figure(4)
stem(n3,Out2)
xlabel('Time')
ylabel('Amplitude')
title(' Discrete cross correlated waveform')
```
## Calculation:
![d365c15f-602a-4701-8bde-c9503e802df1](https://github.com/user-attachments/assets/b899bb5a-13ff-48d3-980d-b98319a5bee3)



## OUTPUT:
X1[n] ={2.3,3.2,-4.1,5.3,1.7,-2.9} X2[n]={3,4,-1.5,2,2.7,3.5,2}
<img width="1920" height="1080" alt="Screenshot 2025-10-09 150009" src="https://github.com/user-attachments/assets/57e57ffe-6b9a-478c-baee-6471f5837d6f" />

## RESULT:
![17bcc0b5-50c7-4c08-a3dd-d23c8055a0df](https://github.com/user-attachments/assets/8761abce-0b36-437c-a2f7-5366636961d5)




