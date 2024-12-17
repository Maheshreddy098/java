import java.util.Scanner;
class Student {
    String name;
    int age;
    double marks;
    public Student(String name, int age, double marks) {
        this.name = name;
        this.age = age;
        this.marks = marks;
    }
    public void displayStudentDetails() {
        System.out.println("Student Name: " + name);
        System.out.println("Age: " + age);
        System.out.println("Marks: " + marks);
    }
}
public class Main {
    public static void main(String[] args)
        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter student name: ");
        String name = scanner.nextLine();
        System.out.print("Enter student age: ");
        int age = scanner.nextInt();
        System.out.print("Enter student marks: ");
        double marks = scanner.nextDouble();
        Student student = new Student(name, age, marks);
        student.displayStudentDetails();
        scanner.close();
    }
}
