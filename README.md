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

    
