# SIMULATION-OF-MEAN-AND-VARIANCE-USING-SCILAB

# AIM:

To write a program for mean, variance and cross correlation in SCILAB and verify the output.

# EQUIPMENTS Needed:

• Computer with i3 Processor

• SCI LAB

# Algorithm:

1.Define the Function: Specify the function you want to simulate. For example, f(x)=sin⁡(x)f(x) = \sin(x)f(x)=sin(x) or any other function.

2.Generate Sample Points: Decide on the range and the number of sample points. Generate these sample points within the desired range.

3.Evaluate the Function: Compute the function values at each of these sample points.

4.Compute Mean, Variance and Cross Correlation: Use Scilab's functions to calculate the mean and variance of the computed function values.

5.Display Results: Output the computed mean variance and Cross Correlation 

# PROCEDURE:
• Refer Algorithms and write code for the experiment.

• Open SCILAB in System

• Type your code in New Editor

• Save the file

• Execute the code 

• If any Error, correct it in code and execute again

• Verify the generated results

# PROGRAM:
```
function X=f(x)
   z=7*(2+x)^2;
   X=x*z
endfunction
a=0;
b=1;
EX=intg(a,b,f);
function Y=c(y)
  z=7*(2+y)^2;
  Y=y*z;
endfunction
EY=intg(a,b,c); 
disp(EX,"i)Mean of X =");
disp(EY,"Mean of Y =");


function X=g(x)
    z=7*(2+x)^2;
    X=x^2*z
endfunction
a=0;
b=1;
EX2=intg(a,b,g);
function Y=h(y)
    z=7*(2+y)^2;
    Y=y^2*z;
endfunction
EY2=intg(a,b,h);
vX2=EX2-(EX)^2;
vY2=EY2-(EY)^2;
disp(vX2,"ii)Variance of X");
disp(vY2," Variance of Y");


x= input("type in the reference sequence=");
y= input("type in the second sequence="); 
n1=max(size(y))-1;
n2=max(size(x))-1;
r=corr(x,y,n1);
plot2d3('gnn',r);

```

# CALCULATION:
![WhatsApp Image 2025-11-04 at 22 35 45_e27a496b](https://github.com/user-attachments/assets/3e1b1d98-de13-419b-9661-62e0191782f2)
![WhatsApp Image 2025-11-04 at 22 35 45_aca48e94](https://github.com/user-attachments/assets/df5aa77b-3873-494c-ab44-55e8d6436c25)
![WhatsApp Image 2025-11-04 at 22 35 46_801c58d7](https://github.com/user-attachments/assets/9da6a33c-4808-4ec0-beeb-00b2b74eef9e)


# OUTPUT:

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/9a23e2d6-b6fb-48f7-b0e3-bacf8b2be30b" />


# RESULT:

Thus the mean , variance and cross correlation are executed in Scilab and output is verified.
