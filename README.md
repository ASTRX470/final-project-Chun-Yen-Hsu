# final-project-Chun-Yen-Hsu
This final project use athena++ code to finish the work.

The public version of the athena++ code can be found: https://github.com/PrincetonUniversity/athena/wiki 

The only thing I add is the Hall effect in the magnetic field diffusion term, where the modifications are at src/field/field_diffusion.

The sub function called FieldDiffusion::HallEMF in the "diffusivity.cpp"

There are a little modifications in the "field_diffusion.cpp"

To compile the problems, the module should include the magnetic field.

Please make sure you have included the "-b" when you compile the code.

Run the "configure.py" with -b, to include the magnetic field in the code.

# first test: whistler wave
For this final project, I test the whistler wave, and the corresponding problem generator (pgen) is named as "linear_wave_Hall_whistler_dv.cpp"

Run the "configure.py" with --prob=linear_wave_Hall_whistler_dv, to set up the problem.

The corresponding input file is named "athinput.test_Hall_whistler" in the inputs folder. Copy the file to the environment in which you want to run the code.

# second test: Brio and Wu shock
The second test is Brio and Wu shock test, and the corresponding problem generator (pgen) is named as "shock_tube_hall.cpp"

Run the "configure.py" with --prob=shock_tube_hall, to set up the problem.

The corresponding input file is named as "athinput.bw_Hall" in the inputs folder.

# Both two tests' results are includeing in the "Test1.ipynb".
See the file to get more information.
