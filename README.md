# Code-2
abstract class  Shape
{
	abstract int numberOfSides();
}
class Rectangle extends Shape
{
	int numberOfSides()
	{
		return 4;
	}
}
class Triangle extends Shape
{
	int numberOfSides()
	{
		return 3;
	}
}
class Hexagon extends Shape
{
	int numberOfSides()
	{
		return 6;
	}
}
public class Main
{
	static int sumOfAngles(int n)
    {
		       return (n-2)*180;
    }
	public static void main(String[] args)
	{
		Rectangle obj1= new Rectangle();
		Triangle obj2 =new Triangle();
		Hexagon obj3= new Hexagon();
		System.out.println("Sides of rectangle is: "+obj1.numberOfSides()+" ,sum of angle: "+sumOfAngles(obj1.numberOfSides()));
		System.out.println("Sides of triangle is: "+obj2.numberOfSides()+", sum of angle: "+sumOfAngles(obj2.numberOfSides()));
		System.out.println("Sides of hexagon is: "+obj3.numberOfSides()+" ,sum of angle: "+sumOfAngles(obj3.numberOfSides()));
	}
}
