# task1-flutter
task 1 flutter
problem1 
import 'dart:io';   
void main() {
 print('enetr your name :');
  String name = stdin.readLineSync();
  print('enter your age :');
  int age = int.tryParse(stdin.readLineSync());
 int yearsTobe100= 100 - age;
  print(yearsTobe100);
  print('Hello $name, you will turn 100 in $yearsTobe100 years.');
}

problem 2
import 'dart:io';   
void main() {
  print('enter any number:');
  int number=int.parse(stdin.readLineSync());
  if (number % 2 == 0) {
    print('The number is even');
  } else {
    print('The number is odd');
  }
}
problem 3
import 'dart:io';   
void main() {
  print('enter any number:');
  int number=int.parse(stdin.readLineSync());
  print('DIvisors of $number are:');
  for(int i=1;i<=number;i++){
    if(number%i==0){
      print(i);
    }
  }
}
problem 4
void main() {
  Map<String, int> cart = {'apple': 5, 'banana': 3, 'cherry': 7};
  int totalSum = 0;

  cart.forEach((key, value) {
    totalSum += value;
  });

  print('Total cart value: $totalSum');
}
problem 5
void main() {
  List<int> a = [5, 10, 15, 20, 25];
  List<int> result = firstAndLast(a);
  print(result); 
}
List<int> firstAndLast(List<int> numbers) {
  if (numbers.isEmpty) return [];
  if (numbers.length == 1) return [numbers[0]];
  return [numbers.first, numbers.last];
}

problem 6
List<int> findMaxMin(List<int> numbers) {
  if (numbers.isEmpty) return [];
  int max = numbers[0];
  int min = numbers[0];
  for (int i = 1; i < numbers.length; i++) {
    if (numbers[i] > max) {
      max = numbers[i];
    }
    if (numbers[i] < min) {
      min = numbers[i];
    }
  }
  return [max, min];
}

void main() {
  List<int> a = [5, 10, 15, 20, 25];
  List<int> result = findMaxMin(a);
  print('Max: ${result[0]}, Min: ${result[1]}');
}
 
    

    


 
    

