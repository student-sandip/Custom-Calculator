import java.util.Scanner;

class InvalidInputException extends Exception{
    
    @Override
    public String toString() {
        return "Can't add number 8 & number 9...";
    }

    @Override
    public String getMessage() {
        return " ";
    }
}

class Cannotsubtraction extends Exception{
    
    @Override
    public String toString() {
        return "Can't suubtract...";
    }
    @Override
    public String getMessage() {
        return  " ";
    }
}

class Notmultiply extends Exception{
    
    @Override
    public String toString() {
        return "Can't multiiply by 0 and 1...";
    }
    @Override
    public String getMessage() {
        return  " ";
    }
}

class CannotDivideByZero extends Exception{
    
    @Override
    public String toString() {
        return "Can't divide by 0...";
    }
    @Override
    public String getMessage() {
        return  " ";
    }
}


class  Maxvaluereached extends Exception{
    
    @Override
    public String toString() {
        return "Input can't be greater than 100000..";
    }
    @Override
    public String getMessage() {
        return  " ";
    }
}

class  Maxmultiplyvaluereached extends Exception{
    
    @Override
    public String toString() {
        return "Input can't be greater than 7000.";
    }
    @Override
    public String getMessage() {
        return  " ";
    }
}

class calculator  {
    double add (double a, double b) throws InvalidInputException, Maxvaluereached {
        if (a>100000 || b>100000) {
            throw new Maxvaluereached();
        }
        if (a==9 && b==8) {
            throw new InvalidInputException();
        }
        return a + b;
    }
    double subtract (double a, double b) throws Cannotsubtraction, Maxvaluereached{
        if (a>100000 || b>100000) {
            throw new Maxvaluereached();
        }
        if (a==0 ||  b==0) {
            throw new Cannotsubtraction();
        }
        return(a-b);
    }
    double multi (double a, double b) throws Notmultiply, Maxmultiplyvaluereached{
        if (a>7000 && b>7000) {
            throw new Maxmultiplyvaluereached();
        }
        if (a==0 && b ==0) {
            throw new Notmultiply();
        }
        return(a*b);
    }
    double div (double a, double b) throws CannotDivideByZero,Maxvaluereached{
        if (a>100000 && b>100000) {
            throw new Maxvaluereached();
        }
        if (b==0){
            throw new CannotDivideByZero();
        }
        return(a/b);
    }
}

public class Ex_6_customcalculator_87 {
    public static void main(String[] args) throws InvalidInputException, Cannotsubtraction, Notmultiply, CannotDivideByZero, Maxvaluereached, Maxmultiplyvaluereached {
        Scanner sc = new Scanner(System.in);
        System.out.println("Enter the 1at number: ");
        double num1=sc.nextDouble();
        System.out.println("Enter the second number:");
        double num2=sc.nextDouble();
        calculator c = new calculator();

        try {
            // System.out.println("It is not possiable to add 9 and 8 at same time.");
            System.out.println("The sum of "+num1+" and " +num2+ " is :" +c.add(num1, num2));
            }
            catch(InvalidInputException e) {
                System.out.print("The error is: "+e);
            }

        try {
            // System.out.println("it is not possible to divide by zero.");
            System.out.println("The division of "+num1+" and "+num2+" is:"+c.div(num1, num2));
        }
        catch(CannotDivideByZero e){
            System.out.println("The error is: "+e);
        }

        try {
            // System.out.println("Multiplication is not allowed for Zero.");
            System.out.println("The multiplication of "+num1+" and "+num2+" is :"+c.multi(num1, num2));
        }
        catch(Notmultiply e){
            System.out.println("The error is: "+e);
        }
        // try-catch marged  ----->   Exception handling 
        // System.out.println("subtraction does't exists for Zero..");
        System.out.println("The subtraction of "+num1+" and "+num2+" is :"+c.multi(num1, num2));

        c.add(num1, num2);
        c.div(num1, num2);
        c.subtract(num1, num2);
        c.multi(num1, num2);
    }
}




    // without try-catch block --> Runtime exception handling   ---> 
    /* 
        System.out.println("Addition: "+c.add(num1,num2));    // <-- throw an exception if put  '9' and '8' as input for
        System.out.println("subtraction: "+c.subtract(num1,num2)); //  <-- throw an exception if put both value 0;
        System.out.println("Multiplication: "+c.multi(num1,num2));   // <-- throw an exception if put both value 0;
        System.out.println("Division: "+c.div(num1,num2));     // <-- throw an exception if put both value 0;
    */

    //     }
    // }
    //                                      finish.
