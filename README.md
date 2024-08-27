# Experiment-11
## AIM
To study and implement Classes and Objects.
## THEORY
Classes: Definition: A class is a blueprint or template for creating objects. It defines the properties (data members) and behaviors (member functions or methods) that the objects created from the class will have.

object: Definition: An object is an instance of a class. When you create an object, you are creating a specific example of the class, with its own set of data.
## CODE AND OUTPUT
A.
```
#include <iostream>
using namespace std;

class cube
{
    public:
    int height = 2.0;
    int width = 3.0;
    int length = 5.0;
};

int main()
{
    cube c1;
    int vol = c1.height*c1.width*c1.length;
    cout<<"volume:"<<vol<<endl;
}
```
![A1](https://github.com/user-attachments/assets/f98ab9ec-4bda-46db-9bd8-e34b057207ce)

B
```
#include <iostream>
using namespace std;

class cube
{
    public:
    int height = 2;
    int width = 2;
    int length = 2;
    int volume()
    {
        int v; 
        v = height*width*length;
        return v;
    }
};

int main()
{
    cube cube1;
    cout<<"volume: "<<cube1.volume()<<endl;
}
```
![A2](https://github.com/user-attachments/assets/bef03c92-f065-434f-8317-61292c036e58)

C
```
#include <iostream>
using namespace std;

class cube
{
    private:
    int height=2;
    int width=3;
    int length=5;

    public:
    int volume()
    {
        double v;
        v=height*width*length;
        return v;
    }
};

int main()
{
    cube cube1;
    cout<<"volume: "<<cube1.volume()<<endl;
}
```
![A3](https://github.com/user-attachments/assets/4a821c5b-7482-4081-beab-4861e55298ef)

D
```
#include <iostream>
using namespace std;
class cube{
    public:
    double height=2.0;
    double width=3.0;
    double length=5.8;
     double volume(){
     double v;
     v=height*width*length;
        return v;
}
void disp_vol(double vol){
    cout<<"Volume:"<<vol<<endl;

}
};
int main()
{
    cube cube1;
    double vol=cube1.volume();
    cube1.disp_vol(vol);
}
```
![A4](https://github.com/user-attachments/assets/a4fc43dd-9f0c-4f4e-a9e7-e6e63dbd59be)

E
```
#include <iostream>
using namespace std;

class Volume 
{
    public:
        float length;
        float breadth;
        float height;
        
        void input() {
            cout << "Enter the value of length: ";
            cin >> length;
            cout << "Enter the value of breadth: ";
            cin >> breadth;
            cout << "Enter the value of height: ";
            cin >> height;
        }
                float vol() {
            return length * breadth * height;
        }
        
        void display() {
            double a = vol();
            cout << "The volume is " << a;
        }
};

int main() {
    Volume volume1;
    volume1.input();
    float a = volume1.vol();
    cout << a;
    return 0;
}
```
![A5](https://github.com/user-attachments/assets/317df3b6-b062-47db-a291-180b60dd8dce)
