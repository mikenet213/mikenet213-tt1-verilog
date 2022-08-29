(Original readme for the template repository [here](https://github.com/mattvenn/wokwi-verilog-gds-test/blob/main/README.md))

4-in => 3-out LUT, loaded via a SPI interface. 4-in => 3-out seemed to be the biggest I could fit :-).

Gave up on the rst_n input (can always shift through zeros to reset) so I could have an extra input, and used it with a rotate signal. That way, we can pulse the rotate line and get a kind of sequencer with 16 steps of 3 sync'ed outputs. Or you can ignore that input and just use it as a normal LUT :-).
