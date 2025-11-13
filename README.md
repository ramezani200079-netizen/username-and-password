# username-and-password
username = "admin"
password = "2000"

user = input("enter your username:")
pas = input("enter your password:")

if user == username and pas == password:
    print("Login successful")


    name_list = []
    while True:
        print("menu")
        print("1)add name")
        print("2)show name")
        print("3)remove name")
        print("0)exit")
        option = int(input("enter your optin:"))

        if option == 1:
            name = input("enter your name:")
            name_list.append(name)

        elif option == 2:
            print(name_list)


        elif option == 3:

             remove_name = input("enter name was to remove:")
             if remove_name in name_list:
                name_list.remove(remove_name)
                print("remove successfully")
             else:
                 print("the name was not in the list")

        elif option == 0:
            break
        else:
            print("invalid option")

else:
    print("The username or password is wrong")
