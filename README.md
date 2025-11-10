# 🏙️ SmartCity

### Overview
**SmartCity** is a text-based Java game set in the bustling metropolis of **Smartopolis**. It was my final projcet for a Java programming course.  
Players explore different parts of the city, from luxurious hotels to busy airports, making spending decisions along the way.  

Each choice adds to a running **trip total**, giving you a lighthearted simulation of urban exploration and budgeting.  
The game is built entirely in **Java**, demonstrating **object-oriented programming**, **user input handling**, and **basic file persistence**.

---

### 🎮 Features
- **Multiple Destinations:**  
  Explore six unique city locations — **Hotel**, **Airport**, **Port**, **Train Station**, **Mall**, and **Restaurant**.
- **Dynamic Pricing System:**  
  Every decision (e.g., room type, seat class, meal choice) affects your total trip cost.
- **Interactive Console Menu:**  
  Navigate through locations using simple numbered options or type `q` to exit.
- **Spending Summary:**  
  The program automatically writes your total expenses to a file named `MoneySpent.txt`.
- **Replayability:**  
  Each session adds a new total to the file, so you can track multiple trips!

---

## 🧭 Locations & Choices

| Location | Options | Example Costs |
|:----------|:--------|:---------------|
| **Hotel** | Bed type (`King`, `Queen`, `Twin`) + Jacuzzi option | King Bed + Jacuzzi → **150.00** |
| **Airport** | Seat class (`First`, `Business`, `Economy`) + Meal option | Business + Meal → **275.00** |
| **Port** | Seat type (`Inside`, `Outside`) + Meal plan | Outside + Meal → **150.00** |
| **Train Station** | Seat type (`Public`, `Private`, `VIP`) | VIP Seat → **1000.00** |
| **Mall (Store)** | Category (`Clothing`, `Footwear`, `Tech`, `Toy`) + Brand name | Clothing → Nike, Gucci, Versace |
| **Restaurant** | Cuisine + Menu items | Italian → Pizza (**15.00**), Lasagna (**20.00**), Alfredo (**45.00**)|

---

## 💰 Price System

All destination classes (e.g., `Hotel`, `Airport`, `Restaurant`) **extend a base class `Service`** that tracks a `price` value.  
Each time a user makes a choice, the service updates its cost using:

--- 

## 🗂️ Project Structure

SmartCity.java        # Main program: menus, navigation, totals, file output
Airport.java          # Handles airport seat and meal options
Hotel.java            # Handles room type and jacuzzi options
Port.java             # Handles cruise options
Restaurant.java       # Handles cuisine and menu item selections
Store.java            # Handles mall store and category selection
TrainStation.java     # Handles train seat options
Service.java          # (Expected) Base class with price field + getters/setters

---

## 🕹️ Example Gameplay

Would you like to start an adventure in the beautiful city of Smartopolis (yes/no)?
yes

You arrive at the historical and beautiful train station of Smartopolis...

Where would you like to start your adventure/tour?
1 - Hotel
2 - Airport
3 - Port
4 - Mall
5 - Restaurant
q - Exit program
1

Very well! Let's go visit the hotel!

Which bed size would you like (King, Queen, Twin)?
King
Would you like a jacuzzi in your room?
yes
Bed Size: King
Jacuzzi: yes
Total Price: 150.0

Where would you like to go next?
1 - Hotel
2 - Airport
3 - Port
4 - Mall
5 - Restaurant
q - Exit program
q

Thanks for visiting Smartopolis!
Total amount of money spent during trip: 150.0
