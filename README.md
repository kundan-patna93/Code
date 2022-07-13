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

    
