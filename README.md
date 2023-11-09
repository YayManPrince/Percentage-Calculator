# Percentage-Calculator
c# percentage calculator
using System;
using System.Collections;
using System.Threading.Tasks;

namespace PerCalc {

    class PercentCalc
    {
        
        public static void Main(string[] args)
        {
            string pick = " ";
            Console.WriteLine("This is a percentage Calculate");

            
            Console.WriteLine("Would you like to (1) Calculate percentage or " +
                "(2) calculate the percentage of a number: ");
            string num = Console.ReadLine();
            

            if (num == "1")
            {
                Console.WriteLine("\nCalculate Percentage");
                Console.WriteLine("Enter number of parts: ");
                double a1 = Convert.ToDouble(Console.ReadLine());
                Console.WriteLine("Enter number of total possible parts: ");
                double a2 = Convert.ToDouble(Console.ReadLine());

                double s = a1 / a2;
                double sum = (s * 100);

                Console.WriteLine("your percentage is: " + sum);

            }else if (num == "2")
            {
                Console.WriteLine("\nCalculate the percentage the number");
                Console.WriteLine("Enter percentage: ");
                double a3 = Convert.ToDouble(Console.ReadLine());
                if (a3 > 100)
                {
                    Console.WriteLine("Incorrect sum of percentage");
                }
                Console.WriteLine("Enter Total number: ");
                double a4 = Convert.ToDouble(Console.ReadLine());

                double sum2 = (a4 * (a3/100));

                Console.WriteLine("Your Number is: " + sum2);
            }else
            {
                Console.WriteLine("Invalid");
            }
        }
    }


}
