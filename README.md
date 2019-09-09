List:

    1:Create empty list and add some element in the list.        
            L=[]
            L=eval(input("enter values in list"));
            print(L);
            print(type(L))
            
    2:write a program show the odd and even no in list withot using Loop and % operator.
            liste=(list(range(1,100,2)));
            print(liste)

    
    3:write a program input the sentence and show seperate with word.
            Sent="i am kundan kumar"
            print(list(Sent));   """sentene into character"""
            print(Sent.split()); """sentence into word"""

    
    4:write a program input data in nasted list.
            liste1=[1,2,3,["sita","gita"],[10.2,10.2],[10+10j,11+20j]]
            print(liste1)        
    
    5:write a prgram input data in list after that you can edite the one particular data.
            liste1=[1,2,3,["sita","gita"],[10.2,10.2],[10+10j,11+20j]]
            print(liste1)
            print("After cahnge data");
            liste1[3][1]="Ram";
            print(liste1)
            
    6:writ a code input data in list and reverse it all element.        
            L=[]
            L=[1,2,3,4,5,6,7,8,9,10]
            print(L)
            L.reverse();
            print(L);
            
    7:write a program input the nubmer 1 to 100, in the list and only show even or odd number.
            L=[]
            for i in range(0,101,2):
                     L.append(i)
            print(L);

    
    8:Code show the possitive and Negetive index with the values
            L=[11,12,13,14,15]
            r=len(L)
            for i in range(r):
                   print("index",i,"Values",L[i],"And Negative index",i-r, "values",L[i])
    
    9:Count the number of elements in the presen list.
            L=[11,12,13,14,15]
            print(len(L))
            """whitout uing inbulid function"""
            c=0;
            for i in L:
               c=c+1;
            print(c);
    
    10:Add item at the end of the list.

    11:Add between 1 to 100 numbers, which are divisiable by 7
            L=[1,2,3,4,5]
            print(L);
            L.insert(0,100);
            print(L)
              
    12:writ a code To insert item at specified index possition.
            L=[11,12,13,14,15]
            print(L)
            L.insert(0,100);
            L.insert(3,300);
            print(L)
    
    13:write a code To add all items of one list to another list 
            L=[1,2,3,4,5]
            L1=[5,6,7,8,9]
            print(L,"and",L1)
            L.extend(L1)
            print(L);

    
    14:Code remove the element in the list, using remove() function.
            L=[11,12,13,14,15,15]
            print(L)
            L.remove(15)
            print(L);
    
    15:write a code remove the element using It removes and returns the last element of the list.
    
    16:wirte a code reverse of all element int the list using reverse function.
            L=[112,13,212,13,114,15,1]
            print(L)
            L.sort()
            print(L);

    
    17:wite a code short the all element using short() function
            L=[112,13,212,13,114,15,1]
            print(L)
            L.reverse()
            print(L);

    
    18:wrtie a program copy one list values to another list
            L=[112,13,212,13,114,15,1]
            print(L)
            print(type(L))
            C=L;
            print(C)
            print(type(C))

    
    19:write a program input two list values and assign third list
            L=[112,113,114,115,116]
            L1=[1,2,3,4,5,6,14,15,16,11]
            print(L)
            print(L1)
            C=L+L1
            print(C)
    
    20:write a program compaire two list values are equal are not
            L=[5,6,7,8,9,10]
            L1=[1,2,3,4,5,6]
            L2=[11,22,33,44,55]
            L3=[11,22,33,44,55.5]
            L4=['kundan','kumar']
            L5=['kundan','kumar']
            L6=['chandan','kumar']
            print(L==L2)
            print(L2==L3)
            print(L4==L5)
            print(L5==L6)


    21:write a program chek the particula element in list avilabel or not.
            L=[5,6,7,8,9,10]
            L1=[1,2,3,4,5,6]
            print(5 in L)
            print(6 in L1)
            print(11 in L)
            print(1 in L)

    
    22:write a program cleat all vales in the list
            L=[5,6,7,8,9,10]
            print(L)
            L.clear()
            print(L)

    
    23:write a program show n=[1,2,[21,22,[100,200,300,400,500],23,24,25],4,5]
       show 
       1)[1,2,[21,22,[100,200,300,400,500],23,24,25],4,5]
       2)[21,22,[100,200,300,400,500],23,24,25]
       3)[100,200,300,400,500]
       4)300
            L=[5,6,7,8,[1,2,[11,12,16,14,15],3,4,5],9,10];
            print(L)
            print(L[2])
            print(L[4])
            print(L[4][1])
            print(L[4][2])
            print(L[4][2][3])

    24:write a program input vales in list n=[[10,20,30],[40,50,60],[70,80,90]]
       show  matrix formate.
       [10, 20, 30]
       [40, 50, 60]
       [70, 80, 90]
       
       10 20 30
       40 50 60
       70 80 90
       
            L=[];
            L=eval(input("enter no in list: "))
            for i in L:
                     print(L);
                     print();
            for i in range(len(L)):
            for j in range(len(L[i])):
            print(L[i][j],end=" ");
                     print()

    25:write a program input 1 to 10 no in list show squre no using
       list comprehensions
            L=[i*i for i in range(1,11)]
            print(L);

    26:wirte a program take input words=["Balaiah","Nag","Venkatesh","Chiranjeevi"]
       show Output['B', 'N', 'V', 'C']
            L=["Balaiah","Nag","Venkatesh","Chiranjeevi"]
            L1=[i[0] for i in L]
            print(L1)


    27:write a progra input two list1, list2 and show comman element.
       num1=[10,20,30,40]
       num2=[30,40,50,60]
            L=[1,2,3,4,5]
            L1=[4,5,6,7,8]
            L2=[i for i in L if i in L1]
            print(L2)

