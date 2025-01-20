# program-using-class-based-on-percentage-increase-
class Salary {
    double salary;
    void calculateSalary(double percentageIncrease) {
        salary = salary + (salary * percentageIncrease / 100);
    }
    void setSalary(double oldSalary) {
        salary = oldSalary;
    }
    void displaySalary() {
        System.out.println("Updated Salary: " + salary);
    }
}
public class PercentageIncreaseExample {
    public static void main(String[] args) {
        Salary salary = new Salary();
        salary.setSalary(50000);
        salary.calculateSalary(10);
        salary.displaySalary();
    }
}
