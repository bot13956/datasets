# datasets
Cleaned dataset that is ready to use for data analysis. Unit test grades for calculus-based introduction to physics course taught at Pittsburg State University, Pittsburg, Kansas. Unit test score ranges from 0 to 100, and grades are assigned according to the following scale: A (90 – 100); B (80 – 89), C (70 – 79), D (60 – 69); and F (0 – 59).

Here is the R-code that assigns letter grades:

# Program to assign letter grades to exam scores for a 100 points exam. Program takes as imput a vector containing scores in the range 0 to 100.

grade_function <-function(x){
  if(x > 100 | x < 0){
    print("Score if out of range. Please enter a score in range [0,100]")
  }
  else {
    if(x >=90 & x <= 100){
      "A"
    }
    else {
      if(x >=80 & x < 90){
        "B"
      }
      else {
        if(x >=70 & x < 80){
          "C"
        }
        else {
        if(x >=60 & x < 70){
          "D"
        }
          else {
            "F"
          }
        }
      }
    }
  }
}

