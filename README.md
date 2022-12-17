# Single-level-Ex3-4

/*
 class A{

    static void m1(){
        System.out.println("Hii From Class A");
    }
    
}   

public class B extends A {
    
    static void m1() {
        System.out.println("Hii From Class B");
      A.m1();
      A a1=new A();
      a1.m1();
    }
    public static void main (String args[]){
        A a1=new A();
        a1.m1();
        System.out.println("Hii From Main");
    }

}
*/

 class A{
    int x;
    
    A(){
        x=5;
         System.out.println("Hii From Default Constructor A");
    }
    A(int x1)
    {
        x=x1;
    }
    
}   

public class B extends A {
    int y;
    B()
    {
        super();
        y=x;
    }
    B(int x ,int y )
    {
        super(x);
        this.y=y;
    }
    public static void main (String args[]){
        A a1=new A();
        B b1=new B();
        B b2=new B(6,7);
        System.out.println(b2.x+"  "+b2.y);
    }

}
