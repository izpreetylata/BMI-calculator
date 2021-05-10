#BMI calculator

height = input("enter your height in m: ")
weight = input("enter your weight in kg: ")
weight_as_int = int(weight)
height_as_float = float(height)
#using the exponent operator
bmi = weight_as_int/height_as_float**2
#or using multiplication and PEMDAS
bmi = weight_as_int / (height_as_float*height_as_float)
bmi_as_int = int(bmi)

print(bmi_as_int)
if bmi_as_int <= 18:
  print(f"Your BMI is {bmi_as_int} , you are underweight")
elif bmi_as_int <= 22 :
  print(f"Your BMI is {bmi_as_int} , you have a normal weight.")
elif bmi_as_int <= 28 :
  print(f"Your BMI is {bmi_as_int}, you are slightly overweight.")
elif bmi_as_int <= 33 :
  print(f"Your BMI is {bmi_as_int}, you are obese.")

else :
  print(f"Your BMI is {bmi_as_int}, you are clinically obese.")

