# Hurtado_Pablo_Gonzalo_SQL_Exercises


# 1. Exercise 1 (10 minutes) – 1 point /30

We must build all the tables constituting the following relational model:
- **Matter** (codemat, wording, coef)
- **Student** (numstud, name, firsname, dateofbirth, street, postalcod, city)
- **Test** (numtest, testdate, place codemat)
- **Notation** (numstud, numtest, score)

The underlined columns are to be declared in primary key. The bold columns are foreign keys.
For that, produce the text file, **CreateBD.txt**, containing the SQL orders allowing the creation of the database and the corresponding tables.
*Any reproduction, even partial, is prohibited without the written permission of HN INSTITUT.*

| Student | Test | Notation |
|---------|------|----------|
| numstud: int | numtest: int | score: float |
| name: char | testdate: Date | |
| firstname: char | place: char | |
| dateofbirth: Date | codemat: char | |
| street: char | wording: char | |
| postalcod: char | coef: float | |
| city: char | | |

# 2. Exercise 2 (50 minutes) – 1 point /30

Fill the tables with a dataset:
- It takes 7 students, including 3 in the same city and 3 whose names are: Dupont, Durand, and Martin. It also takes 2 cities whose name contains « LL ».
- There must be 3 subjects with a coefficient greater than or equal to 1 and at least one of which it is greater than 1.
- 30 marks are required, 18 of which are greater than or equal to 10, 2 equal to 20, and 2 tests with 2 different subjects and less than 6 students marked per test.
- 5 tests are required, 3 of which have the date between 1/1/2014 and 30/6/2014 (inclusive).
- You also need 2 subjects with more than one test.

For that, produce the text file, **InsertTB.txt**, containing the SQL orders allowing the creation of the records of each table.

# 3. Exercice 3 (20 minutes) – 5 points /30

Queries about Students:
- List of all students (1 point)
- List of all students, sorted in reverse alphabetical order (1 point)
- Last name and first name of students domiciled in Lyon (1 point)
- Last name, first name, and city of students whose city contains the string « LL » (1 point)
- First name of students with Dupont, Durand, or Martin names (1 point)

For that, produce the text file, **SelectEtu.txt**, containing the SQL orders allowing to answer the above request.

# 4. Exercice 4 (40 minutes) – 6 points /30

Queries about matter:
- Wording and coefficient (expressed as a percentage) of each subject (3 points)
- Sum of coefficients of all subjects (3 points)

To do this, produce the text file, **SelectMat.txt**, containing the SQL commands used to respond to the above request.

# 5. Exercice 5 (60 minutes) – 17 points /30

Queries on score and tests:
- Total number of tests (1 point)
- List of scores, specifying for each the name and first name of the student who obtained it (1 point)
- List of scores, specifying for each the name and first name of the student who obtained it and the wording of the matter concerned (1 point)
- List of scores greater than or equal to 10 (1 point)
- Last name and first name of the students who obtained at least a score equal to 20 (1 point)
- Average scores for each student (indicate name and first name) (1 point)
- List of tests whose date is between January 1 and June 30, 2014 (1 point)
- List of tests (number, date, and place) including the matter of the subject (1 point)
- Average scores for each student (indicate name and first name), ranked from best to worst (1 point)
- Average scores for matters (indicate the wording) comprising more than one test (4 points)
- Average of scores obtained in the tests (indicate the number of the test) where fewer than 6 students were rated (4 points)

To do this, produce the text file, **SelectNot.txt**, containing the SQL commands used to respond to the above request.
