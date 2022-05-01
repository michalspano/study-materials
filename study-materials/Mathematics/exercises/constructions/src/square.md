# Task to complete 

<!-- define the task in this part -->

Given is a square $ABCD$. We label the sides of the square as $a$ and the diagonal as $d$. We know the measure of $d-a$. Create the steps of such a construction.
___

# Steps of construction. 

<!-- include the steps of construction -->

Suppose a plane $\alpha$. We have a line segment $\overline{AX}$, such that $\overline{AX} \subset \alpha$. Furthermore, $\overline{AX}=d-a$. Then, we create a ray $\overrightarrow{AX}$.  

Suppose we create line segments from $X$ to any of the 4 vertices. We then observe such 4 triangles:

1. $\Delta_{ABX}$, where $\overline{AB}=a$, $\overline{BX}=b$, $\overline{AX}=d-a$
2. $\Delta_{BCX}$, where $\overline{BC}=a$, $\overline{BX}=b$, $\overline{CX}=a$
3. $\Delta_{CDX}$, where $\overline{CD}=a$,  $\overline{CX}=a$, $\overline{DX}=b$
4. $\Delta_{ADX}$, where $\overline{AD}=a$, $\overline{AX}=d-a$,  $\overline{DX}=b$

$\dots$ we observe $\Delta_{ABX} \cong \Delta_{ADX} \land \Delta_{BCX} \cong \Delta_{CDX}$. 

<!-- remark for brevity -->

\*We don't need to specify the size $b$ as it's not for this particular example. Moreover, the triangle $\Delta_{ABX}$ (likewise $\Delta_{ADX}$) are of no significance for this particular exercise. Since, $\Delta_{BCX} \cong \Delta_{CDX}$, we will use $\Delta_{BCX}$ for brevity.

<!-- computation -->

We see that $\Delta_{BCX}$ is an isosceles triangle with an angle $\measuredangle BCX = 45^{\circ}$. Therefore, $\measuredangle CBX = \measuredangle CXB = (180 - 45) \div 2 = 67.5^{\circ}$. We continue with the next step, namely, we create $\overleftrightarrow{p}$, such that $X \in \overleftrightarrow{p} \land \measuredangle \overrightarrow{AX}, \overleftrightarrow{p} = 67.5^{\circ}$ (in the upper half-plane). Additionally,  we have $\overleftrightarrow{q}$, such that $A \in \overleftrightarrow{q} \land \measuredangle \overrightarrow{AX}, \overleftrightarrow{q} = 45^{\circ}$. Consequently, we get the vertex $B$, where $\overleftrightarrow{p} \cap \overleftrightarrow{q} = \{B\}$. In order to obtain the vertex $C$, we create a line $\overleftrightarrow{r}$, such that $B \in \overleftrightarrow{r} \land \overleftrightarrow{q} \perp \overleftrightarrow{r}$. So, we have $C$, where $\overrightarrow{AX} \cap \overleftrightarrow{r} = \{C\}$. Lastly, we create a line segment $\overline{CD}$, where $\overline{CD} \parallel \overleftrightarrow{q} \land$ $\overline{CD} = \overline{AB}$. Finally, we observe the square $ABCD$ in the plane $\alpha$.

