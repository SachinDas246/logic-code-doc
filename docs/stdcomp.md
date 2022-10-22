# Components   
This gives you information about the components in the stdcomp library.  

## 1. Not gate (Inverter)
This produces the inverted state of the input. 


|    Gate      | Inputs       | Outputs       |
| ------------ | ------------ | ------------- |
| Not          |    a         |     o         |



## 2. Controlled Inverter   

This act as an Inverter when the control pin is high else low.  

|         Gate | Inputs       | Outputs       |
| ------------ | ------------ | ------------- |
| CtrlInverter | a, c(control)|     o         |


## 3. Buffer  
This component reproduces the input at the output.  

|    Gate      | Inputs       | Outputs       |
| ------------ | ------------ | ------------- |
| Buffer       |    a         |     o         |



## 4. Controlled Buffer  
This acts as a Buffer when the control pin is high else low.

|         Gate | Inputs       | Outputs       |
| ------------ | ------------ | ------------- |
| CtrlBuffer |  a, c(control) |     o         |



## 5. And
This produces high only when every input is high.

|         Gate | Inputs       | Outputs       |
| ------------ | ------------ | ------------- |
| And2         |    a,b       |     o         |
| And3         |    a,b,c     |     o         |
| And4         |    a,b,c,d   |     o         |


## 6. Or

This produces high signal when at least one of the input is high.  

|         Gate | Inputs       | Outputs       |
| ------------ | ------------ | ------------- |
| Or2         |    a,b       |     o         |
| Or3         |    a,b,c     |     o         |
| Or4         |    a,b,c,d   |     o         |


## 7. Nand  
It produces output which is complement to that of an AND gate.    

|         Gate | Inputs       | Outputs       |
| ------------ | ------------ | ------------- |
| Nand2         |    a,b       |     o         |
| Nand3         |    a,b,c     |     o         |
| Nand4         |    a,b,c,d   |     o         |


## 8. Nor  
It produces output which is complement to that of an OR gate.    

|         Gate | Inputs       | Outputs       |
| ------------ | ------------ | ------------- |
| Nor2         |    a,b       |     o         |
| Nor3         |    a,b,c     |     o         |
| Nor4         |    a,b,c,d   |     o         |



## 9. Xor
The output of an XOR gate is high only when odd number of inputs are high  

|         Gate | Inputs       | Outputs       |
| ------------ | ------------ | ------------- |
| Xor2         |    a,b       |     o         |
| Xor3         |    a,b,c     |     o         |
| Xor4         |    a,b,c,d   |     o         |


## 10. Xnor
The output of an XNOR gate is high only when even number of inputs are high  

|         Gate | Inputs       | Outputs       |
| ------------ | ------------ | ------------- |
| Xnor2         |    a,b       |     o         |
| Xnor3         |    a,b,c     |     o         |
| Xnor4         |    a,b,c,d   |     o         |


## 11. Positive Trigger  
The output of this module is high when input changes from low to high

|    Gate      | Inputs       | Outputs       |
| ------------ | ------------ | ------------- |
| PosTrig      |    i         |     o         |

## 11. Negative Trigger  
The output of this module is high when input changes from high to low.

|    Gate      | Inputs       | Outputs       |
| ------------ | ------------ | ------------- |
| NegTrig      |    i         |     o         |


