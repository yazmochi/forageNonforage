# forageNonforage
Source data are separately stored for each experiment.
* sourceDataExp1.mat: the source data for experiment 1 in the Matlab file format
* sourceDataExp2.mat: the source data for experiment 2 in the Matlab file format

Both files contain the variable “SourceData” which  includes participants’ demographic variables and responses to the risk choices.
SourceData: Number of participants * 5 cell array
* SourceData{i, 1}: Gender of the i-th participant (‘F’=female, ‘M’=male, ’n/a’=not applicable)
* SourceData{i, 2}: Age of the i-th participant
* SourceData{i, 3}: Experimental condition for the environment that the i-th participant assigned（Experiment1: “PR”=Poor-Rich group, “RP”=Rich-Poor group; Experiment2: “IPI”=Intermediate-Poor-Intermediate, “IRI”=Intermediate-Rich-Intermediate）
* SourceData{i, 4}: Experimental condition for the stimulus presentation that the i-th participant assigned（’L’=Yes option is presented on the left, ’R’=Yes option is presented on the right）
* SourceData{i, 5}: Experimental stimulus and the response of the i-th participant
    * SourceData{i, 5}(j, 1): Reward magnitude of the j-th trial
    * SourceData{i, 5}(j, 2): Reward probability of the j-th trial
    * SourceData{i, 5}(j, 3): Choice of the participants on the j-th trial (0=No/ Not gamble, 1=Yes / Gamble)
    * SourceData{i, 5}(j, 5): Reward assignment on the j-th trial (0= Gambled and unrewarded, 1= Gambled and rewarded, 2=Not gambled and rewarded)
