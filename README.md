#include<iostream>
using namespace std;

int main() {
    char startValue;
    char choiceAgain;
    float onlineshopping(void);
    
    startLevel: 
    cout << "Please press S to start shopping" << endl;
    start:
    cin >> startValue;
    if (startValue == 'S' || startValue == 's') {
      float totalAmount = onlineshopping();

      cout << "Total bill amount is " << totalAmount << endl;
      
      shopAgain: 
      cout << "Do you want to shop again, y or n" << endl;
      cin >> choiceAgain;
      if (choiceAgain == 'y' || choiceAgain == 'Y') {
        goto startLevel;
      }
      else if (choiceAgain == 'n' || choiceAgain == 'N') {
        cout << "Thanks for shopping, Have a great day ahead!" << endl;
      }
      else {
        cout << "You have entered a wrong value, Please try again." << endl;
        goto shopAgain;
      }
    }
    else {
        cout << "You have entered a wrong value, Please try again." << endl;
        goto start;
    }
}

float onlineshopping() {
    char choice;
    char item;
    float billamount = 0;
    int quantity;

    cout << "************Welcome to Nirvana**************" << endl;
    cout << "-----------Please follow the instructions------------" << endl;
    cout << "(1) Please enter 'M' to buy mobile phones" << endl;
    cout << "(2) Please enter 'L' to buy Laptops" << endl;
    cout << "(3) Please enter 's' to buy speakers" << endl;
    cout << "(4) Please enter 'H' to buy headsets" << endl;
    cout << "(5) Please enter 'e' to buy earbuds" << endl;
    cin >> choice;

    //************Mobiles**************//

    if (choice == 'm' || choice == 'M') {
        mobileLevel:
        cout << "Mobile details" << endl;
        cout << "(1) Apple => Price: Rs.65,000" << endl;
        cout << "(2) Samsung => Price: Rs.45,000" << endl;
        cout << "(3) Realme => Price: Rs.15,000" << endl;
        cout << "(4) Xiaomi => Price: Rs.20,000" << endl;S
        cout << "(5) Oppo => Price: Rs.25,000" << endl;
        cout << "(6) Vivo => Price: Rs.19,000" << endl;
        cout << "Please enter your choice" << endl;
        cin >> item;
        if (item == '1') {
            cout << "Enter quantity" << endl;
            cin >> quantity;
            billamount += quantity * 65000;
        }
        else if (item == '2') {
            cout << "Enter quantity" << endl;
            cin >> quantity;
            billamount += quantity * 45000;
        }
        else if (item == '3') {
            cout << "Enter quantity" << endl;
            cin >> quantity;
            billamount += quantity * 15000;
        }
        else if (item == '4') {
            cout << "Enter quantity" << endl;
            cin >> quantity;
            billamount += quantity * 20000;
        }
        else if (item == '5') {
            cout << "Enter quantity" << endl;
            cin >> quantity;
            billamount += quantity * 25000;
        }
        else if (item == '6') {
            cout << "Enter quantity" << endl;
            cin >> quantity;
            billamount += quantity * 19000;
        }
        else {
            cout << "You have entered a wrong value, Please try again." << endl;
            goto mobileLevel;
        }
    }

    //************Laptops**************//

    else if (choice == 'l' || choice == 'L') {
        laptopLevel:
        cout << "Laptop details" << endl;
        cout << "(1) Asus => Price: Rs.60,000" << endl;
        cout << "(2) MacBook => Price: Rs.1,20,000" << endl;
        cout << "(3) Dell => Price: Rs.70,000" << endl;
        cout << "(4) Lenovo => Price: Rs.79,000" << endl;
        cout << "(5) Samsung => Price: Rs.44,000" << endl;
        cout << "(6) HP => Price: Rs.59,000" << endl;
        cout << "Please enter your choice" << endl;
        cin >> item;
        if (item == '1') {
            cout << "Enter quantity" << endl;
            cin >> quantity;
            billamount += quantity * 60000;
        }
        else if (item == '2') {
            cout << "Enter quantity" << endl;
            cin >> quantity;
            billamount += quantity * 120000;
        }
        else if (item == '3') {
            cout << "Enter quantity" << endl;
            cin >> quantity;
            billamount += quantity * 70000;
        }
        else if (item == '4') {
            cout << "Enter quantity" << endl;
            cin >> quantity;
            billamount += quantity * 79000;
        }
        else if (item == '5') {
            cout << "Enter quantity" << endl;
            cin >> quantity;
            billamount += quantity * 44000;
        }
        else if (item == '6') {
            cout << "Enter quantity" << endl;
            cin >> quantity;
            billamount += quantity * 59000;
        }
        else {
            cout << "You have entered a wrong value, Please try again." << endl;
            goto laptopLevel;
        }
    }

    //************Speakers**************//

    else if (choice == 's' || choice == 'S') {
        speakerLevel:
        cout << "Speaker details" << endl;
        cout << "(1) Boat => Price: Rs.6000" << endl;
        cout << "(2) Samsung => Price: Rs.1200" << endl;
        cout << "(3) JBL => Price: Rs.7000" << endl;
        cout << "(4) Sony => Price: Rs.1700" << endl;
        cout << "(5) Truke => Price: Rs.4000" << endl;
        cout << "(6) Saregama => Price: Rs.5000" << endl;
        cout << "Please enter your choice" << endl;
        cin >> item;
        if (item == '1') {
            cout << "Enter quantity" << endl;
            cin >> quantity;
            billamount += quantity * 6000;
        }
        else if (item == '2') {
            cout << "Enter quantity" << endl;
            cin >> quantity;
            billamount += quantity * 1200;
        }
        else if (item == '3') {
            cout << "Enter quantity" << endl;
            cin >> quantity;
            billamount += quantity * 7000;
        }
        else if (item == '4') {
            cout << "Enter quantity" << endl;
            cin >> quantity;
            billamount += quantity * 1700;
        }
        else if (item == '5') {
            cout << "Enter quantity" << endl;
            cin >> quantity;
            billamount += quantity * 4000;
        }
        else if (item == '6') {
            cout << "Enter quantity" << endl;
            cin >> quantity;
            billamount += quantity * 5000;
        }
        else {
            cout << "You have entered a wrong value, Please try again." << endl;
            goto speakerLevel;
        }
    }

    //************Headsets**************//

    else if (choice == 'h' || choice == 'H') {
        headsetsLevel:
        cout << "Headsets details" << endl;
        cout << "(1) Boat Rockerz => Price: Rs.600" << endl;
        cout << "(2) Noise => Price: Rs.800" << endl;
        cout << "(3) Apple => Price: Rs.6500" << endl;
        cout << "(4) JBL => Price: Rs.700" << endl;
        cout << "(5) Sony => Price: Rs.1200" << endl;
        cout << "(6) Zebronics => Price: Rs.5500" << endl;
        cout << "Please enter your choice" << endl;
        cin >> item;
        if (item == '1') {
            cout << "Enter quantity" << endl;
            cin >> quantity;
            billamount += quantity * 600;
        }
        else if (item == '2') {
            cout << "Enter quantity" << endl;
            cin >> quantity;
            billamount += quantity * 800;
        }
        else if (item == '3') {
            cout << "Enter quantity" << endl;
            cin >> quantity;
            billamount += quantity * 6500;
        }
        else if (item == '4') {
            cout << "Enter quantity" << endl;
            cin >> quantity;
            billamount += quantity * 700;
        }
        else if (item == '5') {
            cout << "Enter quantity" << endl;
            cin >> quantity;
            billamount += quantity * 1200;
        }
        else if (item == '6') {
            cout << "Enter quantity" << endl;
            cin >> quantity;
            billamount += quantity * 5500;
        }
        else {
            cout << "You have entered a wrong value, Please try again." << endl;
            goto headsetsLevel;
        }
    }

    //************Earbuds**************//

    else if (choice == 'e' || choice == 'E') {
        earbudsLevel:
        cout << "Earbuds details" << endl;
        cout << "(1) Boat => Price: Rs.1200" << endl;
        cout << "(2) Noise => Price: Rs.2500" << endl;
        cout << "(3) Boult => Price: Rs.1500" << endl;
        cout << "(4) Realme => Price: Rs.3500" << endl;
        cout << "(5) Sony => Price: Rs.2000" << endl;
        cout << "(6) JBL => Price: Rs.4500" << endl;
        cout << "Please enter your choice" << endl;
        cin >> item;
        if (item == '1') {
            cout << "Enter quantity" << endl;
            cin >> quantity;
            billamount += quantity * 1200;
        }
        else if (item == '2') {
            cout << "Enter quantity" << endl;
            cin >> quantity;
            billamount += quantity * 2500;
        }
        else if (item == '3') {
            cout << "Enter quantity" << endl;
            cin >> quantity;
            billamount += quantity * 1500;
        }
        else if (item == '4') {
            cout << "Enter quantity" << endl;
            cin >> quantity;
            billamount += quantity * 3500;
        }
        else if (item == '5') {
            cout << "Enter quantity" << endl;
            cin >> quantity;
            billamount += quantity * 2000;
        }
        else if (item == '6') {
            cout << "Enter quantity" << endl;
            cin >> quantity;
            billamount += quantity * 4500;
        }
        else {
            cout << "You have entered a wrong value, Please try again." << endl;
            goto earbudsLevel;
        }
    }

    return billamount;
}
