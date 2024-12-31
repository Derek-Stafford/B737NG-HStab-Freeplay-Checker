from tabulate import tabulate

# Cosmetic
black = '\033[0;30m'
bold = '\033[1m'
cyan = '\033[96m'
end = '\033[0m'
green = '\033[92m'
italic = '\033[3m'
red = '\033[31m'

# Input Values
D1 = float(input(italic+bold+"D1 = "+end))
D2 = float(input(italic+bold+"D2 = "+end))
D3 = float(input(italic+bold+"D3 = "+end))
# Calculating the total freeplay then storing and displaying the reault inside a table
H = (1.25*D3)+((D1+D2)/2)
equation = [
		[italic+bold+"H = (1.25*D3)+((D1 + D2)/2)"+end, bold+str(H)+end]
]
head_1 = [black+italic+bold+"Formula", "Value"+end]
print(tabulate(equation, headers=head_1, tablefmt="grid"))

# Threshold Messages
def check_value(name, value, threshold):
		if value > threshold:
				return bold+italic+red+"Failed"+end
		else:
				return italic+green+"Passed"+end
 
# Check Values against Threshold Conditions, then storing and displaying the results inside a table
head_2 = [black+italic+bold+"Variable","Value", "Limit", "Result"+end]

results = [
		[italic+bold+cyan+"D1"+end, f"{D1:.4f}", 0.066, bold+check_value("D1", D1, 0.066)],
		[italic+bold+cyan+"D2"+end, f"{D2:.4f}", 0.066, bold+ check_value("D2", D2, 0.066)],
		[italic+bold+cyan+"D3"+end, f"{D3:.4f}", 0.056, bold+ check_value("D3", D3, 0.056)],
	[italic+bold+cyan+"H"+end, f"{H:.4f}", 0.078, bold+check_value("H", H, 0.078)]
]

print(tabulate(results, headers=head_2, tablefmt="grid"))
