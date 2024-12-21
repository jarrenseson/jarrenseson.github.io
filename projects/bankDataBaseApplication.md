---
layout: project  
type: project  
image: img/download.jpg  
title: "ICS 212: Bank Database Application"  
date: 2023  
published: true  
labels:  
  - C++  
summary: "A simple banking application that allows users to add 'records' to a linked list, implemented independently."  
---

<img src="/img/single_customer_profile-01_1.webp" class="center">  

This application was developed as part of my program structure class. I created a mock bank database that allowed users to be added, deleted, or searched. The database consisted of a list of users represented by their name, account number, and address, implemented as a linked list data structure. Both the UI and backend were developed in separate files.  

I independently developed this project in my program structure class, receiving general advice from my teaching assistant (TA).  

Through this project, I learned about the linked list data structure and how it functions by chaining each user to another. By implementing the linked list, I gained deeper insight into dynamic memory allocation and pointers, as well as how to handle related errors. Additionally, working with C++, a low-level language, allowed me to better understand object-oriented programming concepts. Developing the user interface also provided valuable experience in creating user-friendly designs.  

~~~cpp
int llist::addRecord(int account_num, char name[], char address[])  
{  
    int return_value = 1;  
    struct record *previous_record;  
    struct record *current_record;  
    struct record *temp;  
    current_record = this->start;  
    previous_record = NULL;  

    #ifdef debug  
        std::cout << "\n/**************************************************************************";  
        std::cout << "\n// ENTERING: addRecord";  
        std::cout << "\n// Parameters";  
        std::cout << "\n// Account Number: " << account_num;  
        std::cout << "\n// Name: " << name;  
        std::cout << "\n// Address: " << address;  
        std::cout << "\n***************************************************************************\n";  
    #else  
        if (current_record == NULL)  
        {  
            current_record = (struct record *) new record;  
            (this)->start = current_record;  
            (current_record)->accountno = account_num;            
            strncpy((current_record)->name, name, 30);         
            strncpy((current_record)->address, address, 50);         
            (current_record)->next = NULL;  
            return_value = 0;  
        }  
        else  
        {  
            if (account_num > (current_record)->accountno)  
            {  
                temp = (struct record *) new record;  
                temp->accountno = account_num;            
                strncpy((temp)->name, name, 30);         
                strncpy((temp)->address, address, 50);         
                (temp)->next = current_record;  
                (this)->start = temp;  
                return_value = 0;  
            }  
            else  
            {  
                while (current_record != NULL && account_num < (current_record->accountno))  
                {  
                    temp = (current_record)->next;  
                    previous_record = current_record;   
                    current_record = temp;                      
                }  
                if (current_record != NULL && account_num == (current_record->accountno)) // Accounting for the middle of the list and duplicate accounts  
                {  
                    return_value = 1;  
                }  
                else  
                {  
                    temp = (struct record *) new record;  
                    (previous_record)->next = temp;  
                    (temp)->accountno = account_num;  
                    strncpy((temp)->name, name, 30);     
                    strncpy((temp)->address, address, 50);  
                    (temp)->next = current_record;  
                    return_value = 0;  
                }    
            }  
        }  
    #endif  

    return return_value;  
}  
~~~  

The code above demonstrates my implementation of the `addRecord` method for a linked list, showcasing my understanding of pointers and dynamic memory allocation.  

Click [here](https://github.com/jarrenseson/ICS-212-Bank-Database-Application.git) to view the full code.  
