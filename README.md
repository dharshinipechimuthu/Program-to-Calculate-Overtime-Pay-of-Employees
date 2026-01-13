# Program-to-Calculate-Overtime-Pay-of-Employees
def calculate_overtime(hours_worked):
    overtime_rate = 200
    normal_hours = 40

    if hours_worked > normal_hours:
        overtime_hours = hours_worked - normal_hours
        overtime_pay = overtime_hours * overtime_rate
    else:
        overtime_hours = 0
        overtime_pay = 0

    return overtime_hours, overtime_pay


# Main Program
emp_id = 201
emp_name = "Anita"
hours_worked = 46

overtime_hours, overtime_pay = calculate_overtime(hours_worked)

print("------ Overtime Pay Details ------")
print("Employee ID     :", emp_id)
print("Employee Name   :", emp_name)
print("Hours Worked    :", hours_worked)
print("Overtime Hours  :", overtime_hours)
print("Overtime Pay    : Rs.", overtime_pay)

OUTPUT:
------ Overtime Pay Details ------
Employee ID     : 201
Employee Name   : Anita
Hours Worked    : 46
Overtime Hours  : 6
Overtime Pay    : Rs. 1200

