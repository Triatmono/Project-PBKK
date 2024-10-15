
## PBKK Project

| Name           | NRP        | Kelas     |
| ---            | ---        | ----------|
| Muhammad Aulia Triatmono | 5025221069 | Pemrograman Berbasis Kerangka Kerja (IUP) |
| Radian Try Darmawan | 5025221097 | Pemrograman Berbasis Kerangka Kerja (IUP) |


## Laravel CRUD with Eloquent Relationships and Filament Integration
We named this project as SIMPELDA (Sistem Pengelolaan Data) which has the purpose of making data management easier. This project demonstrates how to create a CRUD (Create, Read, Update, Delete) application using Laravel's Eloquent relationships and Filament's admin panel features. The application manages two entities: departments `Jurusan` and students `Mahasiswa`, showcasing a One-to-Many relationship.

![Screenshot 2024-10-16 051006](https://github.com/user-attachments/assets/47f2109e-5818-4475-8395-57ca1d113150)

![Screenshot 2024-10-16 051159](https://github.com/user-attachments/assets/ee5208a4-747a-4d45-a4c4-2e604888961e)

![image](https://github.com/user-attachments/assets/69f2156d-9fdb-4c03-b504-8443ba6d48ff)

![Screenshot 2024-10-16 051221](https://github.com/user-attachments/assets/48d9d984-b977-435b-b617-3de8b4fa54c2)


### Key Features
- Eloquent Relationships
    - Models and Relationships: Two models are created: Jurusan (Department) and Mahasiswa (Student), with a One-to-Many relationship using Eloquent relationships in Laravel.
    - Foreign Key Setup: Establishes a foreign key relationship between the Jurusan and Mahasiswa tables to link student data to the respective department.
    - Relationship Implementation: Utilizes BelongsTo on the Mahasiswa model to connect to Jurusan, and HasMany on the Jurusan model to represent multiple students.

- Filament Form and Table Features
    - Form Creation: Explains how to create data input forms using the public static function form in Filament, which automatically generates an HTML form with Laravel's built-in validation.
    - Form Components: Uses TextInput and Select for form fields and displays the input data in tables using Filament's Table Columns.

- Using Select Relationship
    - Dropdown Implementation: Implements a select dropdown to choose a department in the student form, leveraging the relationship between the Jurusan and Mahasiswa models.
    - Data Display: Displays department names in the student table using Filament's Table::make() to show the relationship (jurusan->name) directly in the table.

- Filament Built-In Features
    - Search, Sort, and Pagination: Utilizes Filament's built-in features for data searching, sorting, and pagination without the need for additional code.
    - Data Filtering: Adds a filter to display students based on their department using Filament's SelectFilter feature.

- Data Customization and Validation
    - Data Validation: Explains how to add validation to models using Laravel's fillable property to control which columns can be mass-assigned, preventing unwanted data input.
    - Input Validation: Implements input validation rules, such as ensuring the student ID (NIM) is unique and restricting text input length.

- Demo Application
    - Project Overview: Builds a simple application that manages two entities: departments (Jurusan) and students (Mahasiswa), where each student is linked to a department via a foreign key.
    - Admin Interface: Leverages Filament to create an admin interface with minimal code, letting the framework handle the UI and CRUD logic automatically.
 
By implementing a One-to-Many relationship, data validation, and Filament's built-in functionalities like search, sorting, and filtering, this project should help on managing databases of students in each department.
