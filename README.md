The application represents functionality for the creation and management of water vending machines.

# Water Vending Machine — Lab 5 (MSTest)

## Project Overview
This lab adds **unit testing with MSTest** for the Water Vending Machine class
implemented in Lab-4.

---

## Test Project
- An **MSTest project** is added to the same solution
- Test class name matches the tested class:
  - `WaterVendingMachineTests`

---

## Tested Functionality

### Instance Methods
- `PutMoney(decimal cash)`
- `TakeWater()`
- `Refill()`
- `Refill(int liters)`
- `WithdrawCash()`

### Static Methods
- `CalculateWaterByPrice(decimal cash)`
- `Parse(string s)`
- `TryParse(string s, out WaterVendingMachine machine)`

---

## Property Tests
Setter logic is tested for several properties:
- `WaterCapacityLiters`
- `WaterLeftLiters`
- `OperatorName`
- `Phone`

Invalid values are verified to trigger validation logic.

---

## Constructors
- Default constructor
- Constructor with full manual data
- Constructor with partial data (`WaterCapacityLiters` only)

---

## Test Execution
- All test methods are executed using MSTest
- Failed tests are fixed by adjusting the production code
- Final result: **all tests pass successfully**

---

## Menu Coverage
All application menu options are covered indirectly through unit tests:
- Object creation
- State changes
- Static logic execution
