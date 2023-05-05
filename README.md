Download Link: https://assignmentchef.com/product/solved-ece253-homework-3
<br>
<ol>

 <li>Consider the following FSM:</li>

</ol>

States: a, b, c, d, e, f Transitions:

0,a −<em>&gt; </em>b,1

1,a −<em>&gt; </em>c,0

0,b −<em>&gt; </em>f,0

1,b −<em>&gt; </em>d,0

0,c −<em>&gt; </em>a,0

1,c −<em>&gt; </em>c,0

0,d −<em>&gt; </em>c,1

1,d −<em>&gt; </em>e,0

0,e −<em>&gt; </em>a,0

1,e −<em>&gt; </em>c,0

0,f −<em>&gt; </em>b,0

1,f −<em>&gt; </em>d,0

Is this a minimal machine? If not, find the smallest equivalent machine.

<ol start="2">

 <li>Consider a quadrature encoder that senses the direction (clockwise or counter-clockwise) of a click based on the values on its two pins:</li>

</ol>

Figure 1

When at rest, both pins of the encoder read a logic high. For a clockwise click, Pin1 goes low first, then Pin2 goes low, then Pin1 one goes high, and finally Pin2 goes high. Whereas for a counter-clockwise click, the sequence is reversed: Pin2 goes low first, then Pin1 goes low, then Pin2 one goes high, and finally Pin1 goes high. The two pins never transition at the exact same time.

<ul>

 <li>Design a FSM that has two inputs (Pin1 and Pin2), is triggered on value changes on the inputs and produces two outputs (<em>CW </em>for a clockwise click and <em>CCW </em>for a counterclockwise click). The outputs are produced on completion of the entire sequence described above. Draw a bubble chart for your design. Assume that the start-up state for the machine is (Pin1=1, Pin2=1).</li>

</ul>

1

<ul>

 <li>Mechanical switches and quadrature encoders in specific are often bouncy. The pins undergo several transitions when they switch their state before they settle to a high or low value. A case with bouncing pins during a clockwise click is shown below:</li>

</ul>

Figure 2

When one pin is bouncing, assume that the other pin does not change its state at all. Design a FSM that detects clockwise and counter-clockwise clicks correctly producing a <em>CW </em>output for a clockwise click and <em>CCW </em>output for a counter-clockwise click, given the bouncy behavior of the pins. The pins can bounce any number of times before settling, and the outputs should be produced on completion of the entire sequence of changes for a clock-wise or a counter-clockwise click.

<ol start="3">

 <li>Read Chapter 3 of Lee and Seshia, answer problems 3 and 6. Please note that the book uses a different meaning for non-determinism – in both cases the question arises when multiple states are potential results of a single transaction. In the class version, it transits to all states at the same time. In the book version, it chooses among the possible states and transits to one of them. Both versions are used to simplify the FSM model in the face of “Don’t care” or unspecific behavior.</li>

</ol>