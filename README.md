# RLSB-CongX-Qiskit
Reversible Logic Synthesis Benchmarks for Qiskit and CongX.

[Reversible Logic Synthesis Benchmarks Page](https://webhome.cs.uvic.ca/~dmaslov/) is a useful tools for benchmarking reversible/quantum circuit optimization. The original contents are written in machine-readable format (.tfc file) by Dmitri Maslov et al..

This is a rewriting of Reversible Logic Synthesis Benchmarks in Qiskit by [Shin Nishio](https://scholar.google.com/citations?user=gZNt8twAAAAJ&hl=ja)(a.k.a. parton). 

# How to use ?
Qiskit / CongX quantum circuit. First, install Qiskit and CongX.

1. Requirements
    * `!pip install qiskit`
    * `!pip install CongX`
2. Clone this repository
    * `git clone git@github.com:parton-quark/RLSB-OpenQASM.git`
3. Compile circuits by your compiler! There is an example [here](https://github.com/parton-quark/RLSB-CongX-Qiskit/blob/master/converter/tutorial_for_converter_en.ipynb). Japanese version is [here](https://github.com/parton-quark/RLSB-CongX-Qiskit/blob/master/converter/tutorial_for_converter_jp.ipynb).

3. **Send your Record to [RLSB](https://webhome.cs.uvic.ca/~dmaslov/submit.html)!**

# Contents
Quantum circuits and recording optimization results
## Contents from Original RLSB 
To be released after approval of the original author

<!-- 
|Family/type|Individual functions and circuits|
|:--:|:--:|
|4-bit with maximal gate count:|[4b15g_1](https://github.com/parton-quark/RLSB-CongX-Qiskit/blob/master/circuits/original/00_4-bit_with_maximal_gate_count/RLSBCQ_4b15g_1.py) , 4b15g_2 , 4b15g_3 , 4b15g_4 , 4b15g_5|
|Adders:|1bitadder (rd32) , 5bitadder , 8bitadder|
|Divisibility checkers:|4mod5 , 5mod5|
|Cycle functions:|cycle10_2 , cycle17_3|
|Galois field multipliers:|gf2^3mult , gf2^4mult , gf2^5mult , gf2^6mult , gf2^7mult , gf2^8mult , gf2^9mult , gf2^10mult , gf2^11mult , gf2^12mult , gf2^13mult , gf2^14mult , gf2^15mult , gf2^16mult , gf2^17mult , gf2^18mult , gf2^19mult , gf2^20mult , gf2^32mult , gf2^50mult , gf2^64mult , gf2^100mult , gf2^127mult , gf2^128mult , gf2^131mult , gf2^163mult , gf2^256mult , gf2^512mult|
|Gray code functions|--|
|Hamming coding functions:|ham3 , ham7 , ham15|
|Hidden weighted bit functions:|hwb4 , hwb5 , hwb6 , hwb7 , hwb8 , hwb9 , hwb10 , hwb11 , hwb12 , hwb13 , hwb14 , hwb15 , hwb16 , hwb20 , hwb50 , hwb100 , hwb200 , hwb500 , hwb1000|
|MMD worst case:|3_17 , 4_49|
|Modula adders:|mod5adder , mod1024adder , mod1048576adder|
|N-th prime:|nth_prime3_inc , nth_prime4_inc , nth_prime5_inc , nth_prime6_inc , nth_prime7_inc , nth_prime8_inc , nth_prime9_inc , nth_prime10_inc , nth_prime11_inc , nth_prime12_inc , nth_prime13_inc , nth_prime14_inc , nth_prime15_inc , nth_prime16_inc , nth_prime17_inc|
|Permanent:|permanent1x1 , permanent 2x2 , permanent3x3 , permanent 4x4|
|RD - input weight functions:|rd53 , rd73 , rd84|
|Symmetric functions:|6sym , 9sym|
|Other:|2-4dec , 2of5 , xor5| -->

## Additional Circuits 
Newly written circuit for RLSB-CongX-Qiskit.

|Algorithm|image|.tfc|.py|description|
|:-------:|:---:|:--:|:-:|:---------:|
|Quantum Walk on complete graph|image|circuits|circuits|TBD|

<!-- Quantum Cost is given as follows.
$$C=C_s+C_c \times$ 10$$ where $C_s$ is a number of Single-Qubit gates, and $C_c$ is a number of Two-Qubit Gates. 
 -->
<!-- ## Parameters to optimize
The hardware and system software (including quantum error correction) of the state-of-the-art quantum information processing system define the work that the quantum compiler should do and the method of evaluating its performance.

If you think there is more metric to add to this benchmark, please build an Issue. -->

## Contact and citation
Feel free to contact me via issues for this repository or send email to parton@sfc.wide.ad.jp .
If you use this software, be sure to cite all of the original RLSB, RLSB-CongX-Qiskit, CongX,and Qiskit. Bib file of RLSB, RLSB-CongX-Qiskit, and CongX is [here](https://github.com/parton-quark/RLSB-CongX-Qiskit/blob/master/RLSB-CongX-Qiskit.bib).
The author of Qiskit fluctuates so please collect bib from this [link](https://github.com/Qiskit/qiskit/blob/master/Qiskit.bib).

## Acknowledgement
Special thanks and respect to Dmitri Maslov, the original RLSB maintainer and all programmers involved in that project. 

Thanks to [Atsushi Matsuo(IBM Research)](https://researcher.watson.ibm.com/researcher/view.php?person=jp-MATSUOA) for telling me about the existence of RLSB. Thanks to my supervisor at Keio University SFC, Professor [Rodney Van Meter](https://web.sfc.keio.ac.jp/~rdv/) and Assistant Professor [Takahiko Satoh](http://quantum.sfc.keio.ac.jp/employees/takahiko-satoh/). Thanks to all members of [AQUA](https://aqua.sfc.wide.ad.jp/members_en.html)(Advancing Quantum Architecture group) for useful discussions. 

## See also
* [CongX](https://github.com/parton-quark/CongX) is a controlled gate exansion set for Qiskit. Includes some generalized(biary controlled) Tofolli gate and compilers for them. Made by Shin Nishio.
