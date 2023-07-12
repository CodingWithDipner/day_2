# day_2

Today in class i learned the Strobogrammatic Number.
# 
What is Strobogrammatic  number?
if the number equal to rotation of 180 degree number, then it is called as Strobogrammatic  number

Who is the author?
There is no specific author

What is the iteration condition?
0 to length of the number.

#
Strobogrammatic  Number and its value from 0 to 9

0=0

1=1


6=9

8=8

9=6


#

Algorithm steps


Ø User input ( Number value but string datatype)

Ø Create empty string initially

Ø Assign the Strobogrammatic  number with its value up to 9

Ø Checking empty string is equal to original string


#
Step 1-User input ( Number value but string datatype)


    Scanner sc= new Scanner(System.in);

    System.out.println("Enter the number");

    String num=sc.next();


Step  2-Create empty string


    String s1="";


Step 3- Assign the Strobogrammatic  number with its value up to 9



        for(int i=0;i<num.length();i++)
        {
            char c=num.charAt(i);
            if(c=='0') s1='0'+s1;
            else if(c=='1') s1='1'+s1;
            else if(c=='6') s1='9'+s1;
            else if(c=='8') s1='8'+s1;
            else if(c=='9') s1='6'+s1;
        }

Step 4 - Checking empty string is equal to original String 
        
        if(s1.equals(num))
        {
          System.out.println("Yes");
        }
        else
        {
            System.out.println("No");
        }



        
