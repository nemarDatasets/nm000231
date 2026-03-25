# P300 dataset from Hoffmann et al 2008

P300 dataset from Hoffmann et al 2008.

## Dataset Overview

- **Code**: EPFLP300
- **Paradigm**: p300
- **DOI**: 10.1016/j.jneumeth.2007.03.005
- **Subjects**: 8
- **Sessions per subject**: 4
- **Events**: Target=2, NonTarget=1
- **Trial interval**: [0, 1] s
- **Runs per session**: 6
- **File format**: MATLAB

## Acquisition

- **Sampling rate**: 2048.0 Hz
- **Number of channels**: 32
- **Channel types**: eeg=32, misc=2
- **Channel names**: AF3, AF4, C3, C4, CP1, CP2, CP5, CP6, Cz, F3, F4, F7, F8, FC1, FC2, FC5, FC6, Fp1, Fp2, Fz, MA1, MA2, O1, O2, Oz, P3, P4, P7, P8, PO3, PO4, Pz, T7, T8
- **Montage**: standard_1020
- **Hardware**: Biosemi ActiveTwo
- **Sensor type**: active
- **Line frequency**: 50.0 Hz

## Participants

- **Number of subjects**: 8
- **Health status**: mixed
- **Clinical population**: 4 disabled (cerebral palsy, multiple sclerosis, late-stage amyotrophic lateral sclerosis, traumatic brain and spinal-cord injury C4 level), 4 able-bodied
- **Age**: mean=38.4, min=30, max=56
- **Gender distribution**: male=7, female=1
- **BCI experience**: no training required
- **Species**: human

## Experimental Protocol

- **Paradigm**: p300
- **Number of classes**: 2
- **Class labels**: Target, NonTarget
- **Trial duration**: 1.0 s
- **Study design**: Subjects counted silently how often a prescribed image (one of six: television, telephone, lamp, door, window, radio) was flashed while images were flashed in random sequences
- **Feedback type**: none
- **Stimulus type**: image_flash
- **Stimulus modalities**: visual
- **Primary modality**: visual
- **Mode**: offline
- **Instructions**: Subjects were asked to count silently how often a prescribed image was flashed
- **Stimulus presentation**: flash_duration=100ms, isi=400ms, display=six images (television, telephone, lamp, door, window, radio)

## HED Event Annotations

Schema: HED 8.4.0 | Browse: https://www.hedtags.org/hed-schema-browser

```
  Target
    ├─ Sensory-event
    ├─ Experimental-stimulus
    ├─ Visual-presentation
    └─ Target

  NonTarget
    ├─ Sensory-event
    ├─ Experimental-stimulus
    ├─ Visual-presentation
    └─ Non-target

```
## Paradigm-Specific Parameters

- **Detected paradigm**: p300
- **Number of targets**: 6
- **Inter-stimulus interval**: 400.0 ms
- **Stimulus onset asynchrony**: 400.0 ms

## Data Structure

- **Trials**: {'target': 135, 'non-target': 675}
- **Trials per class**: target=135, non-target=675
- **Trials context**: per_session

## Preprocessing

- **Data state**: raw
- **Preprocessing applied**: False

## Signal Processing

- **Classifiers**: BLDA, FLDA
- **Feature extraction**: temporal samples from selected electrodes
- **Frequency bands**: analyzed=[1.0, 12.0] Hz

## Cross-Validation

- **Method**: leave-one-session-out
- **Folds**: 4
- **Evaluation type**: session-based

## Performance (Original Study)

- **Accuracy**: 100.0%
- **Itr**: 28.8 bits/min
- **Max Bitrate Disabled Avg**: 19.0
- **Max Bitrate Able Bodied Avg**: 38.6
- **Max Bitrate Overall Avg**: 28.8

## BCI Application

- **Applications**: environment_control
- **Environment**: laboratory
- **Online feedback**: False

## Tags

- **Pathology**: Healthy, Cerebral palsy, Multiple sclerosis, Amyotrophic lateral sclerosis, Traumatic brain injury, Post-anoxic encephalopathy
- **Modality**: Visual
- **Type**: Research

## Documentation

- **DOI**: 10.1016/j.jneumeth.2007.03.005
- **License**: Unknown
- **Investigators**: Ulrich Hoffmann, Jean-Marc Vesin, Touradj Ebrahimi, Karin Diserens
- **Senior author**: Karin Diserens
- **Contact**: ulrich.hoffmann@epfl.ch
- **Institution**: Ecole Polytechnique Fédérale de Lausanne
- **Department**: Signal Processing Institute
- **Address**: Signal Processing Institute, CH-1015 Lausanne, Switzerland
- **Country**: CH
- **Repository**: http://bci.epfl.ch/p300
- **Publication year**: 2008
- **Funding**: Swiss National Science Foundation Grant No. 200020-112313
- **Keywords**: Brain–computer interface, P300, Disabled subjects, Fisher's linear discriminant analysis, Bayesian linear discriminant analysis

## References

Hoffmann, U., Vesin, J-M., Ebrahimi, T., Diserens, K., 2008. An efficient P300-based brain-computer interfacefor disabled subjects. Journal of Neuroscience Methods . https://doi.org/10.1016/j.jneumeth.2007.03.005
Appelhoff, S., Sanderson, M., Brooks, T., Vliet, M., Quentin, R., Holdgraf, C., Chaumon, M., Mikulan, E., Tavabi, K., Hochenberger, R., Welke, D., Brunner, C., Rockhill, A., Larson, E., Gramfort, A. and Jas, M. (2019). MNE-BIDS: Organizing electrophysiological data into the BIDS format and facilitating their analysis. Journal of Open Source Software 4: (1896). https://doi.org/10.21105/joss.01896

Pernet, C. R., Appelhoff, S., Gorgolewski, K. J., Flandin, G., Phillips, C., Delorme, A., Oostenveld, R. (2019). EEG-BIDS, an extension to the brain imaging data structure for electroencephalography. Scientific Data, 6, 103. https://doi.org/10.1038/s41597-019-0104-8

---
Generated by MOABB 1.5.0 (Mother of All BCI Benchmarks)
https://github.com/NeuroTechX/moabb
