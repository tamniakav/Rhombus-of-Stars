using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Rhombus_of_Stars
{
    class Program
    {
        static void Main(string[] args)
        {
            int n = int.Parse(Console.ReadLine());

            string stars = "* ";
            for (int row = 1; row <= n; row++)
            {
                Console.Write(new string(' ', n - row));
                for (int i = 0; i < row; i++)
                {
                    Console.Write("{0}", (stars));
                }
                Console.WriteLine();
            }

            for (int row = n - 1; row >= 1; row--)
            {
                Console.Write(new string(' ', n - row));
                for (int j = 0; j < row; j++)
                {
                    Console.Write("{0}", (stars));
                }
                Console.WriteLine();
            }
        }
    }
}
