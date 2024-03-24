# teapot.py

class Teapot:
    def __init__(self):
        self.water_level = 0
        self.tea_bags = 0
        self.is_boiled = False

    def add_water(self, amount):
        self.water_level += amount

    def add_tea_bags(self, count):
        self.tea_bags += count

    def boil(self):
        if self.water_level > 0 and self.tea_bags > 0:
            self.is_boiled = True
            print("Tea is ready!")
        else:
            print("Cannot make tea. Add water and tea bags first.")

    def pour_tea(self):
        if self.is_boiled:
            print("Pouring a cup of tea...")
            self.tea_bags -= 1
            self.water_level -= 1
        else:
            print("Tea is not ready yet. Boil the water first.")


def main():
    teapot = Teapot()

    while True:
        print("\n1. Add water")
        print("2. Add tea bags")
        print("3. Boil water")
        print("4. Pour tea")
        print("5. Exit")

        choice = input("Enter your choice: ")

        if choice == "1":
            amount = int(input("Enter the amount of water to add: "))
            teapot.add_water(amount)
            print("Water added successfully.")

        elif choice == "2":
            count = int(input("Enter the number of tea bags to add: "))
            teapot.add_tea_bags(count)
            print("Tea bags added successfully.")

        elif choice == "3":
            teapot.boil()

        elif choice == "4":
            teapot.pour_tea()

        elif choice == "5":
            print("Exiting...")
            break

        else:
            print("Invalid choice. Please enter a valid option.")


if __name__ == "__main__":
    main()
