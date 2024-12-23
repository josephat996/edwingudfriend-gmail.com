

    cout << "Simple Calculator\n";
    cout << "Enter first number: ";
    cin >> num1;

    cout << "Enter an operator (+, -, *, /): ";
    cin >> operation;

    cout << "Enter second number: ";
    cin >> num2;

    switch (operation) {
        case '+':
            cout << "Result: " << (num1 + num2) << endl;
            break;
        case '-':
            cout << "Result: " << (num1 - num2) << endl;
            break;
        case '*':
            cout << "Result: " << (num1 * num2) << endl;
            break;
        case '/':
            if (num2 != 0) {
                cout << "Result: " << (num1 / num2) << endl;
            } else {
                cout << "Error: Division by zero is not allowed.\n";
            }
            break;
        default:
            cout << "Error: Invalid operator.\n";
            break;
    }

    return 0;
}
