---
layout: project
type: project
image: img/download.jpg
title: "ICS 212: Bank Database Application"
date: 2023
published: true
labels:
  - C++
summary: "Simple banking application that allowed the user to add 'records' to a linked list, implemented by myself."
---

<img src="/img/single_customer_profile-01_1.webp" class="center">

This application was developed by me in my program structure class. I created a mock bank database, which allowed users to be added, deleted, or searched. The database was a list of users, represented by their name, account number, and address in a linked list data structure, implemented by myself. Both the UI and backend were implemented in separate files.

I developed this project by myself in my program structure class with some general advice from my TA.

Through developing this project, I learned about the linked list data structure and how exactly it works, by chaining each user to another. Through the implementation of the linked list data structure, I gained more insight into dynamic memory allocation and pointers. Specifically, how to deal with errors pertaining to them. Also, since C++ is such a low level language, it also allowed me to further grasp exactly how object orientated programming works. Working on the UI also gave me insight in how to develop a user friendly interface. 

~~~
int llist::addRecord(int account_num, char name[], char address[])
{
    int return_value = 1;
    struct record * previous_record;
    struct record * current_record;
    struct record * temp;
    current_record = this->start;
    previous_record = NULL;
    #ifdef debug
        std::cout << "\n/**************************************************************************";
        std::cout << "\n//ENTERING: addRecord";
        std::cout << "\n//Parameters";
        std::cout << "\n//Account Number: " << account_num;
        std::cout << "\n//Name: " << name;
        std::cout << "\n//Address: " << address;
        std::cout << "\n***************************************************************************\n";
    #else
        if(current_record == NULL)
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
            if(account_num > (current_record)->accountno)
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
                while(current_record != NULL && account_num < ((current_record)->accountno))
                {
                    temp = (current_record)->next;
                    previous_record = current_record; 
                    current_record = temp;                    
                } 
                if(current_record != NULL && account_num == (current_record)->accountno) /* accounting for the middle of the list and account already existing */
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
The code displayed above is my implementation of the linked list add method, demonstrating my understanding of pointers.

Click [here](https://github.com/jarrenseson/ICS-212-Bank-Database-Application.git) to see full code.
