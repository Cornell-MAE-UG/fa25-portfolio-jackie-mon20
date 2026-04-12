---
layout: project
title: Update on Team Dragonfly 
description: Functional Prototype — Team Dragonfly / Cornell CALS Extension / E&J Gallo Winery / National Grape
image: /assets/images/SLF.jpg
---

<div style="border:1px solid #ddd; border-radius:10px; padding:1rem 1.25rem; margin:1rem 0 1.5rem 0; background:#fafafa;">
  <h2 style="margin-top:0;">Project Navigation</h2>
  <p style="margin-bottom:0.5rem;">Use the links below to jump directly to each portfolio milestone.</p>
  <ul style="margin-bottom:0;">
    <li><a href="#client-pitch">Client Pitch</a></li>
    <li><a href="#functional-prototype">Functional Prototype</a></li>
  </ul>
</div>

This page documents the evolution of the scraper.

---

## <a id="client-pitch"></a>Client Pitch

For this project, we are developing a scrape that woulo allow people to kill SLF egg masses in a more convient way.

### Problem Statement

Grape farmers in the Northeast US are invaded by spotted lanternflies (SLFs) that infiltrate harvests. The SLF population grows rapidly due to many nymphs surviving to adulthood, where they reproduce abundantly, increasing their population by a factor of 5.47. Current solutions primarily target adults, but rapid population growth is already occurring by this stage, increasing the severity of their impact regardless.

### Proposed Direction

The Scraper would be a device that makes it quicker and simpler for SLF egg masses to be removed while allowing access to hard-to-reach locations. The user would spot egg masses visually or using the light feature, extend the scraper using a telescoping mechanism, and remove the egg masses into an enclosed housing.

Why it’s better than the status quo:
- Current SLF scrapers are credit card–sized and require close contact with egg masses
- Our scraper simplifies the process and improves accessibility
- For our MVP, we will create a prototype that extends and contains egg masses and develop a preliminary UI. Long term, we will - integrate a working UI, camera system, and improve reproducibility.

### Impact

Decreasing SLF’s reproduction factor from 5.47 will slow population growth and potentially stagnate it in an area, reducing the number of SLFs per vine from 400.

---

## <a id="functional-prototype"></a>Functional Prototype

---

## Prototype Overview

The functional prototype consists of the following main subsystems:

- **Box housing** made from laser-cut wooden plates
- **Removable side panel** for user access
- **3D-printed funnel**
- **3D-printed iris mechanism**
- **Chemical diffuser holder and connector**

---

## Design Documentation

