# STM32 Bare-Metal Programming Projects (STM32F407G-DISC1)

This repository is a collection of **bare-metal STM32 projects** developed to gain a strong understanding of **register-level programming**, **GPIO control**, and **bitwise operations** without using HAL or high-level libraries.

All projects are implemented on the **STM32F407G-DISC1** development board.

---

## Hardware & Platform
- **Board:** STM32F407G-DISC1  
- **MCU:** STM32F407VG  
- **Programming Style:** Bare-metal (direct register access)  

---

## Projects Included

### 1. STM32_DigitalInputs_With_Debouncing
**Description:**  
Implemented digital input debouncing using a push button to avoid false triggers.

**Key Points:**
- Software debouncing logic
- Prevents false alerts (panic-button–like use case)
- GPIO input handling at register level

---

### 2. STM32_4x4_Keypad
**Description:**  
Interfaced a **4×4 matrix keypad** and printed keypad values by scanning rows and columns.

**Pin Configuration:**
- **Inputs:** PD8, PD9, PD10, PD11  
- **Outputs:** PD0, PD1, PD2, PD3  

**Key Points:**
- Matrix keypad scanning logic
- GPIO direction control
- Understanding pull-up/pull-down behavior

---

### 3. STM32-PinRead
**Description:**  
Read the status of **PA0** and controlled the on-board green LED (**PD12**) accordingly.

**Logic:**
- PA0 connected to GND → PD12 OFF  
- PA0 connected to VDD → PD12 ON  

**Key Points:**
- GPIO input reading
- Conditional output control

---

### 4. STM32-BoardGreenLedOn_WithoutBitwiseShiftOperator
**Description:**  
Turned ON/OFF the on-board green LED (**PD12**) **without using bitwise shift operators**.

**Key Points:**
- Direct register manipulation
- Manual bit masking
- Understanding raw register values

---

### 5. STM32-BoardGreenLedOn_WithBitwiseShiftOperator
**Description:**  
Controlled the on-board green LED (**PD12**) using **bitwise shift operators**.

**Key Points:**
- Cleaner and scalable GPIO control
- Use of bitwise operators (`<<`, `|`, `&`)

---

### 6. STM32-BoardGreenLedBlink
**Description:**  
Implemented blinking of the on-board green LED using bitwise operations.

**Key Points:**
- GPIO toggling
- Software delay loops
- Register-level timing control

---

## Learning Outcomes
- Strong understanding of STM32 GPIO registers
- Practical use of bitwise operations
- Clear distinction between:
  - With vs without bitwise operators
  - Bare-metal vs HAL-based programming
- Solid foundation for low-level firmware development

---

## Notes
- Each directory represents a **standalone project**
- Code is intentionally simple and readable
- No HAL or abstraction layers are used

---

## Author
**Deepanshu Tanwar**  
