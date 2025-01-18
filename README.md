# multisim-amplifiers-and-simple-digital-circuits

Operational amplifiers

a. Classic integrated operational amplifier
Build a simple amplifier circuit using a classic integrated operational amplifier (type 741) operating in a phase-inverting amplifier circuit

Drawing of the circuit in the file

Measure all the basic parameters of the above amplifier, i.e. voltage gain (total and individual gain stages), input and output impedance.

b. Comparator

Build a comparator circuit according to the drawing below and check its operation when forced by sawtooth pulses.

Drawing of the circuit in the file

Simple digital circuits

1. Check the truth tables for the OR logical sum, AND logical product, modulo XOR sum, using the example below, which was of course compiled to show the operation of the NOT inverter.
Drawing of the circuit in the file

2. Using the Karnaugh method, design a fragment of a BCD binary code decoder to a seven-segment code decoding segment "a". Check the operation of the designed circuit.
Truth table in table file.

All Boolean expressions can be represented in two standard forms: as Sum Of Products (SOP) or as Product Of Sums (POS).

To determine the standard SOP of an expression presented in a truth table, one must list the values ​​of all binary variables for which the output is one.

This is because the standard product term is equal to one only for one combination of input variable values.

For example, the product of terms is equal to 1 when D=0, C=0, B=1, A=0 as shown in the above table according to the transformation below.

To define the expression defining segment a, the standard SOP will be described as follows:

Let us note that the above SOP notation also includes the terms that appear in the truth table as X, i.e. as product or summation terms, which in our case should be seen as 
product terms because this will result in the maximum minimization of the expression, i.e. the simplest implementation of the BCD code decoder to a seven-segment one.

This expression can be directly implemented in a system, although it is better to achieve the maximum minimization of this notation.
The Karnaugh table method helps in this.

The first stage of the method is to create a table with the number of fields equal to the number of variables in the SOP expression.

In the case under consideration, it will be a 4x4 table with sixteen fields.
To describe the coordinates of the table, it is absolutely necessary to use the Grey code as shown in the example below.
Next, the table should be filled with ones for the terms visible in the previous expression.

For the example under consideration, the filled table will look as follows:
(table file table)

The simplified SOP expression will be the sum of four products (that is how many fields are circled in the table). Each product created associated with a specific field will be the product of 
variables that do not change their value in the field. Segment a will be controlled by the following simplified SOP function.

Drawing of the system in the file

Prepare a report on the completion of all points of this exercise

Each report should be provided with the following heading and include:
a detailed description of all completed exercise points along with your own conclusions regarding the work performed
