# Physics All-Topics Review — Vectors, Kinematics and Forces

**One note for everything so far.** Built from Sessions S1–S6: vectors, motion in a line, motion graphs, projectiles, relative velocity, circular motion, Newton's three laws, free-body diagrams, friction, inclines and connected objects.

**Conventions:** $g = 9.81\ \text{m/s}^2$ · up and right are positive · $u$ = initial velocity, $v$ = final velocity, $a$ = acceleration, $t$ = time, $s$ = displacement · angles measured from the $+x$ axis unless stated.

**How to use it (45 minutes):** 10 min section 1 (vectors) · 10 min sections 2–3 · 10 min sections 4–5 · 10 min sections 6–7 · 5 min section 8 (mixed check).

---

## 1. Vectors

### 1.1 Scalar or vector

| | Scalar | Vector |
| --- | --- | --- |
| Has | size (magnitude) only | size **and** direction |
| Examples | distance, speed, time, mass, energy, temperature | displacement, velocity, acceleration, force, weight |
| Adds by | ordinary arithmetic | tip-to-tail or components |

A vector is drawn as an arrow: length = magnitude (to scale), arrowhead = direction. A **negative** vector has the same length and points the opposite way.

### 1.2 Adding vectors

- **Same line:** add with signs. $+8\ \text{N}$ and $-3\ \text{N}$ give $+5\ \text{N}$.
- **Tip-to-tail (drawing):** put the tail of the second vector at the tip of the first. The **resultant** runs from the first tail to the last tip.
- **Perpendicular vectors** (Pythagoras):

$$R = \sqrt{A^2 + B^2} \qquad \tan\theta = \frac{B}{A}$$

*Why:* tip-to-tail, two perpendicular vectors form the legs of a right triangle and the resultant is the hypotenuse.

### 1.3 Components

Any vector $A$ at angle $\theta$ from the $x$-axis is the sum of a horizontal and a vertical part:

$$A_x = A\cos\theta \qquad A_y = A\sin\theta$$

*Why:* in the right triangle with hypotenuse $A$, $\cos\theta = \frac{A_x}{A}$ and $\sin\theta = \frac{A_y}{A}$.

Back from components to the vector:

$$A = \sqrt{A_x^2 + A_y^2} \qquad \theta = \tan^{-1}\!\left(\frac{A_y}{A_x}\right)$$

