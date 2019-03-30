### Objects

- Split your objects by nouns (things).
- In the provided example the following are nouns:

  - Player
  - Tower
  - Map
  - Invader
  - Path

- Best practices dictate we put each of these objects into their own file.

```CS
// We will also need `Game.cs` that contains the `Main()` method - to indicate which file to run first.
Player.cs
Tower.cs
Map.cs
Invader.cs
Path.cs
```

#### Instanciating a new class

- In `Game.cs` if we want to instanciate a Tower object we need to call it.
- Below: we create a new instance of Tower with `new Tower();`.
- Then, we assign the instance of Tower to the `tower` variable.
- We also set the type of tower variable. We could use `var`, but we can also specify the variable as an object type - which reads cleaner.
- So the entire line then becomes `Tower tower = new Tower();`

```CS
namespace TreehouseDefense
{
    class Game
    {
        public static void Main()
        {
            Tower tower = new Tower();
        }
    }
}
```

#### Fields (AKA attributes)

- The `Map` can be defined with two attributes, `height` & `width`.

```cs
namespace TreehouseDefense
{
  class Map
  {
    int Width:
    int Height:
  }
}
```

##### Access Modifiers

- Public: can be accessed by any method in any class or instances of class - Use case: API.
- Private: cannot be access by an instance of the class. Can only be accessed by the same methods in the class they are declared in.

```cs
namespace TreehouseDefense
{
  class Map
  {
    public int Width:
    private int Height:
  }
}
```

#### Constructor Method

- The constructor is called when objects are created.
- The user of the class must provide the parameter (class attribute) values in order for the object to be constructed.
- We need to use the parameters to initalize the fields (attributes) - done in the body.

```cs
namespace TreehouseDefense
{
  class Map
  {
    public readonly int Width:  // Instance variables. Exist as long as the object exists.
    public int Height:          // Convention - Instance variables are uppercase.
                                // `readonly` prevents users from changing the values of the parameters.

    public Map(int width, int height)  // Method level variables. Only exists inside this method (function).
    {                                  // Convention - Method level variables are lowercase.
      Width = width;
      Height = height;
    }
  }
}
```

- Note: the `void` keyword signifies the method doesn't return anything.
- `Void` isn't used on constructor methods, because constructors can't return anything.

#### Cartesian Coordinates

- Are used to identify a point on a two dimensional grid.
