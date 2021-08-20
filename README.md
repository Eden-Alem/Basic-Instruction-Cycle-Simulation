# Basic Instruction Cycle Simulation

Team Members:
    1. Dagmawit Getachew - ATR/3566/11 - Section 1
    2. Eden Berhan Alem - ATR/3661/11 - Section 2
    3. Elshadai Kassu Tegegn - ATR/1831/11 - Section 2
    4. Mintesnot Bezabhi Lemu - ATR/9596/11 - Section 2
    5. Tewodros Mesfin Berahnu - ETR/1103/11 - Section 2


Screen recording of the simulation can be accessed with the link below:
https://drive.google.com/file/d/1NtLAVwPY4GUiicEsGBPh8fb5eEGBJBqR/view?usp=sharing


Rules to consider for proper implementation of this simulation:
- Can not use the same memory address pointer (300, 301, 302,....)
Eg- If 300 already exists with a value; can not use 300 in adding memory addresses through the form

- Can not use the same memory addresses (940, 941,....) for Opcodes 1(0001) and 2(0010): Both instructions load and add to memory respectively thus already include values that cannot be overwritten

- Can use the same memory addresses (940, 941,....) while using Opcode 5(0101): The instruction adds to memory from accumulator register (AC) basically allowing the alteration of already existing memory addresses with a value or even adding to a new memory address with no value

- The form inputs memory address pointer, opcode and memory address are required fields but the value to be stored on the memory address is not: Its not a requirement to add a value to be stored while using opcode 5 (since its instruction doesn't relate with the value)

- It requires that the input of the memory address pointer is above 300 (300 already exits as the minimum simulation example and memory address pointers can not be reused) and for the memory address that holds a value must be greater or equal to 940 (using opcode 5, we might reuse 940 memory address); to reduce input complications and human errors

- Other than numbers other inputs (like strings, characters) can not be added through the form in adding memory addresses

- 'remove last input' button removes the last input accepted through the form from a user and will never remove the basic example with 300 as the memory address pointer (as it is the base simulation implementer for it to serve its purpose as a simulator of the basic instruction cycle, the minimum we could go in witnessing the simluation)