**Signs by quadrant:** left means $A_x < 0$, down means $A_y < 0$. Always check the angle against a sketch (the calculator's $\tan^{-1}$ only returns angles between $-90°$ and $90°$).

### 1.4 The component method (any two or more vectors)

1. Resolve every vector into $x$ and $y$ components.
2. Add: $R_x = A_x + B_x$, $R_y = A_y + B_y$.
3. Rebuild: $R = \sqrt{R_x^2 + R_y^2}$, $\theta = \tan^{-1}(R_y / R_x)$.

*Example.* $A = 5.0\ \text{m}$ at $30°$, $B = 3.0\ \text{m}$ at $120°$.

| | $x$ | $y$ |
| --- | --- | --- |
| $A$ | $5.0\cos 30° = 4.33$ | $5.0\sin 30° = 2.50$ |
| $B$ | $3.0\cos 120° = -1.50$ | $3.0\sin 120° = 2.60$ |
| $R$ | $2.83$ | $5.10$ |

$R = \sqrt{2.83^2 + 5.10^2} = 5.83\ \text{m}$, $\theta = \tan^{-1}(5.10 / 2.83) = 61°$ above the $+x$ axis.

**Subtracting:** $A - B = A + (-B)$. Reverse $B$, then add.

**Equilibrium:** if the vectors add to zero, the object is in equilibrium ($R_x = 0$ and $R_y = 0$).

### 1.5 Scale drawings

Choose a scale (for example 1 cm : 10 N), draw each vector with ruler and protractor, measure the resultant, and convert back. Real size = drawing size × scale factor.

## 2. Motion in a straight line

| Quantity | Definition | Type |
| --- | --- | --- |
| Distance | total path length | scalar |
| Displacement $s$ | change in position, start to finish | vector |
| Average speed | $\dfrac{\text{distance}}{\text{time}}$ | scalar |
| Average velocity | $v_{avg} = \dfrac{\Delta x}{\Delta t}$ | vector |
| Acceleration | $a = \dfrac{\Delta v}{\Delta t} = \dfrac{v - u}{t}$ | vector |

Speeding up: $a$ and $v$ have the same sign. Slowing down: opposite signs. Negative acceleration does not always mean slowing down.

### 2.1 The kinematic equations (constant acceleration only)

**S1.** From the definition of acceleration, $a = \frac{v - u}{t}$:

$$v = u + at$$

**S0.** With constant $a$, velocity changes evenly, so the average velocity is $\frac{u + v}{2}$:

$$s = \tfrac{1}{2}(u + v)\,t$$

**S2.** Put $v = u + at$ into S0:

$$s = \tfrac{1}{2}(u + u + at)\,t = ut + \tfrac{1}{2}at^2$$

**S3.** From S1, $t = \frac{v - u}{a}$. Put it into S0: $s = \frac{(v + u)(v - u)}{2a} = \frac{v^2 - u^2}{2a}$, so

$$v^2 = u^2 + 2as$$

**Choosing:** list the five quantities $s, u, v, a, t$. You know three and want one; use the equation that does not contain the fifth.

*Example.* A car goes from rest to 25 m/s in 10 s. $a = \frac{25 - 0}{10} = 2.5\ \text{m/s}^2$; $s = \frac{1}{2}(0 + 25)(10) = 125\ \text{m}$.

### 2.2 Free fall

Only gravity acts: $a = -g = -9.81\ \text{m/s}^2$ (up positive), the same for every mass.

- At the top of the flight $v = 0$, but $a$ is still $-9.81\ \text{m/s}^2$.
- Time up = time down, and the speed is the same at the same height.

*Example.* Dropped from 45 m: $s = \frac{1}{2}gt^2 \Rightarrow t = \sqrt{\frac{2(45)}{9.81}} = 3.03\ \text{s}$; $v = gt = 29.7\ \text{m/s}$.

### 2.3 Motion graphs

| Graph | Slope gives | Area under the line gives |
| --- | --- | --- |
| position–time | velocity | — |
| velocity–time | acceleration | displacement |
| acceleration–time | — | change in velocity |

Position–time: straight line = constant velocity, curve = accelerating, flat = at rest. Velocity–time: flat = constant velocity, straight sloped line = constant acceleration, crossing the axis = changing direction.

## 3. Projectile motion

**Key idea:** horizontal and vertical motions are independent. Horizontal: constant velocity ($a_x = 0$). Vertical: free fall ($a_y = -g$). They share the same time $t$.

Launch speed $u$ at angle $\theta$: $u_x = u\cos\theta$, $u_y = u\sin\theta$.

$$x = u_x t \qquad v_y = u_y - gt \qquad y = u_y t - \tfrac{1}{2}gt^2$$

### 3.1 Launched from the ground, landing at the same height

- **Time of flight.** Set $y = 0$: $t\,(u_y - \frac{1}{2}gt) = 0$, so $T = \dfrac{2u\sin\theta}{g}$.
- **Maximum height.** At the top $v_y = 0$; from $v_y^2 = u_y^2 - 2gH$: $H = \dfrac{u^2\sin^2\theta}{2g}$.
- **Range.** $R = u_x T = \dfrac{2u^2\sin\theta\cos\theta}{g} = \dfrac{u^2\sin 2\theta}{g}$. Largest at $45°$; angles that add to $90°$ give the same range.

*Example.* $u = 20\ \text{m/s}$ at $30°$: $u_x = 17.3$, $u_y = 10.0\ \text{m/s}$. $T = \frac{2(10.0)}{9.81} = 2.04\ \text{s}$; $H = \frac{10.0^2}{2(9.81)} = 5.10\ \text{m}$; $R = 17.3 \times 2.04 = 35.3\ \text{m}$.

### 3.2 Launched horizontally from a height $h$

$u_y = 0$, so the fall time depends only on the height:

$$t = \sqrt{\frac{2h}{g}} \qquad x = u_x t \qquad v_y = gt \qquad \text{speed} = \sqrt{u_x^2 + v_y^2}$$

*Example.* 15 m/s off a 20 m cliff: $t = \sqrt{\frac{2(20)}{9.81}} = 2.02\ \text{s}$; $x = 15 \times 2.02 = 30.3\ \text{m}$; $v_y = 19.8\ \text{m/s}$; impact speed $= \sqrt{15^2 + 19.8^2} = 24.8\ \text{m/s}$.

### 3.3 Launched at an angle from a height

Take the launch point as the origin. Landing at depth $h$ below it means $y = -h$:

$$-h = u_y t - \tfrac{1}{2}gt^2$$

Solve this quadratic for $t$ (keep the positive root), then $x = u_x t$.

## 4. Relative velocity

$$\vec{v}_{AC} = \vec{v}_{AB} + \vec{v}_{BC}$$

Read it as "velocity of A relative to C = A relative to B + B relative to C". The inner letters match. Also $\vec{v}_{AB} = -\vec{v}_{BA}$.

- **Same line:** two cars at 30 m/s and 20 m/s. Same direction: relative speed 10 m/s. Opposite directions: 50 m/s.
- **Boat crossing a river:** boat 4.0 m/s straight across, current 3.0 m/s. Speed relative to the bank $= \sqrt{4.0^2 + 3.0^2} = 5.0\ \text{m/s}$, at $\tan^{-1}(3.0/4.0) = 36.9°$ downstream of straight across. River 100 m wide: crossing time $= \frac{100}{4.0} = 25\ \text{s}$ (uses only the across component); drift downstream $= 3.0 \times 25 = 75\ \text{m}$.

## 5. Uniform circular motion

Constant speed, but the direction keeps changing, so the object **is accelerating**, toward the center.

$$v = \frac{2\pi r}{T} \qquad a_c = \frac{v^2}{r} \qquad F_c = \frac{mv^2}{r}$$

- $T$ = period (time for one lap); frequency $f = \frac{1}{T}$.
- Velocity is tangent to the circle. Acceleration and net force point to the center (**centripetal**).
- Centripetal force is not a new force. It is the net force supplied by tension, friction, gravity or the normal force. If it vanishes, the object moves off in a straight line along the tangent.

*Example.* $r = 0.50\ \text{m}$, $T = 2.0\ \text{s}$, $m = 0.20\ \text{kg}$: $v = \frac{2\pi(0.50)}{2.0} = 1.57\ \text{m/s}$; $a_c = \frac{1.57^2}{0.50} = 4.93\ \text{m/s}^2$; $F_c = 0.20 \times 4.93 = 0.99\ \text{N}$.

## 6. Newton's laws of motion

**First law (inertia).** An object at rest stays at rest, and an object in motion keeps moving at constant velocity, unless a net external force acts on it.

$$\sum \vec{F} = 0 \iff \vec{v} = \text{constant} \quad (\vec{a} = 0)$$

Inertia is the resistance to a change in motion; mass measures it. Constant velocity means balanced forces, not "no forces".

**Second law.** The acceleration of an object is directly proportional to the net force on it, inversely proportional to its mass, and in the direction of the net force.

$$\vec{F}_{net} = m\vec{a} \qquad 1\ \text{N} = 1\ \text{kg·m/s}^2$$

Apply it separately in each direction: $\sum F_x = ma_x$, $\sum F_y = ma_y$.

**Third law.** When object A exerts a force on object B, B exerts a force on A that is equal in size and opposite in direction.

$$\vec{F}_{A \text{ on } B} = -\vec{F}_{B \text{ on } A}$$

The two forces act on **different objects**, so they never cancel each other. They are the same type of force and exist together. (A book's weight and the normal force from the table are *not* a third-law pair: both act on the book.)

**Mass and weight.** Mass (kg) is the amount of matter and is the same everywhere. Weight is the force of gravity: $W = mg$ (N).

**Apparent weight (elevator).** The scale reads the normal force. From $N - mg = ma$:

$$N = m(g + a)$$

Accelerating up: heavier. Accelerating down: lighter. Constant velocity: $N = mg$. Free fall ($a = -g$): $N = 0$.

**Terminal velocity.** Air drag grows with speed. When drag equals weight, the net force is zero and the speed stays constant.

*Example.* A 60 kg person in an elevator accelerating upward at $2.0\ \text{m/s}^2$: $N = 60(9.81 + 2.0) = 709\ \text{N}$.

## 7. Free-body diagrams, friction, inclines, connected objects

### 7.1 Free-body diagram (FBD)

Draw the object as a dot. Draw only the forces acting **on** it, each as an arrow from the dot, labeled: weight $mg$ (down), normal $N$ (perpendicular to the surface), tension $T$ (along the rope, away from the object), friction $f$ (along the surface, opposing sliding), applied force. Never draw "$ma$" or velocity as a force.

Then: choose axes → resolve tilted forces into components → write $\sum F = ma$ for each axis → solve.

### 7.2 Friction

$$f_s \le \mu_s N \qquad f_k = \mu_k N$$

- **Static** friction matches the push exactly, up to a maximum $\mu_s N$. **Kinetic** friction is constant once sliding; usually $\mu_k < \mu_s$.
- On a level surface with only horizontal pushes, $N = mg$. If a force has a vertical part, $N$ changes.

*Example.* A 10 kg box is pulled horizontally with 50 N; $\mu_k = 0.30$. $N = 10(9.81) = 98.1\ \text{N}$; $f_k = 0.30(98.1) = 29.4\ \text{N}$; $a = \frac{50 - 29.4}{10} = 2.06\ \text{m/s}^2$.

### 7.3 Inclined plane (angle $\theta$)

Tilt the axes along and perpendicular to the slope. Weight resolves into $mg\sin\theta$ down the slope and $mg\cos\theta$ into the slope.

Perpendicular: $N = mg\cos\theta$. Along the slope (sliding down): $mg\sin\theta - \mu_k mg\cos\theta = ma$, so

$$a = g(\sin\theta - \mu_k\cos\theta) \qquad \text{frictionless: } a = g\sin\theta$$

A block just stays at rest when $mg\sin\theta = \mu_s mg\cos\theta$, that is $\tan\theta = \mu_s$.

*Example.* $\theta = 30°$, $\mu_k = 0.20$: $a = 9.81(0.500 - 0.20 \times 0.866) = 3.21\ \text{m/s}^2$.

### 7.4 Connected objects

Same rope: same tension and the same size of acceleration. Write $F_{net} = ma$ for each object, then add the equations so $T$ cancels.

**Atwood machine** ($m_2 > m_1$): $m_2 g - T = m_2 a$ and $T - m_1 g = m_1 a$. Adding:

$$a = \frac{(m_2 - m_1)g}{m_1 + m_2} \qquad T = \frac{2m_1 m_2 g}{m_1 + m_2}$$

**Block on a table ($m_1$) pulled by a hanging mass ($m_2$):** $m_2 g - T = m_2 a$ and $T - \mu_k m_1 g = m_1 a$, so

$$a = \frac{(m_2 - \mu_k m_1)g}{m_1 + m_2}$$

*Example.* Atwood, $m_1 = 2.0\ \text{kg}$, $m_2 = 3.0\ \text{kg}$: $a = \frac{(1.0)(9.81)}{5.0} = 1.96\ \text{m/s}^2$; $T = \frac{2(2.0)(3.0)(9.81)}{5.0} = 23.5\ \text{N}$.

## 8. Mixed check (answers below)

1. Find the components of a 50 N force at $37°$ above the $+x$ axis.
2. A hiker walks 6.0 km east, then 8.0 km north. Find the distance walked and the displacement.
3. A ball is thrown straight up at 14.7 m/s. Find the time to the top and the maximum height.
4. A marble rolls off a 1.25 m high table at 4.0 m/s. How far from the table does it land?
5. A plane flies 200 m/s north in a 50 m/s wind blowing east. Find its velocity relative to the ground.
6. A 1000 kg car takes a 50 m radius curve at 20 m/s. Find the centripetal acceleration and the force. What supplies it?
7. A 5.0 kg block is pushed with 20 N on a level floor. Find $a$ with no friction, then with $\mu_k = 0.20$.
8. A 2.0 kg block slides down a frictionless $25°$ incline. Find its acceleration.
9. On a velocity–time graph, what do the slope and the area represent?
10. A book rests on a table. Name the third-law partner of the book's weight.

### Answers, step by step

1. $F_x = 50\cos 37° = 39.9\ \text{N}$; $F_y = 50\sin 37° = 30.1\ \text{N}$.
2. Distance $= 6.0 + 8.0 = 14.0\ \text{km}$. Displacement $= \sqrt{6.0^2 + 8.0^2} = 10.0\ \text{km}$ at $\tan^{-1}(8.0/6.0) = 53.1°$ north of east.
3. $v = u - gt = 0 \Rightarrow t = \frac{14.7}{9.81} = 1.50\ \text{s}$. $H = \frac{u^2}{2g} = \frac{14.7^2}{2(9.81)} = 11.0\ \text{m}$.
4. $t = \sqrt{\frac{2(1.25)}{9.81}} = 0.505\ \text{s}$; $x = 4.0 \times 0.505 = 2.02\ \text{m}$.
5. Speed $= \sqrt{200^2 + 50^2} = 206\ \text{m/s}$; direction $\tan^{-1}(50/200) = 14.0°$ east of north.
6. $a_c = \frac{20^2}{50} = 8.0\ \text{m/s}^2$; $F_c = 1000 \times 8.0 = 8000\ \text{N}$, supplied by static friction between the tires and the road.
7. No friction: $a = \frac{20}{5.0} = 4.0\ \text{m/s}^2$. With friction: $f_k = 0.20(5.0)(9.81) = 9.81\ \text{N}$; $a = \frac{20 - 9.81}{5.0} = 2.04\ \text{m/s}^2$.
8. $a = g\sin\theta = 9.81\sin 25° = 4.15\ \text{m/s}^2$ (the mass cancels).
9. Slope = acceleration. Area between the line and the time axis = displacement.
10. The weight is Earth pulling the book down, so the partner is the book pulling Earth up with an equal force. (Not the normal force.)

## Notes for next session

- Weakest areas to check first: signs of components in quadrants II–IV, and third-law pairs versus balanced forces.
- Not yet covered: work, energy, momentum.
