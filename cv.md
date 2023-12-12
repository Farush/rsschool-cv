
# Farkhad Sibgatullin

***

![my image](img/photo_small.jpeg "My photo")

## Contact information:
* Phone: +381 63 885 9102
*  Whatsapp: +90 531 010 6274
* e-mail: farusha.q@gmail.com
* github: https://github.com/Farush
* telegram: @farusha
* discord: Farhad  Sibgatullin (@farush)

## Summary:
Junior level software engineer. Most recent experience
includes programming in Python and database management. Constantly
expanding into new areas of knowledge and improving current skills.

## Skills
Studying IT on geekbrains platfom. Gained basic skills in these:
* git, github can be found [here](https://github.com/Farush)
* python. 
* html, css.
* MySQL. 
* fastAPI, Docker stuying at the moment. 
***

## Examples of code:

``` 

class Matrix:
    def __init__(self, matrix_lines):
        self.matrix = matrix_lines
        self.columns = len(self.matrix[0])
        self.lines = len(self.matrix)
        for line in self.matrix:
            if len(line) != self.columns:
                raise Exception ('All the lines in Matrix should have the same length') # the better way is to
                # find the longest line and add zeros to the shorter ones
        self.dimension = [self.lines, self.columns] # needed to make matrices' dimensions comparable
        #print(self.matrix[0][0])

    def __add__(self, other):
        new_matrix = []
        new_line = []
        if self.dimension != other.dimension: # We refuse to add matrices with different dimensions.
            # The better way is to fill missing lines and columns with zeros which demands writing a more complex
            # code
            raise ArithmeticError('Matrices have different dimensions')
        else:
            for line in range(len(self.matrix)):
                for column in range(len(self.matrix[0])):
                    new_line.append(self.matrix[line][column] + other.matrix[line][column])
                new_matrix.append(new_line)
                new_line = []

            return Matrix(new_matrix)

    def __str__(self):
        matrix_square = ''
        for line in range(len(self.matrix)):
            for column in range(len(self.matrix[0])):
                matrix_square = matrix_square + f'|  {self.matrix[line][column]}  '
            matrix_square = matrix_square + '|\n'
        return matrix_square

    def __mul__(self, multiplier): # just because I can
        new_matrix = []
        new_line = []
        for line in range(len(self.matrix)):
            for column in range(len(self.matrix[0])):
                new_line.append(self.matrix[line][column] * multiplier)
            new_matrix.append(new_line)
            new_line = []

        return Matrix(new_matrix)


matr1 = Matrix([[1, 2, 3], [2, 5, 8], [65, 67894, 0]])

matr2 = Matrix([[2, 5, 9], [789, -17, -36], [0, 0, 56]])

matr3 = matr1 + matr2

matr4 = matr1 + matr2 + matr3 + matr1

matr5 = matr1 * 1

print(matr5 * 15.7)

print(type(matr3))

print(matr3)
print(matr4)


```

## Experience:

* python: examples of homeworks I did can be found [here](https://github.com/Farush/HomeworkPython)
* html, css: Adaptive homework project can be found [here](https://farush.github.io/html-css-study-project/index.html)
* MySQL: [MySQL database project](https://github.com/Farush/MySQL-Study-Project)
* FastAPI: [here](https://github.com/Farush/Library_fastAPI)

## Education:

- School: Tatar-american regional institute. 
- Field of study: Linguistics, cross-cultural communication.
- Degree: bachelor

## Languages:
1. English. B2/C1. 
2. Russian
3. Turkish B2.
4. Tatar native.

## About me:
Used to work as a rope access technician for more than ten years, which included installing cellular base stations and configuring equipement by given instructions. I also worked as a system administrator in an orphanage up to 2011. Back in Kazan (Republic of Tatarstan which is within Russia) me and my friend we ran a music studio. Examples of work can be found [here](https://www.youtube.com/results?search_query=%D0%BF%D0%BE%D0%BF%D1%80%D1%8B%D0%B3%D1%83%D0%BD+%D0%B8+%D0%B3%D0%B2%D0%BE%D0%B7%D0%B4%D0%B8).
