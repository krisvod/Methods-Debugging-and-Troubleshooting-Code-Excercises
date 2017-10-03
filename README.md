# Methods-Debugging-and-Troubleshooting-Code-Excercises

1 - 
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApplication4
{
    class Program
    {
        static void Main(string[] args)
        {
            string name = Console.ReadLine();
            OutputName(name);
        }
        static void OutputName(string name)
        {
            Console.WriteLine("Hello, {0}!", name);
        }
    }
}

2 -
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApplication4
{
    class Program
    {
        static void Main(string[] args)
        {
            int a = int.Parse(Console.ReadLine());
            int b = int.Parse(Console.ReadLine());
            int d = GetMax(a, b);
            GetMax(a, b);
            int c = int.Parse(Console.ReadLine());
            if (c > d)
                Console.WriteLine(c);
            else if (d > c)
                Console.WriteLine(d);
        }
        static int GetMax(int a, int b)
        {
            if (a > b)
                return a;
            else
                return b;
        }
    }
}

3 -
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApplication4
{
    class Program
    {
        static void Main(string[] args)
        {
            int a = int.Parse(Console.ReadLine());
            int word = GetNum(a);
            if (word == 0)
                Console.WriteLine("zero");
            else if (word == 1)
                Console.WriteLine("one");
            else if (word == 2)
                Console.WriteLine("two");
            else if (word == 3)
                Console.WriteLine("three");
            else if (word == 4)
                Console.WriteLine("four");
            else if (word == 5)
                Console.WriteLine("five");
            else if (word == 6)
                Console.WriteLine("six");
            else if (word == 7)
                Console.WriteLine("seven");
            else if (word == 8)
                Console.WriteLine("eight");
            else if (word == 9)
                Console.WriteLine("nine");
        }
        static int GetNum(int a)
        {
            a = a % 10;
            return a;
        }
    }
}

4 -

5 -
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApplication4
{
    class Program
    {
        static void Main(string[] args)
        {
            int num = int.Parse(Console.ReadLine());
            Console.WriteLine(Fib(num));
        }
        static int Fib(int n)
        {
            int a = 0;
            int b = 1;
            for (int i = 1; i <= n; i++)
            {
                int temp = a;
                a = b;
                b = temp + b;
            }
            return b;
        }
    }
}

6 -
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApplication4
{
    class Program
    {
        static void Main(string[] args)
        {
            int num = int.Parse(Console.ReadLine());
            Console.WriteLine(IsPrime(num));
        }
        static bool IsPrime(int n)
        {
            for (int i = 2; i < n; i++)
            {
                if (n % i == 0)
                    return false;
            }
            return true;
        }
    }
}

7 - 
