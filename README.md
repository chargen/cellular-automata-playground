# cellular-automata-playground

http://www.kchapelier.com/cellular-automata/ (see below for examples)

A little utility to work with 2D cellular automata and a demo for the [cellular automata](https://github.com/kchapelier/cellular-automata) npm module.

Said module is designed and optimized to process sequences of rules in a single shot.

The following [rule formats](https://github.com/kchapelier/cellular-automata-rule-parser) are accepted : Life (S/B), custom Extended Life (E S/B), Extended Stochastic (E S:P/B:P), Vote for life and LUKY. In my opinion the Extended Life rule format is the most readable and the most polyvalent as it can be used with large neighborhoods and higher dimensions (3D, 4D, ...).

## Examples 2D

Click on the images to load the app with the matching settings.

<a href="http://www.kchapelier.com/cellular-automata/#width=100&height=100&oov=1&rule=E_3,4_/_0,3,4_corner_2*8&rule=E_3,4_/_0,2,4_corner_4*4&rule=E_2,3_/_3*6"><img src="https://github.com/kchapelier/cellular-automata-playground/raw/master/example-images/example1.png" alt="" height=200 /></a> <a href="http://www.kchapelier.com/cellular-automata/#width=100&height=100&oov=1&rule=E_2,3_/_3,6*100&rule=E_2..5_/_0,7..8*3&rule=E_1..7_/_*3"><img src="https://github.com/kchapelier/cellular-automata-playground/raw/master/example-images/example2.png" alt="" height=200 /></a> <a href="http://www.kchapelier.com/cellular-automata/#width=100&height=100&oov=1&rule=E_2..4_/_0:0.035,2,3,4_V*40&rule=E_4,3_/_V*1&rule=E_3..8_/_7..8*1"><img src="https://github.com/kchapelier/cellular-automata-playground/raw/master/example-images/example3.png" alt="" height=200 /></a> <a href="http://www.kchapelier.com/cellular-automata/#width=100&height=100&oov=1&rule=E_4..7_/_0,1,4,6,7,8_V*96"><img src="https://github.com/kchapelier/cellular-automata-playground/raw/master/example-images/example4.png" alt="" height=200 /></a> <a href="http://www.kchapelier.com/cellular-automata/#width=100&height=100&oov=1&rule=E_3,4,6,7_/_3..4_axis_2*25&rule=E_8..12_/_2..4_V_2*11"><img src="https://github.com/kchapelier/cellular-automata-playground/raw/master/example-images/example5.png" alt="" height=200 /></a> <a href="http://www.kchapelier.com/cellular-automata/#width=100&height=100&oov=1&rule=E_3,2_/_3*40&rule=E_1,2_/_2,4_corner*6&rule=E_2,3_/_2,3_V*3"><img src="https://github.com/kchapelier/cellular-automata-playground/raw/master/example-images/example6.png" alt="" height=200 /></a>

## Examples 3D

<a href="http://www.kchapelier.com/cellular-automata/#d=3&width=35&height=35&depth=35&oov=1&rule=E_6..12_/_12,6..10,17*10&rule=E_20..24_/_3..6_corner_15*6"><img src="https://github.com/kchapelier/cellular-automata-playground/raw/master/example-images/example3d-1.png" /></a>
<a href="http://www.kchapelier.com/cellular-automata/#d=3&width=60&height=60&depth=60&oov=1&rule=E_4..8_/_6..8_corner_4*2&rule=E__0..24_/_9..24*6&rule=E_5..6_/_6..8_corner_12*10"><img src="https://github.com/kchapelier/cellular-automata-playground/raw/master/example-images/example3d-2.png" /></a>

# Roadmap

* Refactoring index.js should be the priority for the next version.
* Download as PNG, [OBJ](https://github.com/kchapelier/three-geometry-to-obj) and [VOX](https://github.com/kchapelier/ndarray-to-vox).
* More sanitization of user inputs.
* Add support for multi-states rules (Generations, Cyclic CA and NLUKY). They are already supported by the underlying modules.
* Output using with marching squares to smooth out the edges in 2D.
* Allow the edition of the initial grid.
