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
    <li><a href="#final-prototype">Final Prototype</a></li>
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

## <a id="final-prototype"></a>Final Prototype

### Context and Problem Statement:
The spotted lanternfly presents an especially challenging problem as its population grows rapidly
due to a high number of nymphs surviving to adulthood, where they reproduce abundantly, increasing
their population by a factor of 5.47 [1]. Current solutions primarily target adults, but rapid population growth is already occurring by this stage, increasing the severity of their impact regardless.
This aspect is promising as it tackles the root issue: limiting SLF populations by reducing
reproduction success. We aim to reduce the overall population of SLFs in a vineyard or region. Creating even a small dent in SLF’s reproduction rate can have a significant impact on their numbers and harm.

### Final Prototype and Application:
Our final prototype is an extendable scraper with a conforming blade that matches the curvature
of a surface by utilizing 3-point bending. The scraper is lightweight and has a telescoping handle,
allowing it to be used at multiple lengths. The blade is attached to a collection pouch that egg masses fall into when scraped, and the handle itself uses a spring hinge mechanism to vary its angle. Additionally, there are several orientations of the handle, allowing the user to vary its angle with respect to two planes.
The scraper is meant to be an accessible and easy method for users and the general public to
scrape egg masses off of trees and other varied surfaces, thus reducing the SLF population and the
infestation issue for harvesters. This could be used in vineyards and farms, where SLFs are especially troublesome. Additionally, the scrapers could be incentivized and placed in parks for the general public.
The user workflow is as follows: A user spots an SLF egg mass, extends the scraper using the
telescoping handle, scrapes the egg masses using the compliant blade, and finally, the egg masses fall into the collection pouch for easy disposal and removal.

### Conclusion and Recommendation:
This design has potential, but it requires more in-depth updates and field testing. The scraper
would be more effective if outfitted with a light, a camera, and a display that would aid users in viewing egg masses, and the telescoping could be automated in future iterations. Our tests proved the scraper could withstand heavy usage and conform to different surfaces, but showed issues with the disposable bag. In the future, the disposable plastic bag should be replaced with a permanent container housing disposable liners, and the scraper should be tested with environmental factors (eg. weather).
However, even with this design, it is hard to guarantee that people would use the scraper without
a larger incentive. Furthermore, it is more expensive than anticipated to implement this, as vineyards would have to hire someone to scrape off the egg masses. More research and studies should be done into existing incentive numbers i.e., how many people use the SLF egg mass credit cards vs how many are handed out. Surveys could be conducted on this to discern if this is truly a promising product. This could affect future implementations of this product, and ways to reduce the production cost should also be considered (whether mass-producing them or switching to certain lower-cost parts).

### Testing and Results:
We aimed to create a scraper that is quick to use, can durably conform to varying surfaces, is comfortable to the average user, and:
● It should be able to be set up and used in under 30 seconds. Time is a high priority.
● It should be able to withstand repeated use, maintaining its functionality by not deforming more
than ¼” after 50 times of use. Durability is a high priority.
● It should be able to bend to a minimum radius of curvature of 4 inches to allow it to follow many
different surface curvatures for ease of removal. Adapting to different surfaces is a high priority.
● It should require a comfortable level of force for the average user. At least 75% of users must rate their comfort with the force exerted to scrape off ‘egg masses’ at least a 7/10 on flat and curved surfaces. A reasonable comfort level is a high priority.
● It should collect egg masses consistently in the collection pouch. At least 75% of scraped egg
masses should fall into the pouch, and it should not overflow or deteriorate within 15 scrapings.

Our earlier prototypes required a lot of force from users despite being able to curve to a large radius, which led us to use a thinner, 1/32” scraper blade. Additionally, we sized up the handle radius to1-¼”. The final prototype was able to be set up within 15 seconds when replacing the bag (took <5 without replacement), did not show any signs of degradation or deformation after a full exhibition or repeated testing, had a minimum radius of curvature of 9.16”, and was rated highly by users as seen in the chart below. We tested it on trees outside, and it scraped modeled egg masses reasonably well with gravity aiding this, as we struggled to collect our egg masses properly when scraping horizontally during demonstrations. Thus, as seen in this testing, the scraper is easy to set up, durable, conforms to a variety of surfaces, and is comfortable for users. However, the scraper struggled with collecting egg masses. The disposable pouch only caught egg masses about 50% of the time when tested on trees and seemed flimsy at times. Future iterations of this product should either implement support for the disposable pouch or replace it with a permanent container housing replaceable liners.

