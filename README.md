# Steel-bellows-under-internal-pressure
A steel bellows is subjected to an internal pressure of 50bars.

This is a kind of basic example of a simulation in Salome-Meca/Code_Aster. The geometry is prepared in Salome-Meca (minor repairs, designing the flanges). Meshing is performed in SMESH with netgen, flanges and bellows are meshed separately and glued together in Code_Aster via liaisons. Wall thickness is 1mm only, very thin compared to the overall size. A pressure of 50bars is applied to the internal surfaces. The bottom surfaces of both flanges are fixed. The simulation results in approx. 7M DOFs and takes about 1000s on a dual CPU workstation.

![Bildschirmfoto vom 2023-03-05 19-29-09](https://user-images.githubusercontent.com/89903493/222978925-e82c081c-44a5-4e45-8a42-495ef73f1ee9.png)
This image shows the bellows at t=1 with 50bars and the VonMises result with 5x exaggerated displacements. The pressure deforms the bellows on the outside a little more (larger internal surface --> larger force). This internal pressure leads to >1000MPa in the thin steel, which is already a very high value.
