# OOPTASK
void main() {
  //Student Objects
  Student student1 = Student('Alice', 20, 'A');
  Student student2 = Student('Ahmed', 30, 'A+');
  Student student3 = Student('Emad', 20, 'C');

  //Print Information
  student1.PrintInfo();
  student2.PrintInfo();
  student3.PrintInfo();

  //Update Grades
  student1.updateGrade('B');
  student1.updateGrade('A');
  student1.updateGrade('D');
}

// Define Class Student
class Student {
  //Variables
  String name;
  int age;
  String grade;

  //Constructour
  Student(this.name, this.age, this.grade);
  void PrintInfo() {
    print('Student name:$name');
    print(' Age:$age');
    print(' Grade:$grade');
  }

  void updateGrade(String newGrade) {
    grade = newGrade;
    print('$name :$grade'); //grade has been updated
  }
}
