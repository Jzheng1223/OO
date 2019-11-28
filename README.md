# 0624084 鄭智升
## 0624084 鄭智升
### 0624084 鄭智升
#### 0624084 鄭智升
##### 0624084 鄭智升
###### 0624084 鄭智升

:cry:
:top:
:car:

| 1 | 1 | 1 |
|:--| :--: |--:|
| 1 | 2 | 3 |

[Nkust](https://www.nkust.edu.tw/)

![Paradise](Weed.jpg)

[巨槌國動 開剁](https://www.youtube.com/watch?v=rV1C_GzJESA)
[你過來一下](https://youtu.be/gbp8-KbYtWA)
[巨槌國動 開剁](https://www.youtube.com/watch?v=rV1C_GzJESA)
#

```js
import java.util.;
import java.lang.;
import java.io.;

abstract class CShape
{
    protected String color;
    public void setColor(String str)
    {
        color = str;
    }
    public abstract void show();
}
class CTriangle extends CShape
{
    protected int side_a,side_b,side_c;
    public CTriangle(int a,int b,int c)
    {
        side_a=a;
        side_b=b;
        side_c=c;
    }
    public void show()
    {
        System.out.print("color="+color+",");
        System.out.print("area="+0.5*side_a*side_b);
    }

}
public class app11_1
{
    public static void main(String args[])
    {
        CTriangle trian = new CTriangle(3,4,5);
        trian.setColor("RED");
        trian.show();
    }
}



public interface Shape {  // Use keyword "interface" instead of "class"
   // List of public abstract methods to be implemented by its subclasses
   // All methods in interface are "public abstract".
   // "protected", "private" and "package" methods are NOT allowed.
   double getArea();
}
// The subclass Rectangle needs to implement all the abstract methods in Shape
public class Rectangle implements Shape {  // using keyword "implements" instead of "extends"
   // Private member variables
   private int length;
   private int width;

   // Constructor
   public Rectangle(int length, int width) {
      this.length = length;
      this.width = width;
   }

   @Override
   public String toString() {
      return "Rectangle[length=" + length + ",width=" + width + "]";
   }

   // Need to implement all the abstract methods defined in the interface
   @Override
   public double getArea() {
      return length * width;
   }
}
// The subclass Triangle need to implement all the abstract methods in Shape
public class Triangle implements Shape {
   // Private member variables
   private int base;
   private int height;

   // Constructor
   public Triangle(int base, int height) {
      this.base = base;
      this.height = height;
   }

   @Override
   public String toString() {
      return "Triangle[base=" + base + ",height=" + height + "]";
   }

   // Need to implement all the abstract methods defined in the interface
   @Override
   public double getArea() {
      return 0.5 * base * height;
   }
}
