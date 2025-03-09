## 2. Library Bookly

A library called Bookly keeps track of books and members who borrow them. Each book has a title, author, and ISBN number. Each member has a membership ID, name, and contact information. A member can borrow multiple books, but each book can be borrowed by only one member at a time.

`a)` Identify the entities and attributes for each entity.

#### Book

- ISBN
- title
- author

#### Member

- first_name
- last_name
- membership_id
- phone
- adress
- email

#### Borrowing

- borrowing_id
- ISBN
- membership_id
- return_date
- borrowing_date

`b)` Determine the relationship between member and books.

- A member can have zero, one or several Borrowings
- A Borrowing can be made by one and only one Member
- A Borrowing is linked to one and only one Book
- A Book can be in zero, one or more Borrowings

`c)` Draw a conceptual ERD using crow foots notation.

#### Initial conceptual ERD

<img src="../assets/bookly_0.png" width =400>

<br>

#### Replaced many-to-many with a bridge table

<img src="../assets/bookly_1.png" width =400>
