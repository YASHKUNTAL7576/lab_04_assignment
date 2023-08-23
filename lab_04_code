flight_table = {
    "AI161E90": ["BLR", "BOM", 5600],
    "BR161F91": ["BOM", "BBI", 6750],
    "AI161F99": ["BBI", "BLR", 8210],
    "VS171E20": ["JLR", "BBI", 5500],
    "AS171G30": ["HYD", "JLR", 4400],
    "AI131F49": ["HYD", "BOM", 3499]
}

def search_flights():
    print("Please select a search parameter:")
    print("1. Flights for a particular City")
    print("2. Flights From a city")
    print("3. Flights between two given cities")
    
    choice = int(input("Enter your choice: "))
    
    if choice == 1:
        city = input("Enter the city name: ")
        flights = [k for k, v in flight_table.items() if city in v]
        if flights:
            print(f"Flights for {city}:")
            for flight in flights:
                print(flight)
        else:
            print(f"No flights found for {city}")
            
    elif choice == 2:
        city = input("Enter the city name: ")
        flights = [k for k, v in flight_table.items() if v[0] == city]
        if flights:
            print(f"Flights from {city}:")
            for flight in flights:
                print(flight)
        else:
            print(f"No flights found from {city}")
            
    elif choice == 3:
        city1 = input("Enter the first city name: ")
        city2 = input("Enter the second city name: ")
        flights = [k for k, v in flight_table.items() if v[0] == city1 and v[1] == city2]
        if flights:
            print(f"Flights between {city1} and {city2}:")
            for flight in flights:
                print(flight)
        else:
            print(f"No flights found between {city1} and {city2}")
            
search_flights()

