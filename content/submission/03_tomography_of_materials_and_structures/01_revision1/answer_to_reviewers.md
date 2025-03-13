# Answer to reviewers

## Reviewer 1

> The study proposes a contrast agent - the µAngiofil - that promises to fill even microvessels; its performance was verified by the authors ex-vivo on different animal models: i.e nr. 1 21-month-old transgenic VEGF male mouse, five CB17SCID male mice, three C57BL/6 mice, and two Göttingen minipigs.
> Different microtomographic systems, with several experimental settings were tested in order to allow the analysis of biopsies of interest in the field of dentistry and oral pathology.
> The contrast agent is already on the market and, according to what the authors claim, it holds great promise for addressing key questions in tissue engineering, implantology, and a wide range of related research fields.
> Although this reviewer agrees with the authors that the proposed contrast agent could be interesting as an aid in the diagnosis of various pathologies and also in the field of tissue engineering, at the same time doubts arise as to how the experimental activity was conducted and whether it can demonstrate what the authors claim above.

### Main Comments:
> Therefore, the first doubt lies in the novelty of the study.
> In fact, there are already several studies in the literature that use microAngiofill also for the study of bone tissue.
> For this reason, it would be appropriate to better outline how this study surpasses the performance of previous ones, paying particular attention to citing all these studies.


> Moreover, the authors have omitted to cite, neither in the Introduction nor in the Discussion, research and review studies that have already addressed the problem of simultaneously visualizing and, above all, quantifying vascular flow and bone microarchitecture; in particular, the studies performed at the synchrotron using phase contrast microtomography without the use of contrast media, successfully performed on both animal and human model biopsies (examples: https://doi.org/10.3389/fphys.2017.00769 ; https://doi.org/10.5966/sctm.2012-0136 , etc. ).


> In any case this reviewer continues to consider the proposed problem relating to the simultaneous visualization of soft tissues (in this specific case, the vascular endothelium) and hard tissues (bones, teeth, dental implants, etc.) through the use of the benchtop microCT.
> Unfortunately, this reviewer fears that the problem has not been well focused in the present study and, consequently, the experimental method to address that.
> In fact, both in dental diagnostics and in oral pathology, up to bone tissue engineering, the object of study requires a very high resolution to be able to visualize even the smallest blood capillaries which are the main actors in tumor kinetics and tissue regeneration.
> Consequently, to appreciate the effectiveness of this contrast medium, it is first necessary to have a high-resolution tomograph (I would say a nanotomograph!) to maintain a single experimental setting for all the tests.
> Subsequently, it is necessary to provide an adequate number of biopsies (same situ in animal models of the same strain, age, sex, etc) that present the same clinical problem, in order to proceed with a quantitative analysis compared to a control group (also made of adequate number of elements).
> In fact, only a quantitative analysis, based on selection of appropriate shape complexity features, can establish the actual efficacy of a contrast agent in these contexts. The visualization of large vessels as performed in your work does not determine the effectiveness of contrast agents in solving problems that are more specifically related to micro vessels, to capillaries, for example in the case of tumor invasion.

### Minor comments:

> In the Materials and Methods chapter, it would be necessary to insert a descriptive table of each animal model studied, reporting strain, age, number, sex, model of the tomograph used to study it, pixel size, Energy, current, etc.

Information on the animals used and and overview on the settings of the tomographic imaging were already present in the manuscript text.
The complete information on the tomographic imaging was already present in a table in the supplementary materials.
We included all the requested information into the mentioned table.

The relevant parameters of the tomographic imaging are mentioned in the text at the beginning of each relevant section.
In addition, a tabular collection of the relevant parameters is collated in a table both attached as supplementary material and available online (linked in the manuscript) at https://github.com/habi/BrukerSkyScanLogfileRuminator/tree/microvasculature-manuscript
In addition---as mentioned in the supplementary materials section---*all* logfiles of *all* scans performed for this study are also available online, permitting the keen reader to exactly replicate the tomographic scan settings we used.

> avoid repeating the same concepts in different parts of the manuscript; for example, the fact that decalcification does not allow the simultaneous study of bone and vessels.

> if the object of the study lies in the characteristics of the contrast agent, it is not enough to recall some literature to describe it, but a brief description of its preparation is also needed.

> Nowadays, threshold-based segmentation of tomographic images is obsolete for many researches since convolutional neural networks support more performant segmentations, also based on morphology and orientation of structures.
> Although this is not the subject of this study, it is necessary to mention these options in the Discussion, citing the supporting literature.

> With reference to the analyses conducted in Dual Energy, it is not very clear what the gain is in terms of vessels detection.
> The analysis carried out at 50kV already allows for a sufficiently clear threshold segmentation.
> In fact, the increase in energy (90kV) seems only allow for an increase in the counts, probably improving the peak shape referred to the vessels.

We agree that a gray value threshold-based segmentation seems already possible with the data from the 50 kV scan, but the compounding issue is that the mineralization of the mouse bones (and thus the gray value in the data) varies in a larger extent than what is visible in panel A of Fig. 7.
Combining both scans into a dual-energy dataset greatly enhances detectability.
As we state in the manuscript already, the difference in gray values for the bones from 50 kV to 90 kV positive, while the gray value difference inside the blood vessels between those values is negative, as is technically evident in panel C' of Fig. 7.
Your statement about already allowing threshold segmentation on the shown data is true in the case for the shown slice, but it is *not* true for the full three-dimensional dataset.

## Reviewer 2

> The manuscript presents valuable results beautiful images of vasculature in different bones (in some cases including implants) imaged using µCT following perfusion with the contrast agent µAngiofil.
> While I believe that the results are methodology shown are very valuable, I do think that the manuscript could benefit from some restructuring to better highlight the main results.
> At the current stage, the paper unfortunately reads more like a report than a publication and I think with the quality of the results that the authors have, they can provide more insights.

# Major comments:

> It's not clear to me why in this instance, the results should be merged with the materials and methods section.
> The details on µCT settings are not the main finding of this paper are they?
> Therefore, I would strongly suggest to separate the results, so that the authors can fully focus on presenting these in a separate section and/or merge them with the discussion section.

> The images are very nice, but there is a number of very large figures (Figs. 1-5), not all of which appear necessary to me.
> At the same time the results are then not presented in much detail.
> Importantly, I'm missing any quantitative evaluation of the perfusion quality achieved.
> Segmentations are sometimes provided, e.g. in Fig.6, but it is unclear to me what we learn from this.
> This poses the important question: how do the authors assess the quality of their perfusion?
> I strongly believe that at least some quantification of vessel diameters, connectivity or similar should be performed for all instances.

> As said above, the images provided are beautiful.
> But I am lacking in most cases a cross-sectional slice that would allow the reader to see the perfusion of the blood vessels more clearly.
> Importantly, I would also like to see corresponding histological slices that show whether certain blood vessels remained non-perfused and that would also show if any shrinkage of the perfusion agent occured.

So called correlative imaging was previously performed to validate the perfusion: https://doi.org/10.1038/srep41842, which is cited several times in the  present manuscript.
In that manuscript we have evaluated the perfusion efficiency of microAngiofil by correlating microCT slices with registered histological slices.
In a total of 3800 assessed capillaries we found that 98% of them were microAngiofil-filled, concluding that microAngiofil allows for an adequate perfusion and visualization of the entire vasculature including the smallest capillaries.
For some of the samples shown in the present study, namely those with metal implants it is also not feasible to produce histological slices.

> At this stage, I think these major comments should first be addressed before more minor comments would be commented on.
