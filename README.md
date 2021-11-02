# S1_Jamela-Alcantara

    #include <iostream>
    #include <string>
    using namespace std;

    int main()
    {
        string name;
        int age;
        float p1, p2, sum, ave;

        cout << "Enter your full name: ";
        getline(cin, name);

        cout << "Enter your age: ";
        cin >> age;

        cout << "Enter two product prices: " << endl;
        cin >> p1; //first product price
        cin >> p2; //second product price

        if (p1 >= 0 && p2 <= 100) {
            double sum = (p1 + p2); //formula for sum
            double ave = (p1 + p2) / 5; //formula for average
            cout << "\nSum = " << sum << endl;
            cout << "Average = " << ave << endl;
            if (ave >= 70 && ave <= 100) //70-100
            {
                cout << "\nYou're spending quite a lot without saving anything.";
            }
            else if (ave >= 50 && ave <= 69) //50-69
            {
                cout << "\nMedium spending and saving, well done.";
            }
            else if (ave >= 49 && ave <= 10) //49-10
            {
                cout << "\nIt seems like you didn't spend much.";
            }
            else if (ave >= 0 && ave <= 9) //0-9
            {
                cout << "\nYou practically didn't buy anything at all.";
            }
        }
        return 0;
    }
