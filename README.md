# summer-work

This is some sample code written in Jupyterhub notebooks during my summer as an LCLS intern at SLAC, 
the goal of the project was to improve the analysis of photon detections against an ANDOR detector. 
The existing technique when I arrived was to:

1.) Throw away photon firing events with an outputted eV counts > 825 as these were suspected gamma effects
2.) Subtract the average outputted noise of the detector
3.) Sum the differences between the outputs of the "pixel strings" and their normal outputs

I improved on this technique by applying pixel to pixel noise calculations, as well as confirming that there
was a statistically significant amount of electron drift across pixels. Then I determined that drift was significant up 
to two pixels away from the suspected collision location. Finally, I adapted the technique to sum the 2 neighboring pixels
on either side of the suspected collision as opposed to across the entire lens of the detector, which increased the normalcy of 
our suspected counts/collision measurement.
