---
layout: page
heading: Science & the Whole Tale
subheading: 
full_footer: false
header_content: false
container_col: 8
container_class: bigtext
---

An early preview release of the WT dashboard has been made available at the
first Whole Tale hackathon (a.k.a. "provathon"), collocated and co-organized
with DataONE at Tamaya, New Mexico. Now scientists and researchers can begin to
develop and share tales through the dashboard at
https://dashboard.wholetale.org/ .

Why and how do we expect scientists to use Whole Tale?

Imagine the following real-world computational science scenarios: 

# Computational Archaeology

A research team has developed a new method for reconstructing ancient climates
from tree-ring chronologies. Their current workflow is implemented as R scripts
and consists of (1) downloading relevant tree-ring and modern climate datasets
available in various federated data repositories; (2) cleaning and
restructuring those datasets to prepare them for analysis; (3) running
embarrassingly parallel steps to model ancient climate across whole landscapes;
(4) generating spatiotemporal predictions for those past climates; and (5)
converting them to visual or statistical presentations (videos, figures, graphs
of summary statistics). The research team has shared their workflow as a series
of R scripts in GitHub for reuse and reproducibility and invited other
researchers to use their code and contact them with questions. However, the
scripts written by the research team are not platform independent or language
agnostic and require users to build and install several system tools (external
to R) from source. The system also hasn’t been designed to take advantage of
large compute resources. This research team has been trying to help other
researchers at the Long-term Vulnerability and Transformation Project to
reproduce elements of their study, and have run up against all of these issues.

Using Whole Tale, a team member logs into WT-federated ID management with her
university credentials and gains access to her personal WT environment. Making
use of an available RStudio docker container, she opens her notebook for this
experiment and uses the available library functions to seamlessly discover and
access relevant data from federated data sources, such as tDAR or DataONE.
Using a docker container with access to Globus transfer services and to XSEDE
national analysis and visualization resources, she constructs an analysis
workflow that can be easily and collaboratively reviewed and reproduced by
other researchers. To model ancient landscapes and then to generate a set of
summary statistics, Globus transfer services move the prepared data to Wrangler
at TACC to utilize an optimized and parallelized instance of the workflow (in
R, Matlab, or Python) with the results sent back to her notebook.

# Astronomy

A team of computational astrophysicists carries out a landmark cosmology
simulation of the first stars and galaxies in the universe on the Blue Waters
supercomputer, producing in excess of 2PB of simulation output data and a set
of stunning initial scientific discoveries. The researchers are interested in
not only making the raw data available but also enabling individuals not
originally part of the research team to conduct meaningful analysis that may
lead to subsequent discoveries. Even if the data were made available for
download, it is unlikely that external researchers would be able to make full
use of it without an enormous amount of effort to transfer the data, identify
resources for analyzing that data, and then somehow share and publish their own
results.

Using Whole Tale and his local university credentials, a team member logs into
the WT-federated ID management and gains access to his personal WT environment,
comprising data staging areas, interactive Jupyter notebooks, and transparent
data access capabilities. He creates a data compendium that includes source
code, output data, and yt-based analysis tools, gets a DOI, and places the
collection into the WT-extended BW Data Sharing Service. He submits a
manuscript for publication to Science with the DOI for the data collection,
which includes the source code for their analysis and access to the collection.
As the paper is reviewed and published, the WT-linking service links the paper
and the 2PB collection, which is curated at NCSA in collaboration with the
researcher’s home institution, along with the raw data and analysis tools in
the WT environment. Other astronomers, who work on the Dark Energy Survey (DES)
and are not part of the original collaboration, connect to remote analysis
resources at TACC and SDSC via Internet2 supported, SDN-enhanced network paths
to compare DES data with a new analysis of the published simulation data. The
additional discoveries are seamlessly captured in the personalized staging
areas for the individual researchers, shared via the publishing system, and
published through the same process.

## What’s next?

Whole Tale will enable science uses cases like these and others, by providing
seamless access to uniquely identified (registered) data, popular frontends
(such as Jupyter notebooks, RStudio, and others), and computational resources:
all through a convenient dashboard, directly from the user’s browser, without
the need to install software (e.g. RStudio or Jupyter) locally on the user’s
computer or laptop. As we are increasing the capabilities of WT and the
WT-dashboard, we would like to hear from you how you have used (or would like
to use) the WT system.

<Link: Please tell us your science story and how you have used (or would like to used) the WT system>


