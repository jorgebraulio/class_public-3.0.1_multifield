Modification to Julien Lesgourgues code CLASS in its version 3.0.1 
(https://github.com/lesgourg/class_public/releases/tag/v3.0.1)
The modules modified were primordial.h, primordial.c and input.c

Replacing this 3 original files from the code version mentioned allows to work with multifield 
inflationary models having a separable (polynomial) field potential.

Input modifications allow to read potential parameters for several field from 
the input parameteres file (*.ini) at execution using for example the expresion

V_0_0=1.e-16\n
V_0_1=-1.e-17\n
V_0_2=7.e-17\n
V_0_3=0\n
V_0_4=0\n
V_1_0=1.e-16\n
V_1_1=-1.e-17\n
V_1_2=7.e-17\n
...\n
\n
Where the first index indicates the field number and the second the degree coefficient in the polynomial
The multifield option is selected with

Pk_ini_type = multifield

And the potential type (only polynomial supported for multifield) and field number with

potential = polynomial
n_of_fields =3



# class_public-3.0.1_multifield_primordial
