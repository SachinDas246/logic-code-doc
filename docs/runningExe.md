# Arguments for running Executable
./exe represents the generated executable file. This may vary depending on your OS.
## 1. Modes (-m <mode>)  
This allows the user to select how the program should run .  
```
./exe -m <mode>
```

### 1.1 Modes available

##### Direct input (d)
In this method, users can provide input directly as arguments. It requires -i to give the inputs.Note the number of inputs should match the number of arguments after -i. The order of the input is same as that of the input declaration in the workspace header.

```
./exe -m d -i 0 1 1     // there 3 inputs which are given 0,1,1.
```

##### Interactive mode (i)
This mode allows the user to provide the input signal at every step using tab (spacing) and return key. 

```
./exe -m i
```

#### File mode (f)
This mode allows the user to provide a csv file with inputs to generate an output file with results of the input file. You have to use -f to provide the input file.
```
./exe -m f -f <path to input file>
```
The input file should follow the following format:  

```
name:<name of component>
output_file_name:<name of the output file>
upp:7
totaltime:1400_m_s <time has not yet implemented, so skip for now>
interval:200_m_s    <time has not yet implemented>
end:<number of inputs>
<inputs at a first stage saperated by commas>
<inputs at a second stage saperated by commas>
<inputs at a third stage saperated by commas>
<inputs at a fourth stage saperated by commas>

```

A sample input.csv file for a full adder would look like:  
```
name:FullAdder
output_file_name:output.csv
upp:7
totaltime:1400_m_s
interval:200_m_s
end:3
0,0,0
0,0,1
0,1,0
0,1,1
1,0,0
1,0,1
1,1,0
1,1,1
```

If want to see the output while processing use "-p y" .  
```
./exe -m f -f <path to input file> -p y
``