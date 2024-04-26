<image align="right" alt="Milad" width = "380" src="http://up44.ir/previews/c3c5f7dab58aa78702557eeb7517235e.jpg"> 
    
<pre>import math     # library of python for calculate the calculation of below <br />
ζ_a = 1         # amplitude <br />
L_w = 20        # wave lenght <br />
g = 9.81        # gravity <br />
π = 3.14        # pi number <br />
V_w = (g * L_w) / (2 * π)    # wave velocity <br />
time_values = [0, 0.1, 0.2, 0.3, 1]   # Assuming you want to calculate ζ 
                                        for specific time values <br />
for t in time_values:
<pre>    for x in range(21):  # Assuming x ranges from 0 to 20 <br />
           ζ = ζ_a * math.sin((2 * π / L_w) * (x - (V_w * t))) <br />
           print(f"ζ at t={t:.1f}, x={x}: {ζ:.4f}") <br />
