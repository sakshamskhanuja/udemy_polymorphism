## Polymorphism

### Description

For this exercise you will create four classes of vehicles. The first class should be named <b>Car</b>. This will be the base class for three other classes, <b>Mitsubishi</b>, <b>Holden</b>, and <b>Ford</b>.

The first class contains four member variables, or fields, with these names and conditions:

<ul>
<li><b>engine</b> of type <b>boolean</b></li>
<li><b>cylinders</b> of type <b>int</b></li>
<li><b>name</b> of type <b>String</b></li>
<li><b>wheels</b> of type <b>int</b></li>
</ul>

All four member variables should have <b>private</b> access.

The constructor should accept two parameters, <b>cylinders</b> and <b>name</b>. Also, all of these cars have an engine and four wheels. So the other two fields should be set to default values.

In addition, there are five other methods These methods should be defined as described below:

<ul>
<li><b>startEngine</b> accepts no parameters and returns a message which says that the car's engine is starting.</li>
<li><b>accelerate</b> accepts no parameters and returns a message that says the car is accelerating.</li>
<li><b>brake</b> accepts no parameters and returns a message stating the car is braking.</li>
</ul>

The messages these methods return should somewhere contain the name of the class, Car.

Two getter methods should also be defined here for the member variables cylinders and name. All methods have <b>public</b> access.

The other three classes mentioned above are sub-classes of <b>Car</b>. These classes have no member variables and the constructor for each will call the parent constructor for object instantiation. Each of these classes will override the three parent methods <b>startEngine</b>, <b>accelerate</b>, and <b>brake</b>. The return messages for these methods should somewhere contain the name of the class to which the methods belong.

### Test Code

    Car car = new Car(8, "Base car");
    System.out.println(car.startEngine());
    System.out.println(car.accelerate());
    System.out.println(car.brake());
     
    Mitsubishi mitsubishi = new Mitsubishi(6, "Outlander VRX 4WD");
    System.out.println(mitsubishi.startEngine());
    System.out.println(mitsubishi.accelerate());
    System.out.println(mitsubishi.brake());
     
    Ford ford = new Ford(6, "Ford Falcon");
    System.out.println(ford.startEngine());
    System.out.println(ford.accelerate());
    System.out.println(ford.brake());
     
    Holden holden = new Holden(6, "Holden Commodore");
    System.out.println(holden.startEngine());
    System.out.println(holden.accelerate());
    System.out.println(holden.brake());

### Output

    Car -> startEngine()
    Car -> accelerate()
    Car -> brake()
    Mitsubishi -> startEngine()
    Mitsubishi -> accelerate()
    Mitsubishi -> brake()
    Ford -> startEngine()
    Ford -> accelerate()
    Ford -> brake()
    Holden -> startEngine()
    Holden -> accelerate()
    Holden -> brake()
