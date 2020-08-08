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
