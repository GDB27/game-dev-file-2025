#include <iostream>
#include <string>

using namespace std;

// Class definition (Object)
class Student {
private:
    string name;
    int scores[5];  // Array to store 5 test scores

public:
    // Function to input data (including input)
    void inputData() {
        cout << "Enter student name: ";
        getline(cin, name);

        cout << "Enter 5 test scores:\n";
        for (int i = 0; i < 5; i++) {
            cout << "Score " << (i + 1) << ": ";
            cin >> scores[i];
        }
        cin.ignore();  // Clear newline after input
    }

    // Function to calculate average score (using loops)
    double calculateAverage() {
        int sum = 0;
        for (int i = 0; i < 5; i++) {
            sum += scores[i];
        }
        return sum / 5.0;
    }

    // Function to decide pass/fail (decision)
    void displayResult() {
        double avg = calculateAverage();
        cout << "\nStudent: " << name << endl;
        cout << "Average Score: " << avg << endl;

        if (avg >= 60) {  // Decision
            cout << "Result: Pass" << endl;
        } else {
            cout << "Result: Fail" << endl;
        }
    }
};

// Function outside class (additional function)
void eventTrigger() {
    cout << "\nEvent Triggered: Student score evaluation complete.\n";
}

int main() {
    Student s;

    s.inputData();   // Input data (input)
    s.displayResult();  // Output and decision

    eventTrigger();  // Event

    return 0;
}
