# JIRA_CHQ1
Automated Chemistry activity: CHQ 1
def parse_input(input_string):
    reactants = input_string.split("+")
    return reactants

def predict_products(reactants):
    if "H2" in reactants and "o2" in reactants:
        return ["H2O"]
    return []
   
def balance_equation(reactants,products):
    return f"{reactants} -> {products}"

def main(input_string):
    reactants = parse_input(input_string)
    products = predict_products(reactants)
    balanced_equation = balance_equation(reactants,products)
    return balanced_equation

input_string = "H2 + O2"
result = main(input_string)
print(result)
    
