print("NORTON'S THEOREM CALCULATION")

# Input values
V = float(input("Enter source voltage (V): "))
R1 = float(input("Enter resistance R1 (ohms): "))
R2 = float(input("Enter resistance R2 (ohms): "))
RL = float(input("Enter load resistance RL (ohms): "))

# Norton resistance
Rn = (R1 * R2) / (R1 + R2)

# Norton current (short circuit current)
In = V / R1

# Load current using Norton equivalent
IL = (In * Rn) / (Rn + RL)

# Load voltage
VL = IL * RL

# Display results
print("\n--- Norton Equivalent ---")
print("Norton Current (In) =", round(In, 2), "A")
print("Norton Resistance (Rn) =", round(Rn, 2), "ohms")
print("Load Current (IL) =", round(IL, 2), "A")
print("Load Voltage (VL) =", round(VL, 2), "V")# norton-s.py
A python program on nortons theorem
