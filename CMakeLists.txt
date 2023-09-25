#include <iostream>
#include <numcpp/numcpp.h>

using namespace std;

int main() {
  // Create a NumPy array from the given numbers.
  nc::array<int> numbers = {144, 131, 105, 153, 125, 155, 167, 144};

  // Calculate the mean.
  double mean = nc::mean(numbers);

  // Calculate the median.
  double median = nc::median(numbers);

  // Calculate the mode.
  nc::array<int> mode = nc::mode(numbers, axis=0);

  // Calculate the standard deviation.
  double stddev = nc::std(numbers);

  // Print the results.
  cout << "Mean: " << mean << endl;
  cout << "Median: " << median << endl;
  cout << "Mode: " << mode << endl;
  cout << "Standard deviation: " << stddev << endl;

  return 0;
}

