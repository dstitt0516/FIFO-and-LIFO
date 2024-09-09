import names

go = 1
people_through_store = 0
customer_queue = []
customer_counter = 0
customer_count = (customer_counter, "customers are in the store.")


print("Type '1' to add someone to the checkout")
print("Type '2' to have the cashier checkout the first person in line")
print("Type '3' to have the cashier checkout the last person in line")
print("Type '4' to end the checkout session")

while go == 1:
    choice = int(input("Type 1, 2, 3, or 4! "))
    #try
    print('')
#____________________________________________________________________
    if choice == 2 and customer_counter == 0 or choice == 3 and customer_counter == 0 :
        print("You cannot check anyone out if there is no one in the store!")
        print("")

    if choice >= 5 or choice <= 0:
        print("This option is not accepted try again!")
        print("")
#____________________________________________________________________ 
    if choice == 1:
        
        for i in range(1):
            x = names.get_full_name()
            customer_queue.append(x)
            customer_counter += 1
            customer_count = customer_counter, "customers are in the store."
            print(customer_queue)
            print(customer_count)
            print('')    #____________________________________________________________________
    if choice == 2 and customer_counter > 0:
        customer_queue.pop(0)
        customer_counter -= 1
        people_through_store += 1
        customer_count = customer_counter, "customers are in the store."
        print(customer_queue)
        print(customer_count)
        print('')
    #____________________________________________________________________
    if choice == 3 and customer_counter > 0:
        if customer_counter < 2:
            customer_queue.pop(0)
            customer_counter -= 1
            people_through_store += 1
            customer_count = customer_counter, "customers are in the store."
        
            
        if customer_counter > 1:
            customer_queue.pop(customer_counter - 1)
            customer_counter -= 1
            people_through_store += 1
            customer_count = customer_counter, "customers are in the store."
        print(customer_queue)
        print(customer_count)
        print('')

#____________________________________________________________________
    if choice == 4:
        go -= 1
        print(people_through_store, "people went through the store and you left", customer_counter, "people in the store.")
