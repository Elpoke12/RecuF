# RecuF

Algorimo
<3

class ClaseFibonacci
	{
        
        static int RecurF(int n)
    {
            if(n==1||n==0)
            {
                return 1;
            }
            else
            {
                return RecurF(n - 1) + RecurF(n - 2); 
            }

    }

    static void Main(string[] args)
    {
            TimeSpan stop;
			TimeSpan start = new TimeSpan(DateTime.Now.Ticks);
            int n;
            Console.Write("Ingrese un valor: ");
            n = int.Parse(Console.ReadLine());
            for (int v = 0; v < n;v++)
            {
                Console.Write("El Fibonacci "+ (v+1)+ " es "+ RecurF(v)+ "\n");
            }
            Console.Write("Se completo en: ");
		stop = new TimeSpan(DateTime.Now.Ticks);
		Console.WriteLine(stop.Subtract(start).TotalSeconds);
        Console.ReadKey();
    }
  }
