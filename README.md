# Portfolio 3: Functions
## Title: Molar Concentration Calculator

### Description:
#### This program calculates the molarity of a
#### chemical solution using mass, molar mass,
#### and volume.

### Formula:
#### moles = mass / molar_mass
#### molarity = moles / volume

### Function to compute number of moles
```python
def compute_moles(mass, molar_mass):
    moles = mass / molar_mass
    return moles
```

### Function to compute molarity
```python
def compute_molarity(moles, volume):
    molarity = moles / volume
    return molarity
```

### Function to determine concentration level
```python
def get_concentration(molarity):
    if molarity >= 1:
        return "Concentrated Solution"
    else:
        return "Dilute Solution"
```

### Main program
```python
print("Solution Concentration Calculator")
```
```python
compound = input("Enter compound name: ")
mass = float(input("Enter solute mass (g): "))
molar_mass = float(input("Enter molar mass (g/mol): "))
volume = float(input("Enter solution volume (L): "))
```

### Function calls
```python
moles = compute_moles(mass, molar_mass)
molarity = compute_molarity(moles, volume)
remark = get_concentration(molarity)
```

### Display results
```python
print("RESULTS")
print("Compound:", compound)
print("Moles:", moles)
print("Molarity:", molarity, "M")
print("Remarks:", remark)
```