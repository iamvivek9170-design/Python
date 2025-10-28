# def my_dict_store():
            
mydict  = {
        1: "A", 
        2: "B", 
        3: "C", 
        4: "D", 
        5: "E", 
        6: "F", 
        7: "G", 
        8: "H", 
        9: "I", 
        10: "J"
        




        # "Canada": "Ottawa",
        # "USA": "Washington, D.C",
        # "Brazil": "Brasília",
        # "Chile": "Santiago" ,
        # "France": "Paris",
        # "Germany": "Berlin",
        # "Italy": "Rome",
        # "Russia": "Moscow",
        # "China": "Beijing" ,
        # "India": "New Delhi",
        # "Indonesia": "Jakarta",
        # "Japan": "Tokyo",
        # "Pakistan": "Islamabad"        
    }
print(mydict)
   

while(True):
    # my_dict_store()

    print("\n--- Dictionary Operations Menu ---")
    print("1. Add new country-capital")
    print("2. Update capital of an existing country")
    print("3. Delete a country")
    # print("4. Search capital by country")
    # print("5. Display all country-capital pairs")
    # print("6. Exit")
    choice = int(input("Which operation do you want to perform : "))
    

    if (choice == 1):
        print ("To Add")
        key = int(input("Enter kay value"))
        if key in mydict:
            print("Already exist in dicttonary")
        else :
            value = input("Enter value to add new one")
            mydict[key]= value
            print(mydict)


    elif (choice == 2):
        print ("To update")
        key = int(input("Enter kay value"))
        if key in mydict:
            value = input("Enter value to update")
            mydict[key] = value
            print(mydict)
        else :
            print("your key is not in dictonary")


    elif (choice==3):
        print("\n--- Accessing the Dictionary  ---")
        print("1. To access the value by key")
        print("2. To acces all key")
        print("3. To acsess all values")
        print("4. To access all items")


        aa = int(input("Enter how you want to acces the dictionary....... "))
        
        if (aa == 1):
            key = int(input("Enter the key to access the value : "))
            if key in mydict :
                a = mydict[key]
                print(f"the value for {key} is {a}")
            else :
                print("key is not present in the dictionary")  
        elif (aa == 2):
            a = mydict.keys()
            print("All key in the dictionary",a)
        elif (aa == 3):
            b = mydict.values()
            print("All values in the dictionary",b)
        elif (aa ==4):
            c = mydict.items()
            print("All items in the dictionary",c)
        else :
            break
    

        
         
        





    


    

    
    
    
    # choose = input("Enter any value to continue......")
    # if (choose=="N"):
    #     break
