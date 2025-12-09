---
layout: project
title: ENGRD 2020 HW5 
description: Design a mechanism to lift a maximised weight to a maximised hight 
technologies: [LaTeX, Design]
image: /assets/images/HW4Design1.png
---
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/katex@0.16.0/dist/katex.min.css" integrity="sha384-..." crossorigin="anonymous">
<script defer src="https://cdn.jsdelivr.net/npm/katex@0.16.0/dist/katex.min.js" integrity="sha384-..." crossorigin="anonymous"></script>
<script defer src="https://cdn.jsdelivr.net/npm/katex@0.16.0/dist/contrib/auto-render.min.js" integrity="sha384-..." crossorigin="anonymous"
    onload="renderMathInElement(document.body);"></script>

Given a 2D design space of 150cm long and 50cm tall, a rigid bar of a fixed length, 3 pin supports of which two need to be mounted on the ground and a linear actuator, design a frame/mechanism to lift the maximum possible weight to the highest possible height.
![Before and After]({{ "/assets/images/HW4Design2.png" | relative_url }}){: .inline-image-r}

**Constraints** & **Objectives**: Select beam cross section such that deflection must be under 2% of length. 

**I-Beam Deflection**

**Dimensions:**
- Overall height: $$h = 290$$ mm
- Flange width: $$b_f = 165$$ mm
- Flange thickness: $$t_f = 19$$ mm
- Web thickness: $$t_w = 11$$ mm

$$I_z = \frac{b_f h^3}{12} - \frac{(b_f - t_w)(h - 2t_f)^3}{12}$$

$$I_z = \frac{165 \times 290^3}{12} - \frac{(165 - 11)(290 - 38)^3}{12}$$

$$I_z = \frac{165 \times 24,389,000}{12} - \frac{154 \times 252^3}{12}$$

$$I_z = \frac{4,024,185,000}{12} - \frac{154 \times 16,003,008}{12}$$

$$I_z = 335,348,750 - 205,372,103$$

$$I_z = 129,976,647 \text{ mm}^4$$

$$F_{\perp} = F_{actuator} \sin(\alpha) = 5000 \times \sin(60°) = 5000 \times 0.866 = 4330 \text{ N}$$

$$\delta_{end} = \frac{F_{\perp} d^2}{6EI}[3L - d]$$

$$\delta_{end} = \frac{4330 \times 300^2}{6 \times 69,000 \times 129,976,647} \times [3(1000) - 300]$$

$$\delta_{end} = \frac{389,700,000}{53,810,331,858,000} \times 2700$$

$$\delta_{end} = \frac{1,052,190,000,000}{53,810,331,858,000}$$

$$\delta_{end} = 19.55 \text{ mm}$$

$$\frac{\delta_{end}}{L} = \frac{19.55}{1000} = 0.01955 = 1.955\%$$




