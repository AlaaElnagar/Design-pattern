**Design patterns**

**Introduction**

Design patterns become popular after publishing of the book **Design Patterns  Elements of Reusable Object-Oriented Software book** *at 1995*

This book was written by four editors so it was known as Gang of Four design patterns

Target was finding solutions for OO design problems

**What is meant by a pattern :**

The keyword pattern was built by the architect Cristopher alexander  he defined it to solve a common problems 

Language and domain independent for solving OOP design problems

patterns deliver different ways to solve recurring issue providing flexibility and reusability 

developers can use these patterns as suggestions to solve their problems 

[Note] A pattern give a generic solution and can have different implementation 

**Design pattern catalogue**

01- Creational patterns

These patterns provide various object creation mechanisms, which increase flexibility and reuse of existing code.

02- Structural patterns

These patterns explain how to assemble objects and classes into larger structures while keeping these structures flexible and efficient

03- Behavioral patterns

These patterns are concerned with algorithms and the assignment of responsibilities between objects.

 <p align="center">
  <img src="img9.jpg" />  
</p>


UML Class diagram

To understand the pattern and how interaction occurs  UML  understanding is needed

What mean by UML : UML stands for unified machine language and consists of 

01 - class 

Each class consists of a class name , attributes and the methods that class contains 

![](img\img10.PNG)

**example**

![](/img/img11.PNG)

### relations between classes and each others

To understand how classes interact with each others main types of relation lines understanding is needed

### 1-Inheritance (Generalization):

Is used when there is a parent class and child class and we need to show the relation between each others that the child **Savings and Current** classes is inherited from Account as shown 

**Note** Generalization arrow is empty and points to the most general class to inherit from 

​                                                                                                                                                        ![](img\img12.PNG)

### 2-Abstract class 

The name of abstract class is shown in italics  and contains virtual method and must be implemented by child classes and also it uses generalization arrow

​                                                                                                                       ![](img\img13.PNG)



### 3- Composition 

A composition show part of for example Button is part of window and when window the `container`  is destroyed the button will be destroyed `one of container elements`  also and we can represent that using composition  arrow

​                                                                                                                                          ![](img\img14.PNG)

### 4-Aggregation

The need for aggregation appears when we need to destroy the container and keep it's elements and can be represented with hollo diamond a

​																																	        ![](img\img15.PNG)

​                      																												                                                                     

### 4-Association

### Appears when   a class need  to use a feature of other class  as shown here the driver use the  car  association relationship represented with a arrow 

​                                                                                                                                ![](img\img16.PNG)

**5-Note notation** 

​    This  notation is needed  when extra notes is needed and not mentioned in the diagram and known as a comment  as shown PI is a constant                                                                                                                              																																							![](img\img17.PNG)![](img\img18.PNG)



