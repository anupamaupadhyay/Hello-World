# Hello-World
My first repository 

largest  = None
smallest = None

while True:
    string = raw_input("Enter a number: ")

    if string == "done":
        break

    try:
        num = int(string)
    except ValueError:
        print "Invalid input"
        continue

    if largest is None or num > largest:
        largest = num

    if smallest is None or num < smallest:
        smallest = num
                
print "Maximum is", largest
print "Minimum is", smallest     
