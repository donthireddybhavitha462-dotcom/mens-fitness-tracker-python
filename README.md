# Men's Fitness & BMI Tracker

print("===== Men's Fitness & BMI Tracker =====")

name = input("Enter your name: ")
age = int(input("Enter your age: "))
height = float(input("Enter your height (in meters): "))
weight = float(input("Enter your weight (in kg): "))

bmi = weight / (height * height)

print("\n----- Fitness Report -----")
print("Name:", name)
print("Age:", age)
print("BMI:", round(bmi, 2))

if bmi < 18.5:
    print("Status: Underweight")
    print("Suggestion: Eat a balanced diet and do strength training.")
elif bmi < 25:
    print("Status: Healthy")
    print("Suggestion: Keep exercising and maintain your diet.")
elif bmi < 30:
    print("Status: Overweight")
    print("Suggestion: Exercise regularly and reduce junk food.")
else:
    print("Status: Obese")
    print("Suggestion: Consult a doctor and follow a healthy fitness plan.")

water = weight * 0.035
print("Recommended daily water intake:", round(water, 2), "liters")

print("\nStay healthy and stay strong! 💪")
