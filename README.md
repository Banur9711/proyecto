        // Solicitar nombre y edad
        Console.WriteLine("=== Programa de Operaciones Básicas ===\n");
        
        Console.Write("Ingresa tu nombre: ");
        nombre = Console.ReadLine();

        Console.Write("Ingresa tu edad: ");
        edad = int.Parse(Console.ReadLine());

        // Solicitar dos números para las operaciones
        Console.WriteLine("\nAhora ingresa dos números para realizar operaciones:");
        Console.Write("Número 1: ");
        numero1 = double.Parse(Console.ReadLine());

        Console.Write("Número 2: ");
        numero2 = double.Parse(Console.ReadLine());

        // Operaciones básicas
        double suma = numero1 + numero2;
        double resta = numero1 - numero2;
        double multiplicacion = numero1 * numero2;
        double division = 0;

        if (numero2 != 0)
            division = numero1 / numero2;
        else
            Console.WriteLine("\n¡Advertencia! No se puede dividir entre cero.");

        // Mostrar resultados
        Console.WriteLine("\n=== RESULTADOS ===");
        Console.WriteLine($"Nombre: {nombre}");
        Console.WriteLine($"Edad: {edad} años");
        Console.WriteLine($"\nOperaciones con {numero1} y {numero2}:");
        Console.WriteLine($"Suma:          {numero1} + {numero2} = {suma}");
        Console.WriteLine($"Resta:         {numero1} - {numero2} = {resta}");
        Console.WriteLine($"Multiplicación:{numero1} * {numero2} = {multiplicacion}");
        
        if (numero2 != 0)
            Console.WriteLine($"División:      {numero1} / {numero2} = {division}");
        else
            Console.WriteLine("División:      No definida (división entre cero)");

        Console.WriteLine("\n¡Programa terminado! Presiona cualquier tecla para salir...");
        Console.ReadKey();
    }
}
