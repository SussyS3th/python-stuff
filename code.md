# September 23, 2025 - First real coding proiblem i solved in python

x = float(input("Enter value for x: "))
print("y =",str( 1 / (x+1 /(x+1/ (x+1))) / x))


# September 30 - Evaluate the end time of a period of time, given as a number of minutes. The start time is given as a pair of hours (0..23) and minutes (0..59).

hour = int(input("Starting time (hours): "))

mins = int(input("Starting time (minutes): "))

dura = int(input("Event duration (minutes): "))

TMS = hour * 60 + mins 

TME = TMS + dura

end_hour = (TME//60) % 24

end_minutes = TME % 60

print(end_hour, end_minutes, sep=":")
