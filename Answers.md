# 1NebulaAssessment
## Database Challenges
### Question 1
The ERD can be improved by changing it to First Normal Form (1NF) where I remove repeating groups in the Employee table. This repeating group is the address information. I can name the new entity as EmployeeAddress. Next, I can identify the primary key for EmployeeAddress which will be AddressId. The Employee entity is now in 1NF with the repeating group removed.

### Question 2

Please see the attached images **(DBCode, DBNumberofTicketsSold, TicketsTable, MoviesTable)** with the SQL Script.

## Back-end Code Challenges
### Question 1

```C#
    static void Main(string[] args)
    {
      String name = "Orange";
      myMethod(name);
    }

    static void myMethod(String str){
    if(str.Length % 2 == 0){
      Console.WriteLine("Stack");
    }
    if(str.Length % 4 == 0){
       Console.WriteLine("Overflow");
    }
    if(str.Length % 2 == 0 && str.Length % 4 == 0){
      Console.WriteLine("Stack Overflow!");
    }
    else{
    Console.WriteLine("Odd number!");
    }
  }
}
```
### Question 2
```c#
 public class Animal
    {
        public string Eat()
        {
            return "Yummy";
        }

        public virtual string MakeNoise()
        {
            return "Durrr";
        }
    }
    
    class Horse : Animal
    {
    
    	public Horse()
        {
        	Animal = new Horse();
        }
        
        public override void Eat()
        {
            Console.WriteLine("Yummy");
        }

        public override void MakeNoise()
        {
            Console.WriteLine ("Neigh");
        }
    }
    
    class Sheep : Animal
    {
    
    	public Sheep()
        {
        	Animal = new Sheep();
        }
        
        public override void Eat()
        {
           Console.WriteLine ("Yummy");
        }

        public override void MakeNoise()
        {
            Console.WriteLine ("Baaah");
        }
     }
```

## Front-end Code Challenges
### Question 1
1. firstDiv = red, secondDiv = orange
2. Once the code runs, the user will have to click on the **Change Color** button first:
```html
  <!DOCTYPE html>
<html>
<head>
<title>Page Title</title>
</head>
<body><div id="firstDiv" class="red-card">
<button onclick="changeColor();">Change Color</button>
<h1>This is a Heading</h1>
</div><div id="secondDiv" class="red-card">
<p>This is a paragraph.</p>
</div><style>
#secondDiv {
background: orange;
} div {
height: 150px;
width: 150px;
background: green;
} .red-card {
background: red;
} .yellow-card {
background: yellow;
}
</style>
  </body>
  </html>
  ```
  
  ```script
  <script>

function changeColor(){
var element = document.getElementById("firstDiv");
element.style.backgroundColor = "pink";
}

</script>
```
3.

### Question 2
