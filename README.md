# WeldXRef
Fanuc Robot mig welding cross referencing.

Did this program to keep track of weld information and usage in a project, it's very specific for the case I had but it's easy to customize.

In my case a main program (example.LS) would call separate weld programs (all starting with "W"), each weld program would have two sections, first one would touchsense to locate a part, would be called with parameters(PR1, PR2, 1) to save touchsense offset data in PR1 and PR2, and then would be called with parameters (PR1, PR2, 2) to weld while having PR1 and PR2 available to apply as offsets.

1. Create .LS backup of robot.
2. Open file in excel, enable macros (you can look at the code if you want to)
3. Select main weld LS program(s).
4. Click start.
