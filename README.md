

**Intro to x86 Assembly Language**
****
*The Stack*

- LIFO data structure
- Is an array
- Stack pointer (register)  
  - esp is top point of the stack
  - ebp is base point of the stack
- Random access

```mov ebx, 123``` 		 ; ebx = 123

```mov eax, ebx``` 			 ; eax = ebx

```add ebx, ecx```    		 ; ebx += ecx

```sub ebx, edx ```  		 ; ebx -= edx

```mul ebx ```          		 ; eax *= ebx

```div edx    ```        		 ; eax /= edx

32-bit data registers: EAX, EBX, ECX, EDX.

A-Accumulator

B-Base

C-Counter

D-Data

**AX is the primary accumulator**; it is used in input/output and most arithmetic instructions. For example, in multiplication operation, one operand is stored in EAX or AX or AL register according to the size of the operand.

**BX is known as the base register**, as it could be used in indexed addressing.

**CX is known as the count register**, as the ECX, CX registers store the loop count in iterative operations.

**DX is known as the data register**. It is also used in input/output operations. It is also used with AX register along with DX for multiply and divide operations involving large values.


*Instruction pointer*

- EIP
- Location of execution
- Not like a register
- Changed by jump operations

```cmp``` -compare

```je``` -Jump if Equal

```jne```-Jump if Not Equal

```jg```-Jump if Greater

```jge```-Jump if Greater or Equal

```jl```-Jump if Less

```jle```-Jump if Less or Equal

```dec```-decrement

```int```-increment

db is 1 byte(8 bits)

dw is 2 bytes(16 bits)

dd is 4 bytes(32 bits)

```call```
- Pushes EIP to stack
- Preforms a jump


*Cheat-sheets*
https://www.cheatography.com/siniansung/cheat-sheets/linux-assembler/
