using System;

class Program
{
    static void Main()
    {
        //Create an instance of the Bunny class (nested inside Animal)
        Animal.Bunny myBunny = new Animal.Bunny();
        
        //Access properties and methods of the public Bunny class
        Console.WriteLine("The name of the bunny is: " + myBunny.Name);
        myBunny.Hop();
    }
}
//Outer class
public class Animal
{
    //Nested class
    public class Bunny
    {
        //Property
        public string Name { get; set; }
        //Constructor
        public Bunny()
        {
            Name = "Noctis";
        }
        //Method
        public void Hop()
        {
            Console.WriteLine(Name + " likes Carrots and Humans.");
        }
    }
}
