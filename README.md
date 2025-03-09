# CSA
AP Computer Science A studying project:
goal: somehow implement daily lessons? (resizable windows??)
      have a mini terminal that users can interact with?


Unit 1
  1.1
    Java is a class based (& object oriented) language.
    Have to declare a class when we write a program.
    Class names must match file names.
    Main method: public static void main(String[] args) {..} controls everything
  
  System.out.print("..") displays content to console, prints & cursor blinks
  System.out.println("..") prints a line and cursor jumps to next line
  
  For output to appear on console, use system class

  1.12
    A string literal is the exact sequence of characters (numbers, symbols) in double quotes
    ex ("A")

  1.13
    Error types:
      > Syntax/compiler error: identified when the program is compiled (some IDES
        will recognize - programs will not compile while syntax errors are present.
      > Exception: occur while the program is running andwill cause the program to
        terminate abnormally (throws an exception)
      > Logic errors: usually detected after a program has been run when actual output
        is compared to anticipated.
  
  1.21
    Primitive data determines size and type of information (booleans as true/false,
    ints as whole #s)
    other than String, additional types can be created for non-primitive types
    Only non-primitive types can use methods to perform actions.

  1.22
    Variable is a name given to a memory location holding specified type of value
    Variables are case sensitive & cannot start with a digit. Can consist of letters,
    digits or underscore but no spaces. Use camelCase.
    format to declare variable type, ex.
    dataType variableName;
    int total;
    to declare a variable we want to stay constant after we initalize, use "final"
    final int DAYS_IN_WEEK;

  1.31
    Operations result in same or bigger data type: int + int = int, int * double = double
    A literal (not a string literal) is the source code representation of a fixed value:
    "3" + "3" != 3+3
  
  1.32
    Compound expression = more complex arithmetic expressions
    operation precedence same as PEMDAS (% same as * )
    Can input variables into operators, first declare & plug in, ex.
    System.out.println(8*6-x);
    & dividing by 0 would throw an exception

  1.33
    Assign value on right of assignment operator to the variable on the left, ex.
    y = 8+4*x;
    & not
    7 = x
    because 7 already has a literal value
    assignment operator is last in operator precedence : takes calculated value
    can assign multiple operators in same line


  1.41
    Compound assignment operators (+=) ex.
    x += 7
    instruct to compiler: first take value stored as x, add 7 & assign new value to x
    same as
    x = x+7

  1.42
    ++ increment & -- decrement operators
    must be attached to a variable
    x++;
    adds 1 to current value stored in x and assigns result back to x
      only postfix on AP: position of ++ affects when increment take place


  1.43
    practice describing/tracing code

1.51
  casting can temporarily change a data type's variable
  ex. System.out.println((double) 6/4);
  or using a casting operator of double will give us a decimal answer
  Can use to round by casting ints

1.52
  Data types are limited in how much info they can store
  max integer = -10 integers, which causes an overflow error

2.1
  A class is a blueprint for creating objects with the same behavior
  An object is a specific entity made from a class that can be manipulated
  an object is an instance of classes with variables used to name them
  Each object has behaviors and attributes defined by the class used to create it.

2.2
  Constructors are used to initalize the attributes for an object
  They always start with public and have the same name as the class
  public Person(String..
    is called the signature, which contains the name of the constructor
    and the parameter list that initalizes those values
    The formal parameters take place within the parantheses, ex.
    Person(string nm, int ag, boolean ad)
    referring to String nm, int ag.
    The call by value are the objects you are passing to your call
    (when passing the values "Bryce", 17, & false
    copies are sent to the constructor and stored into the instance variables
    Actual parameters refer to the defined values that are going to be initalized
    as attributes with your constructor
    You can have more than one constructor for an object, which is known as overloading
    the constructor. A no-argument/default parameter will set the instance variables
    for that object to the default values for the given data type.
    the constructors

2.31
