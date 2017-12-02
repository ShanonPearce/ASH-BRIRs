# ASH IR Dataset

[![Join the chat at https://gitter.im/ASH-BRIRs/Lobby](https://badges.gitter.im/ASH-BRIRs/Lobby.svg)](https://gitter.im/ASH-BRIRs/Lobby?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
**ASH** (**Audio Spatialisation for Headphones**) is an impulse response dataset that can be used for binaural synthesis of spatial audio systems on headphones. It includes binaural room impulse responses (BRIRs), headphone compensation filters (HPCFs) and configuration files for Equalizer APO. The dataset can be used to create virtual surround sound on headphones through BRIR convolution.

## Binaural Room Impulse Responses
This dataset contains BRIRs derived from a range of freely available BRIR datasets. The BRIRs were measured using Head and Torso Simulators (HATS) in a variety of rooms, each containing unique acoustical properties. For each room a set of BRIRs are provided for a range of source directions around the head on the horizontal plane. The frequency response of each BRIR has been compensated to remove undesired spectral distortions and allow for accurate binaural synthesis of acoustic environments on headphones. The BRIRs are provided as 2 channel WAV files sampled at 44100Hz.

## Headphone Compensation Filters
A set of headphone compensation filters are provided for some commonly used headphones. The filters can be used to equalise individual headphones to the diffuse-field target frequency response. Individual headphone equalisation is recommended as the effectiveness of binaural synthesis will depend on how closely the frequency response of the headphones matches the diffuse-field target. The filters are minimum phase FIRs and are provided as single channel WAV files sampled at 44100Hz. 

## Equalizer APO configuration files
This dataset can be used with [Equalizer APO](https://sourceforge.net/projects/equalizerapo/), an Audio Processing Object (APO) for windows featuring convolution capabilities. Configuration files for BRIR convolution are provided for each room in the dataset and for a range of speaker configurations. Configuration files for HPCF convolution are also provided. A configuration file can be included in your ‘config.txt’ file using the 'Include' control in the configuration editor. The dataset must be placed within the Equalizer APO directory for the configurations to be read.

## License
Unless otherwise stated, all files in this repository are licensed under Creative Commons Attribution-NonCommercial-ShareAlike 4.0 https://creativecommons.org/licenses/by-nc-sa/4.0/

## Further Information
Refer to the [Wiki](https://github.com/ShanonPearce/ASH-BRIRs/wiki) for more information about the dataset including [configuration instructions](https://github.com/ShanonPearce/ASH-BRIRs/wiki/Equalizer-APO-Configuration).
