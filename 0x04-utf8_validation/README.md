This is for the 0x04-utf8_validation project


### UTF-8 Validation Project Notes 

### 1. **Bitwise Operations in Python:**
   - **Basic Operators**:
     - **AND (`&`)**: Compares each bit of two numbers; if both bits are `1`, the result bit is `1`.
     - **OR (`|`)**: Compares bits; if either bit is `1`, the result bit is `1`.
     - **XOR (`^`)**: Compares bits; if the bits are different, the result bit is `1`.
     - **NOT (`~`)**: Flips all bits in the number.
   - **Shift Operations**:
     - **Left Shift (`<<`)**: Shifts bits to the left by a specified number of positions, effectively multiplying by powers of 2.
     - **Right Shift (`>>`)**: Shifts bits to the right, dividing by powers of 2.
   - **Applications**: Bitwise operations are often used in low-level data manipulation, optimizing data processing, and tasks like UTF-8 validation.

### 2. **UTF-8 Encoding Scheme:**
   - **Encoding Rules**: UTF-8 encodes characters as one to four bytes, depending on the character's Unicode value.
     - 1-byte characters: 0xxxxxxx
     - 2-byte characters: 110xxxxx 10xxxxxx
     - 3-byte characters: 1110xxxx 10xxxxxx 10xxxxxx
     - 4-byte characters: 11110xxx 10xxxxxx 10xxxxxx 10xxxxxx
   - **Validation**: Ensuring that each byte sequence adheres to these patterns is crucial in determining valid UTF-8 data.

### 3. **Data Representation:**
   - **Byte-Level Representation**: Manipulating data at the byte level involves using integer values that represent bits.
   - **Least Significant Bits (LSB)**: This approach focuses on the last bit(s) in a binary number, often used in encoding, encryption, and data validation.

### 4. **List Manipulation in Python:**
   - **Basics**: Accessing, modifying, and iterating through lists are essential for working with sequences of data, like byte arrays.
   - **List Comprehensions**: A concise way to create and modify lists, useful for filtering and processing byte data in encoding tasks.

### 5. **Boolean Logic:**
   - **Logical Operations**: Operations like `and`, `or`, `not`, and `xor` help make decisions based on multiple conditions.
   - **Application**: In UTF-8 validation, Boolean logic helps ensure that each byte follows the encoding rules for valid characters.

Together, these concepts provide a foundation for understanding data encoding and validation, particularly when applying bitwise and logical operations to UTF-8 encoding checks.