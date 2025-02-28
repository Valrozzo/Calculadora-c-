# Calculadora-c-
#include <iostream>

int main() {
    int num1, num2;
    char operador;

    std::cout << "Ingrese el primer numero: ";
    std::cin >> num1;
    std::cout << "Ingrese el operador( +, -, *, / ): ";
    std::cin >> operador;
    std::cout << "Ingrese el segundo numero: ";
    std::cin >> num2;

    int resultado;
    switch (operador) {
        case '+':
            resultado = num1 + num2;
            break;
        case '-':
            resultado = num1 - num2;
            break;
        case '*':
            resultado = num1 * num2;
            break;
        case '/':
            resultado = num1 / num2;
            break;
        default:
            std::cout << "Operador invalido" << std::endl;
            return 1;
    }
    std::cout << "Resultado: " << resultado << std::endl;
    return 0;
}
