## **Dynamo**: Mapping Vector Field of Single Cells
![Dynamo](https://raw.githubusercontent.com/Xiaojieqiu/jungle/master/dynamo_intro.png)

Understanding how gene expression in single cells progress over time is vital for revealing the mechanisms governing cell fate transitions. RNA velocity, which infers immediate changes in gene expression by comparing levels of new (unspliced) versus mature (spliced) transcripts (La Manno et al. 2018), represents an important advance to these efforts. A key question remaining is whether it is possible to predict the most probable cell state backward or forward over arbitrary time-scales. To this end, we introduce an inclusive model (termed Dynamo) capable of predicting cell states over extended time periods, that incorporates promoter state switching, transcription, splicing, translation and RNA/protein degradation by taking advantage of scRNA-seq and the co-assay of transcriptome and proteome. We also implement scSLAM-seq by extending SLAM-seq to plate-based scRNA-seq (Hendriks et al. 2018; Erhard et al. 2019; Cao, Zhou, et al. 2019) and augment the model by explicitly incorporating the metabolic labelling of nascent RNA. We show that through careful design of labelling experiments and an efficient mathematical framework, the entire kinetic behavior of a cell from this model can be robustly and accurately inferred. Aided by the improved framework, we show that it is possible to analytically reconstruct the transcriptomic vector field from sparse and noisy vector samples generated by single cell experiments. The analytically reconstructed vector further enables global mapping of potential landscapes that reflects the relative stability of a given cell state, and the minimal transition time and most probable paths between any cell states in the state space This work thus foreshadows the possibility of predicting long-term trajectories of cells during a dynamic process instead of short time velocity estimates. Our methods are implemented as an open source tool, [dynamo](https://github.com/aristoteleo/dynamo-release).

## **Dynamo package**: comprehensive analysis of single cell expression dynamics
![dynamo_demo](https://raw.githubusercontent.com/Xiaojieqiu/jungle/master/dynamo_demo.png)

[Dynamo tutorials](https://github.com/aristoteleo/dynamo-tutorials) - [Dynamo workflow](https://github.com/aristoteleo/dynamo-release/wiki/Dynamo-workflow) - [Installation](https://github.com/aristoteleo/dynamo-release/wiki/Dynamo-workflow#installation) - [Citation](https://github.com/aristoteleo/dynamo-release/wiki/Dynamo-workflow#citation) - [Theory behind dynamo](https://github.com/aristoteleo/dynamo-release/wiki/Dynamo-workflow#theory-behind-dynamo)



## Acknowledgement
We would like to sincerely thank the developers of velocyto (La Manno Gioele and others), scanpy (Alex Wolf and others) and svelo (Volker Bergen and others) on their amazing tools which demonstrate the best practice of scientific programming in Python. Dynamo takes various technical inspiration from those packages. Dynamo is (we are trying to and hope users can contribute to) fully compatible with those tools and velocity estimation from either scvelo or velocyto can both be used as input to learn the functional form of vector field for predicting the cell fate over extended time period and mapping global cell state potential. 

## Contribution 
If you want to contribute to the development of dynamo, please check out CONTRIBUTION instruction: [Contribution](https://github.com/aristoteleo/dynamo-release/blob/master/CONTRIBUTING.md)

## Documentation  
The documentation of dynamo package is available at [readthedocs](https://dynamo-release.readthedocs.io/en/latest/)
