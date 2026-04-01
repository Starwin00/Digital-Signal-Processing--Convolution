# Digital-Signal-Processing--Convolution
## Aim:
                  To perform linear convolution using MAT LAB.
## Software Required:
MAT LAB R2012
## Algorithm:
Step 1: Open mat lab. Write the program.

Step 2: Read the first input sequence.

Step 3: Read the second impulse sequence.

Step 4: Plot the input sequences with x-label and y-label with suitable title. 

Step 5: Perform convolution for both the sequences using conv2() function.
  
Step 6: Plot the sequence with x-label and y-label with suitable title

Step 7: Terminate the program.

## PROGRAM: 
```
clc; % clear screen
%clear all; % clear screen
close all; % close all figure windows

% input sequence
% X[n]={2,3,-5.2,1.4,-2.6,3.8,4} h[n]={3.2,4.1,5,-6.4,2.1,3.9};

a = input("enter the starting x(n)");
x = input("enter the x(n) sequence");
n = a:1:length(x)+a-1;
figure(1);
stem(n,x);
xlabel('time');
ylabel('amplitude');
title('input sequence');

%impulse sequence

b= input('enter the starting h(n)');
y = input('enter the h(n) sequence');
m = b:1:length(y)+b-1;
figure(2);
stem(m,y);
xlabel('time');
ylabel('amplitude');
title('impulse response');

%linear convolution

z = conv2(x,y);
n1 = a+b:1:length(z)+a+b-1;
figure(3);
stem(n1,z);
xlabel('time');
ylabel('amplitude');
title('linear convolution');
```

## OUTPUT:
### Input Sequence:

<img width="701" height="529" alt="image" src="https://github.com/user-attachments/assets/65ae987a-44d0-4ce5-b419-85cd1dd5db5e" />

### Impulse Sequence:

<img width="693" height="527" alt="image" src="https://github.com/user-attachments/assets/68854fe2-a998-4375-9058-cecc58123aab" />

### Linear Convolution:

<img width="700" height="525" alt="image" src="https://github.com/user-attachments/assets/5b0a5747-ca72-47f2-9a11-d2ad56e0d254" />



## RESULT:

![WhatsApp Image 2026-03-28 at 11 26 56 AM (2)](https://github.com/user-attachments/assets/39750aeb-54c8-45ed-bc4b-f0539e35c8b2)