Parts:
- 1 Clear Impact-Resistant Polycarbonate Rectangle Tube (1" x 1" x 1')
- McMaster code: 3161T31-3161T311
- 1 Spring Spring Hinge
- McMaster code: 15205A83
- 1' x 1' x 1/16" PVC Plate
- McMaster Code: 8747K111
- Balsa Wood
- ¼ - 20 Hardware (screws, nuts, etc.)
- M3 Hardware (screws, nuts, etc.)

---

## Assembly
Assembly Instructions:
1. Cut the 1' x 1' PVC Plate to 4¼" x 2¾" using band saw
2. Belt sand the PVC plate at a 30° angle
3. Cut Balsa Wood to 3 ¼" x 1 ½" using band saw
    a. Optional: Sand corners for a cleaner finish
4. Drill three ¼” holes into both the balsa wood and the PVC Plate
5. Assemble springs onto the bolts and bolt through the wood and PVC, placing a nut on
the other end
6. Torque the nut while still allowing for compression, while keeping the assembly secure
7. Drill two M3 holes in the wood piece and attach the spring hinge with M3 hardware
8. Cut more Balsa Wood into an isosceles triangle (3¼” side length, 2¾” base)
a. Optional: Sand corners for a cleaner finish
9. Drill ¼” holes into the balsa wood triangle (5 of them in a semi-circle and one of them in
the tip of the isosceles triangle, with the 5 holes 2” apart from the hole in the tip)
10. Drill two M3 holes in the top of the triangle piece and attach it to the spring hinge with M3
hardware
11. Drill two ¼” holes across the tube 2” apart
12. Screw the lower hole of the tube with the hole in the tip of the isosceles triangle
13. Pin the other hole toward the tip of the tube with one of the 5 holes in the semi-circle of
the isosceles triangle
14. Add cardboard and tape to the back as a makeshift stopper

---

## Design Tests

---

## Test 1: 
The angle of the scraper blade must vary to conform to different surfaces. Ideally, it can
vary to a radius of curvature of 4”.
### Description:
This tests the scraper blade itself, springs, and spring hinge mechanism. To
conduct this test, we will measure the displacement of the tip of the scraper blade
from its initial position to its fully ‘bent’ position. This will allow us to calculate the
angle and determine how much the ends of the blade are able to conform. We
will repeat this a few times to ensure that we are measuring the
displacement/angle consistently to lower our margin of error.
### Results:
We measured that the center of the tip of the scraper can deflect at most about
0.25” when pressed against a smooth round surface. Using that measurement
and the fact that the two edges of the PVC blade are 4 ¼” apart, we can calculate
that the minimum radius of curvature our scraper can wrap around is about 9.16”.
This is constrained by the mounting and flexibility of our blade.
### Implications:
From this test, we can conclude that the placement of the springs/bolts and the
flexibility of the blade are insufficient, as they don’t allow the blade to wrap
around surfaces with our benchmark radius of curvature. We will likely keep a
similar design and dimensions, but change the thickness of the scraper blade to
allow for more flexibility in the blade itself. In the future, we plan to test our
prototypes on a variety of surfaces outside to get accurate results.

---

## Test 2: 
The force transferred from the user to the scraper blade must be within regular comfort
for a user. This is quantifiable by surveying users and having them rate their comfort
levels on a scale of 1-10.

### Description:
This tests the scraper blade and the length/general sizing of the handle. This will
be especially useful as we move towards modeling and understanding the
telescoping handle in the future. To test this, we will have 10 people try to scrape
off modeled egg masses. Each participant will rank the ease and comfort of the
force they are applying so that the handle can be modeled for the average
person’s strength.

### Results:
For smooth, flat surfaces, all 10 users rated that the experience was
“comfortable” and it didn’t require too much force to scrape off the egg masses.
However, for curved surfaces, 9 out of 10 users rated that the experience
required an uncomfortable amount of force to bend the blade to the shape of the
surface before scraping, and all 10 thought it was easier to scrape multiple times
from different angles with the blade being flat rather than to try to bend the blade
and scrape everything off in one go.

### Implications:
The flat surface part of the test told us that our overall design works well, as there
weren’t any issues with transferring force from the handle to the blade, so we will
likely keep a similar overall design. Through the curved surface test, we learned
that there are still many improvements to be made. For our blade, we used a
1/16” piece of acrylic since we thought that would be thin enough to easily bend
and mold to the shape of surfaces with small amounts of pressure. However,
through this test, we learned that that is not the case and that 1/16” is still too
thick. For our next prototype, we plan to make the blade thinner - about 1/32” - to
allow it to bend and flex easily. Additionally, we will build up the size and length of
the handle as we move towards our telescoping handle design to ensure that
users do not have to exert a significant amount of force.
---

## Test 3: 

Through cyclic use, the scraper blade must not experience significant deformation
beyond ¼”.

### Description:
This tests the scraper blade and the spring mechanisms. This ensures that with
repeated use, the mechanism does not degrade and does not apply a force on
the blade such that it enters the plastic deformation region. To test this, we will
take measurements and record the scraper blade and spring displacement
before any scraping. Then, we will scrape off modeled egg masses 40 times and
retake these measurements to see if the scraper blade has deformed and if the
springs have changed. We will also visually inspect the blade and mechanism for
any visible damage.

### Results:
We ran the test as specified above and found that there are no meaningful
differences before and after scraping - the blade visually appears the same as
before, and the scraper blade and springs are in the same spot relative to each
other. There seems to be minimal deflection within 1/32” of an inch, which is
negligible in the scope of the design.

### Implications:
Through this test, we discerned that the materials we chose are strong and
durable enough for their intended purpose. Since these materials are able to
withstand repeated bending and scraping, we will likely use them again for our
later prototypes and final product. We aim to do this test again once we change
the thickness of our blade, as this can impact deformation over time with
repeated use. Additionally, the next time we run this test, we want to test the
scraper repeatedly on surfaces outside, as this time we mostly used surfaces
inside the lab space

---

## Success Criteria

A scraper that is quick to use, conforms to different surfaces durably, is more appealing to the
average user than an alternate card or disposal method, and:

- It should be able to be set up and used in under one minute. Time is a high priority.
- It should be able to withstand repeated use, maintaining its functionality by not
deforming more than ¼” after 40 times of use. Durability is a high priority.
- It should be able to bend to a minimum radius of curvature of 4 inches to allow it to follow
many different surface curvatures for ease of removal. Adapting to different surfaces is a
high priority.
- It should be better to use than a standard card: after being offered both, at least 15 out of
20 people should choose our scraper over the current standard as their preferred egg
disposal method. A higher preference rate is a high priority.
The success criteria of being able to conform to surfaces will be shown in the demo on exhibit
day. We will show how the scraper bends enough to effectively remove egg masses on a variety
of surfaces with different curvatures, including a 4-inch radius of curvature, as an example of an
egg mass on an 8-inch diameter tree. We can provide samples of different surfaces (e.g., tree
bark, concrete) to allow users to demo using the scraper on a variety of surfaces to depict how
the blade can be widely used.

---