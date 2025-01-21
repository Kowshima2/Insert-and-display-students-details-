# Insert-and-display-students-details-
import java.util.Scanner;

class Student {
    
    String name;
    int rollNumber;
    double mark;
    Student(String name, int rollNumber, double marks) {
        this.name = name;
        this.rollNumber = rollNumber;
        this.marks = marks;
    }

 
    void displayDetails() {
        System.out.println("Student Name: " + name);
        System.out.println("Roll Number: " + rollNumber);
        System.out.println("Marks: " + marks);
    }
}

public class StudentDetails {
    public static void main(String[] args) {
   
        Scanner scanner = new Scanner(System.in);

  
        System.out.print("Enter student's name: ");
        String name = scanner.nextLine();

        System.out.print("Enter student's roll number: ");
        int rollNumber = scanner.nextInt();

        System.out.print("Enter student's marks: ");
        double marks = scanner.nextDouble();


        Student student = new Student(name, rollNumber, marks);

    
        System.out.println("\nStudent Details:");
        student.displayDetails();

       
        scanner.close();
    }
}
 Output 
Enter student's name: John
Enter student's roll number: 102
Enter student's marks: 90.5

Student Details:
Student Name: John
Roll Number: 102
Marks: 90.5
