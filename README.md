# EXP 6 : SPEECH RECOGNITION USING SCILAB

## AIM: 

To perform and verify multirate DSP without function using SCILAB.

## APPARATUS REQUIRED: 
PC installed with SCILAB. 

## PROGRAM : 
```
clc;
close;
n = 0:%pi/50:2*%pi;
x = sin(%pi*n); 

M=input('Enter the downsampling factor');
L=input('Enter the upsampling factor');

downsampling_x = x(1:M:length(x));
disp(x,'Input signal x(n)=');
disp(downsampling_x,'Downsampled Signal');
figure(1);
subplot(2,1,1)
plot2d3(1:length(x),x);
xtitle('original singal')
subplot(2,1,2)
plot2d3(1:length(downsampling_x),downsampling_x);
xtitle('Downsampled Signal by a factor of M');


upsampling_x=[];
for i=1:length(x)
upsampling_x(1,L*i)=x(i);
end
disp(x,'Input signal x(n)=');
disp(upsampling_x,'Upsampled Signal');
figure(2);
subplot(2,1,1);
plot2d3(x);
title('original signal');
subplot(2,1,2);
plot2d3(upsampling_x);
title('Upsampled Signal by a factor of L');
```


## OUTPUT: 
<img width="1918" height="1193" alt="image" src="https://github.com/user-attachments/assets/d8d5a081-57e3-4926-832b-21385999d456" />
<img width="1918" height="1197" alt="image" src="https://github.com/user-attachments/assets/64e6e11b-ef2a-4864-9d2a-65e6c6e62a8e" />


## RESULT: 
Thus the decimation process by a factor M and interpolation process by a factor L using SCILAB was implemented.
Thus the decimation process by a factor M and interpolation process by a factor L using 
SCILAB was implemented. 