### Prototype and Testing Details:
Our first “proof of concept” prototype is shown here and was constructed from cardboard, wood, and paper. This prototype helped us discern estimates for the blade size and handle length and identify problems that arise during physical assembly, such as positioning of the disposable collection pouch. We moved from this to our first real prototype, where our main goal was to troubleshoot the scraper blade and test our 3 point bending mechanism, spring hinge, and scraper blade variance. We created CAD as a mockup and constructed the scraper as pictured here. For this prototype, we stress
tested it over 40 times to determine if the blade would deflect, had users rate their comfort on flat and curved surfaces with modeled egg masses, and calculated our maximum radius of curvature. The blade experienced negligible deflection, there was no degradation, and the maximum radius of curvature was well above the required 4”. However, users struggled to scrape egg masses on curved surfaces. We also found difficulty in the range of motion with the blade itself, as the spring hinge created a tendency to ‘snap’ back after scraping was done.
Prototype 2 focused on the telescoping handle: making it work, figuring out handle connectors,
moving to a new handle size, and testing this. We ordered 2 aluminum hollow rods & 2 different types of handle connectors to determine which was more ideal. Through this, we experimented and found a way to make the rods telescope, and test users unanimously agreed the lever locking mechanism was more intuitive than the knob locking mechanism. We tested the telescoping over 50 uses
and saw no degradation during this period.
Our final prototype used a 1/32” CPVC scraper blade, 3 aluminum rods with 2 telescoping connectors, foam to softly stop the scraper blade from ‘snapping’ back, a large disposable bag, lasercut handle connector and triangular handle piece, 3D printer converter to take the circular rod to rectangular to connect to the blade assembly, the same spring hinge, and similar ¼”-20 and M3 hardware. This
prototype withstood 50 uses in testing and subsequent use during presentations and exhibition day without significant degradation or deflection, was tested on trees outside, was rated highly across all users on comfort on both curved and flat surfaces, and had a maximum radius of curvature of 9.16”.

### Assembly Instructions1:
1. Assembling the Scraper Blade
  a. Cut the 1' x 1' CPVC Plate to 4¼" x 2¾" using band saw, belt sand at a 30° angle1
  b. Assemble springs onto ¼”-20 bolts and bolt through the laser-cut handle connector and CPVC scraper blade, placing a nut on the other end
    i. Torque the nut to allow for compression while keeping the assembly secure
2. Assembling the Angling Head
  a. Hold the spring hinge open and align it with corresponding holes in the laser-cut pieces
    i. Ensure the hinge folds so the blade goes into the Triangular Handle Piece
  b. Connect to the Handle Connector & Triangular Handle Piece using M3 hardware
  c. Torque nuts tightly with a small wrench
3. Assembling the telescoping handle
  a. Wrap 3 layers of tape on the bottom of the Telescoping Rods to create a makeshift stop
  b. Place the Large Telescoping Connector onto the Large Telescoping Rod
  c. Slide the Medium Rod through the bottom of the Large Rod with the taped side of the
  Medium one at the bottom (this taped section should not go through the connector)
  d. Using a wrench, tighten the bolts on the Telescoping Connector until the rod can move in
  it, but there is enough friction to keep hold it when left alone
  e. Repeat for the Small Telescoping Connector and the Small Telescoping Rod
4. Attaching the Angling Head to the handle
  a. Press the 3D Printed Handle Converter onto the Small Telescoping Rod
    i. Holding the blade back to keep it from interfering, align the Triangular Handle
    Piece and place ¼”-20 bolts through the top and bottom holes (top hole may be chosen by the user and changed anytime to change the orientation of the blade)
    ii. Secure with nuts, torque tightly
  b. Be careful not to ‘snap’ the blade in one direction due to the spring hinge
  c. Place foam on top of the Handle Converter as a soft stop for the blade
5. Attach the disposable bag to the back of the blade assembly by pushing it onto the bolts