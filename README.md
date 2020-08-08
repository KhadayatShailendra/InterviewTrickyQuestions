# C# Interview Tricky Questions

### 1. What is the output?

    int[] arr = new int[0];
    Console.WriteLine(arr[0]);

### 2. What is the output?
    byte b = 100;
    Console.WriteLine(b.GetType());
    b += 255;
    Console.WriteLine(b.GetType());
    b += 256;
    Console.WriteLine(b.GetType());

### 3. What will be printed in console?
    using System;
    class Program
    {
        static void Main() {
            DerivedClass d = new DerivedClass();
            d.i = 2;
            d.Print();
        }

        public abstract class BaseClass{
            public int i = 0;
            public int j = 0;
            public abstract void Print();
        }

        public class DerivedClass: BaseClass{
            new int j = 1;
            public override void Print(){
                this.j = 3;
                Console.WriteLine("i= {0} and j= {1}", i, this.j);
            }
        }
    }
