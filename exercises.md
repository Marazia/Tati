

 ## More exercises on Python strings

  Use the `len` to print the lenght of the string:

  ` x = "Hello World"
   print(len(x)) `

  Return the string without any whitespace at the beginning or the end.
  
  ` txt = " Hello World "
   x = txt.strip() `

  Convert the value of `txt` to  upper case
  
  ` txt = " Hello World "
   txt = txt.upper() ` 


  Convert the value of `txt` to  lower case
   
   ` txt = " Hello World "
     txt = txt.lower() `
  
  Replacing characters
    
   ` txt = " Hello World "
     txt = txt.replace ("H", "J")

  ## More exercises on Python operators

  **Membership operator**
  `fruits = ["apple", "banana"] 
   if "apple" in fruits
   print(" Yes, apple is a fruit! ")`

  ## Changing lists 
   
    **Changing "apple" to kiwi**
   `fruits = ["apple", "banana", "cherry"]
    fruits[0] = "kiwi" `

    **Use `insert` adding "lemon" as the second item in fruits list:**
   `fruits = ["apple", "banana", "cherry"]
    fruits.insert(1, "lemon")

  ## Changing sets
   
   **adding multiple items (more_fruits) to the fruits set.**
   
   `fruits = {"apple", "banana", "cherry"}
    more_fruits = ["orange", "mango", "grapes"]
    fruits.update(more_fruits)

   **`discard` method of removing items of sets
   	
   `fruits = {"apple", "banana", "cherry"}
    fruits.discard("banana")

  ## Dictionaries 

    `get` printing method 
   
   **Using `get` to print the value of the "model" key of the `car` dictionary**
  
   `car = {
   "brand": "Ford"
   "model": "Mustang"
   "year": 1964
   }
    
    print(car.get("model") `

   **Changing "year" value from 1964 to 2018**
   
   `car = {
    "brand": "Ford"
    "model": "Mustang"
    "year": 1964
    }
    
    car["year"] = 2018`

   ** Adding a key-value pair **
     `car = {
    "brand": "Ford"
    "model": "Mustang"
    "year": 1964
    }
    
     car["color"] = "red" `

   **Removing with `pop` method**
     ` car = {
     "brand": "Ford"
     "model": "Mustang"
     "year": 1964
     }
    
     car.pop("model") `

   **Emptying a dictionary with `clear` method**
    `car = {
     "brand": "Ford"
     "model": "Mustang"
     "tear": 1964
     }
   
     car.clear() `

   

    ##If...else

    Print "Hello World!" if a is greater than b
 `
    a = 50
    b = 10 
    if a > b:
    print( "Hello World!") `

   Print "Hello World!" if a is not equal to b
 `
    a = 50
    b =10 
    if a != b:
    print( "Hello World!") `


   If... else 
   
  ` a = 50
    b = 10 
    if a == b:
    print("Yes")
    else:
    print("No") `
  
  ` a = 50 
    b = 10 
    if a == b:
    print ("1")
    if a > b:
    print("2")
    else: 
    print("3")
 
   While loops

  
  