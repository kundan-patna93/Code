1) Check whether following json is valid or invalid. If Invalid correct it.
   
         code:
         import json
         def json_validation(data):
            try:
               json_data=json.loads(data)
               print("Valide formate")
            except:
               print("Invalide formate")
         data= """{ "company":{ "employee":{ "name":"emma", "payble":{ "salary":7000, "bonus":800} } } }"""

         json_validation(data)
         
 2) Rename key of a dictionary.
 
         code:
         dic[new_key]=dic.pop[old_key]
         
 3) Assign a different name to function and call it through the new name.
 
         code:
         def show_record(name):
           print(name)

         show_record(name="sunil")
         display_record=show_record
         display_record(name="krishana")
      
 4) Open two python threads and share a blank list between them.Then start first thread and append even numbers from 1 to 10 in the list,next start 2nd           thread and append odd.
 
             
         code:
         from threading import *
         from time import sleep

         #Create list with use global
         global lst
         lst=[]

         class EvenClass(Thread):
             def run(self):
                 for i in range(1,11):
                     if i%2==0:
                         lst.append(i)

         class OddClass(Thread):
             def run(self):
                 for i in range(1,11):
                     if i%2!=0:
                         lst.append(i)

         #Create Object
         obj1=EvenClass()
         obj2=OddClass()

         obj1.start()
         sleep(1)
         obj2.start()

         print(lst)

 
 
 5) Write a program to find HCF & LCM of given values:
         
         
         
          code:HCF
          def find_hcf(a,b):
             for i in range(1,(min(a,b))+1):
                if a%i==0 and b%i==0:
                   hcf=i
             print("HCF:",hcf)
          find_hcf(702, 153)

         
          Code:LCM
          def find_lcm(a,b,c,d):
             i=max(a,b)
             while i>0:
                if i%a==0 and i%b==0 and i%c==0 and i%d==0:
                   lcm=i 
                   break
                i=i+1

             print("LCM: ",lcm)
          find_lcm(31, 99, 33, 33)
 
 
 
 6) Write a program to find LCM of given array elements

          
          Code:HCF
          def find_hcf_array_element(lst):
            for i in range(1,(min(lst))+1):
               c=0
               for val in lst:
                  if val%i==0:
                     c=c+1
               if len(lst)==c:
                  hcf=i
            print("HCF: ",hcf)

          find_hcf_array_element(lst=[350, 500, 130, 260])

          
          code:LCM
          def find_lcm_array_element(lst):
            i=1
            while i>0:
               c=0
               for val in lst:
                  if i%val==0:
                     c=c+1
               if len(lst)==c:
                  lcm=i
                  break
               i=i+1
    
            print("LCM: ",lcm)
          fine_lcm_array_element(lst=[76, 26, 72])
          
          
   
7) Without inbulid function reverse the list element.

         code 1:
         def reverse_list_element(list_val):
            l=len(list_val)
            out=[]
            for i in range((l-1),-1,-1):
               out.append(list_val[i])
            print(out)

         list_val=[1,2,4,5,6,9,8,7]
         reverse_list_element(list_val)
         
         code 2: 
         def reverse_list(lst):
            l=len(lst)
            for i in range(0,len(lst)//2):
               tem=lst[i]
               lst[i]=lst[len(lst)-i-1]
               lst[len(lst)-i-1]=tem
         print(lst)

         lst=[2,4,6,8,10,12]
         reverse_list(lst)
         
         code 3:
         def reverse_list(lst):
            l=len(lst)//2
            for i in range(l):
               lst[i],lst[-1-i]=lst[-1-i],lst[i]
            print(lst)

         lst=[2,4,6,8,10,12]
         reverse_list(lst)
         
         
8) .CSV file Write and Read contents:

         Code : Write CSV File
         import csv
         def create_csv_file_insert_records():
             with open("emp.csv",'w',newline="") as f:
                 w=csv.writer(f)
                 w.writerow(["Name","Age","salary"])
                 n=int(input("Enter no of record: "))
                 for i in range(n):
                     name=input("Enter name: ")
                     age=int(input("Enter age: "))
                     salary=int(input("Enter salary: "))
                     w.writerow([name,age,salary])
                     print("insert record: ",i,"\n")
         create_csv_file_insert_records()
         
         
         Code : Read CSV file
         import csv
         def read_csv_file_show_the_data():
          with open("emp.csv",'r') as f:
              r=csv.reader(f)
              for val in r:
                  for val2 in val:
                      print(val2,end="\t")
                  print()
        read_csv_file_show_the_data()
         
         
9) .Zip and unzip files

         code : Zip files
         from zipfile import *
         def zip_file():
             f=ZipFile("files.zip",'w',ZIP_DEFLATED)
             f.write("file1.txt")
             f.write("file2.txt")
             f.write("file3.txt")
             f.close()
             print("successfull create zipfile")
         zip_file()
         
         
         code : Unzip files
         def unzip_file():
          f=ZipFile("files.zip","r",ZIP_DEFLATED)
          names=f.namelist()
          for name in names:
              print("file name: ",name)
              f1=open(name,'r')
              print(f1.read())
              print()
         unzip_file()




10) .

         code :
11) .

         code :
         
         


    
