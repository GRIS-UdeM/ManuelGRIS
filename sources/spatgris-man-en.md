**SpatGRIS**

<img src="/media-en/media/image1.png"
style="width:2.01572in;height:2in" />

**Tools for 2D and 3D sound spatialization**

Developed by the

Groupe de Recherche en Immersion Spatiale

**GRIS**

<http://gris.musique.umontreal.ca/>

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>Director:</strong></th>
<th>Robert NORMANDEAU</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><strong>Programmer:</strong></td>
<td>Gaël LANE LÉPINE</td>
</tr>
<tr class="even">
<td><strong>Assistants:</strong></td>
<td>Nicola GIANNINI</td>
</tr>
</tbody>
</table>

**Manual**

*SpatGRIS* 3.3.7

*SpeakerView* 0.0.7

*ControlGRIS2* 1.4.5

*BlackHole* 0.6.0

**April 2025**

<img src="/media-en/media/image2.png"
style="width:1in;height:1in" />

Faculté de musique

<img src="/media-en/media/image3.png"
style="width:3.71155in;height:0.27559in" />
<img src="/media-en/media/image4.png"
style="width:1.02116in;height:0.3937in" />

**Table of Contents**

[1. General presentation
[6](#general-presentation)](#general-presentation)

[1.1. SpatGRIS is a spatialization tool
[6](#spatgris-is-a-spatialization-tool)](#spatgris-is-a-spatialization-tool)

[1.1.1. Spatialization [6](#spatialization)](#spatialization)

[1.1.2. Localization [6](#localization)](#localization)

[1.2. SpatGRIS is a recorder and a player
[6](#spatgris-is-a-recorder-and-a-player)](#spatgris-is-a-recorder-and-a-player)

[1.3. SpatGRIS makes speaker setups
[6](#spatgris-makes-speaker-setups)](#spatgris-makes-speaker-setups)

[1.3.1. DOME speaker setups
[6](#dome-speaker-setups)](#dome-speaker-setups)

[1.3.2 CUBE speaker setups
[6](#cube-speaker-setups)](#cube-speaker-setups)

[1.4. The speakers can be part of the spatialization and the
localization
[6](#the-speakers-can-be-part-of-the-spatialization-and-the-localization)](#the-speakers-can-be-part-of-the-spatialization-and-the-localization)

[1.5. The three components of SpatGRIS
[7](#the-three-components-of-spatgris)](#the-three-components-of-spatgris)

[1.6. What’s new and improved in ControlGRIS/SpatGRIS?
[7](#whats-new-and-improved-in-controlgrisspatgris)](#whats-new-and-improved-in-controlgrisspatgris)

[1.7. Groupe de Recherche en Immersion Spatiale (GRIS)
[8](#groupe-de-recherche-en-immersion-spatiale-gris)](#groupe-de-recherche-en-immersion-spatiale-gris)

[2. INTRODUCTION [8](#introduction)](#introduction)

[2.1. Architecture [8](#architecture)](#architecture)

[2.2. SpatGRIS [9](#spatgris)](#spatgris)

[2.2.1. History [9](#history)](#history)

[2.2.2. System requirements
[9](#system-requirements)](#system-requirements)

[2.2.3. Installation notes
[9](#installation-notes)](#installation-notes)

[2.2.4. Access to the microphone
[10](#access-to-the-microphone)](#access-to-the-microphone)

[2.2.5. BlackHole volume at 0 dB
[10](#blackhole-volume-at-0-db)](#blackhole-volume-at-0-db)

[2.2.6. New Users of BlackHole and macOS 14 Sonoma
[10](#new-users-of-blackhole-and-macos-14-sonoma)](#new-users-of-blackhole-and-macos-14-sonoma)

[2.3. ControlGRIS [10](#controlgris)](#controlgris)

[2.3.1. History [10](#history-1)](#history-1)

[2.3.2. System requirements
[10](#system-requirements-1)](#system-requirements-1)

[2.3.3. Installation notes
[11](#installation-notes-1)](#installation-notes-1)

[2.3.4. AU, VST, AAX [11](#_Toc179799657)](#_Toc179799657)

[2.4. Quick Start Guide [12](#quick-start-guide)](#quick-start-guide)

[3. Connections [14](#connections)](#connections)

[3.1. Connect the DAW to SpatGRIS
[14](#connect-the-daw-to-spatgris)](#connect-the-daw-to-spatgris)

[3.1.1. Open SpatGRIS [14](#open-spatgris)](#open-spatgris)

[3.1.2. Adjust the output level
[14](#adjust-the-output-level)](#adjust-the-output-level)

[3.1.3. Assign the DAW to BlackHole
[14](#assign-the-daw-to-blackhole)](#assign-the-daw-to-blackhole)

[3.1.4. Multiclient [14](#multiclient)](#multiclient)

[3.2. Connect ControlGRIS to SpatGRIS
[15](#connect-controlgris-to-spatgris)](#connect-controlgris-to-spatgris)

[3.2.1. Numbering audio and OSC
[15](#numbering-audio-and-osc)](#numbering-audio-and-osc)

[3.2.2. Sources Colour [16](#sources-colour)](#sources-colour)

[4. ControlGRIS [17](#controlgris-1)](#controlgris-1)

[4.1. Introduction [17](#introduction-1)](#introduction-1)

[4.2. Graphical interface
[17](#graphical-interface)](#graphical-interface)

[4.3. Configuration panel
[18](#configuration-panel)](#configuration-panel)

[4.3.1. Settings [18](#settings)](#settings)

[MODE [18](#mode)](#mode)

[OSC Port [18](#osc-port)](#osc-port)

[IP Address [18](#ip-address)](#ip-address)

[Number of Sources [18](#number-of-sources)](#number-of-sources)

[First Source ID [18](#first-source-id)](#first-source-id)

[4.3.2. Sources [18](#sources)](#sources)

[4.3.3. Controllers [19](#controllers)](#controllers)

[4.4. Spatialization views
[19](#spatialization-views)](#spatialization-views)

[4.4.1 View in DOME mode [19](#view-in-dome-mode)](#view-in-dome-mode)

[4.4.2. Spans in DOME mode
[20](#spans-in-dome-mode)](#spans-in-dome-mode)

[4.4.3. View in CUBE mode [20](#view-in-cube-mode)](#view-in-cube-mode)

[4.4.4. Spans in CUBE mode
[21](#spans-in-cube-mode)](#spans-in-cube-mode)

[4.4.5. CUBE Elevation in Normal or Extended Top mode
[21](#cube-elevation-in-normal-or-extended-top-mode)](#cube-elevation-in-normal-or-extended-top-mode)

[4.4.6. CUBE Elevation in Extended Top and Bottom mode
[22](#cube-elevation-in-extended-top-and-bottom-mode)](#cube-elevation-in-extended-top-and-bottom-mode)

[4.5. How to use ControlGRIS
[22](#how-to-use-controlgris)](#how-to-use-controlgris)

[4.5.1. Load the plugin on a track
[22](#load-the-plugin-on-a-track)](#load-the-plugin-on-a-track)

[4.5.2. Save presets and recording automation
[22](#save-presets-and-recording-automation)](#save-presets-and-recording-automation)

[4.5.3. Recall presets [23](#recall-presets)](#recall-presets)

[4.6. Trajectories [23](#trajectories)](#trajectories)

[4.6.1. Sources Link [24](#sources-link)](#sources-link)

[Azimuth-Elevation (DOME) and Azimuth-Distance (CUBE) Links
[24](#azimuth-elevation-dome-and-azimuth-distance-cube-links)](#azimuth-elevation-dome-and-azimuth-distance-cube-links)

[Elevation Links (CUBE mode only)
[24](#elevation-links-cube-mode-only)](#elevation-links-cube-mode-only)

[4.6.2. Trajectory Type [24](#trajectory-type)](#trajectory-type)

[Azimuth-Elevation (DOME) and Azimuth-Distance (CUBE) Trajectory Type
[25](#azimuth-elevation-dome-and-azimuth-distance-cube-trajectory-type)](#azimuth-elevation-dome-and-azimuth-distance-cube-trajectory-type)

[Elevation (CUBE only) Trajectory Type
[25](#elevation-cube-only-trajectory-type)](#elevation-cube-only-trajectory-type)

[Other settings [25](#other-settings)](#other-settings)

[Realtime [25](#realtime)](#realtime)

[Drawing [26](#drawing)](#drawing)

[Shift-Click in Drawing mode
[26](#shift-click-in-drawing-mode)](#shift-click-in-drawing-mode)

[Activate [27](#activate)](#activate)

[Trajectory recording in the DAW [27](#_Toc179799703)](#_Toc179799703)

[4.6.3. A special case: the pendulum
[27](#a-special-case-the-pendulum)](#a-special-case-the-pendulum)

[4.6.4. Presets and automated trajectories
[27](#presets-and-automated-trajectories)](#presets-and-automated-trajectories)

[5. SpatGRIS [29](#spatgris-1)](#spatgris-1)

[5.1. Introduction [29](#introduction-2)](#introduction-2)

[5.2. SpeakerView [30](#speakerview)](#speakerview)

[5.2.1. Visibility and keyboard shortcuts
[30](#visibility-and-keyboard-shortcuts)](#visibility-and-keyboard-shortcuts)

[5.2.2. Two distinct applications
[30](#two-distinct-applications)](#two-distinct-applications)

[5.3. Change the setup not the spatialization
[31](#change-the-setup-not-the-spatialization)](#change-the-setup-not-the-spatialization)

[5.4. Settings [32](#settings-1)](#settings-1)

[5.5. Controls [32](#controls)](#controls)

[5.6. The DOME and the CUBE
[32](#the-dome-and-the-cube)](#the-dome-and-the-cube)

[5.6.1. DOME [33](#dome)](#dome)

[5.6.2. CUBE [33](#cube)](#cube)

[5.7. The HYBRID mode: DOME and CUBE in the same project
[34](#the-hybrid-mode-dome-and-cube-in-the-same-project)](#the-hybrid-mode-dome-and-cube-in-the-same-project)

[5.7.1. What is saved in HYBRID mode?
[34](#what-is-saved-in-hybrid-mode)](#what-is-saved-in-hybrid-mode)

[5.72. What Mode is loaded according to the opening order of Speaker
Setup and Project?
[34](#what-mode-is-loaded-according-to-the-opening-order-of-speaker-setup-and-project)](#what-mode-is-loaded-according-to-the-opening-order-of-speaker-setup-and-project)

[5.7.3. Attenuation settings in CUBE or HYBRID mode
[35](#attenuation-settings-in-cube-or-hybrid-mode)](#attenuation-settings-in-cube-or-hybrid-mode)

[5.7.4. Convert from DOME to CUBE and vice versa
[36](#convert-from-dome-to-cube-and-vice-versa)](#convert-from-dome-to-cube-and-vice-versa)

[5.7.5. Spatialization in 2D and 3D
[36](#spatialization-in-2d-and-3d)](#spatialization-in-2d-and-3d)

[5.8. Speaker Setup [37](#speaker-setup)](#speaker-setup)

[5.8.1. Speaker Setup Edition
[38](#speaker-setup-edition)](#speaker-setup-edition)

[5.8.2. Speakers’ order and image representation
[38](#speakers-order-and-image-representation)](#speakers-order-and-image-representation)

[5.8.3. Minimal requirements
[39](#minimal-requirements)](#minimal-requirements)

[5.8.4. Direct outputs [40](#direct-outputs)](#direct-outputs)

[Independent direct outputs
[40](#independent-direct-outputs)](#independent-direct-outputs)

[Spatialized direct outputs
[40](#spatialized-direct-outputs)](#spatialized-direct-outputs)

[5.8.5. Show Speaker Numbers
[41](#show-speaker-numbers)](#show-speaker-numbers)

[5.9. Sources and Speakers
[42](#sources-and-speakers)](#sources-and-speakers)

[5.9.1. Mute and Solo [43](#mute-and-solo)](#mute-and-solo)

[5.9.2. Peak indicators and Reset
[43](#peak-indicators-and-reset)](#peak-indicators-and-reset)

[5.10. STEREO reduction [43](#stereo-reduction)](#stereo-reduction)

[5.10.1. STEREO [43](#stereo)](#stereo)

[5.10.2. BINAURAL [44](#binaural)](#binaural)

[5.11. Recording [44](#recording)](#recording)

[6. PLAYER [46](#player)](#player)

[6.1. To make a recording for the PLAYER
[46](#to-make-a-recording-for-the-player)](#to-make-a-recording-for-the-player)

[6.2. To open and to play a project with the PLAYER
[46](#to-open-and-to-play-a-project-with-the-player)](#to-open-and-to-play-a-project-with-the-player)

[6.2.1. Open the listening speaker setup
[46](#open-the-listening-speaker-setup)](#open-the-listening-speaker-setup)

[6.2.2. Open the PLAYER window and load the files
[47](#open-the-player-window-and-load-the-files)](#open-the-player-window-and-load-the-files)

[6.2.3. To play the piece [48](#to-play-the-piece)](#to-play-the-piece)

[6.2.4. DOME in CUBE or CUBE in DOME
[48](#dome-in-cube-or-cube-in-dome)](#dome-in-cube-or-cube-in-dome)

[6.2.5. Regarding the direct outs in the PLAYER
[49](#regarding-the-direct-outs-in-the-player)](#regarding-the-direct-outs-in-the-player)

[6.3. To save a PLAYER project
[50](#to-save-a-player-project)](#to-save-a-player-project)

[7. Menus [51](#menus)](#menus)

[7.1. File menu [51](#file-menu)](#file-menu)

[7.2. View menu [51](#view-menu)](#view-menu)

[7.3. Naming and Saving [52](#naming-and-saving)](#naming-and-saving)

[7.4. Representations [53](#representations)](#representations)

[7.4.1. 3D Representation [53](#d-representation)](#d-representation)

[7.4.2. 2D Representation
[54](#d-representation-1)](#d-representation-1)

[7.5. Performance and CPU burst
[54](#performance-and-cpu-burst)](#performance-and-cpu-burst)

[7.6. Help Menu [54](#help-menu)](#help-menu)

[8. Addendum [55](#addendum)](#addendum)

[8.1. Sources Link descriptions
[55](#sources-link-descriptions)](#sources-link-descriptions)

[8.1.1. Azimuth-Elevation and Azimuth-Distance
[55](#azimuth-elevation-and-azimuth-distance)](#azimuth-elevation-and-azimuth-distance)

[8.1.2. Elevation (CUBE mode only)
[56](#elevation-cube-mode-only)](#elevation-cube-mode-only)

[8.2. Trajectory descriptions
[57](#trajectory-descriptions)](#trajectory-descriptions)

[8.2.1. Azimuth-Elevation and Azimuth-Distance
[57](#azimuth-elevation-and-azimuth-distance-1)](#azimuth-elevation-and-azimuth-distance-1)

[8.2.2. Elevation (CUBE mode only)
[58](#elevation-cube-mode-only-1)](#elevation-cube-mode-only-1)

[8.3. OSC messages in SpatGRIS
[58](#osc-messages-in-spatgris)](#osc-messages-in-spatgris)

[8.4. OSC messages in ControlGRIS
[60](#osc-messages-in-controlgris)](#osc-messages-in-controlgris)

[8.5. Open Stage Control and Lemur
[60](#open-stage-control-and-lemur)](#open-stage-control-and-lemur)

[8.6. Uninstall [60](#uninstall)](#uninstall)

[8.6.1. SpatGRIS [60](#spatgris-2)](#spatgris-2)

[8.6.2. ControlGRIS [60](#controlgris-2)](#controlgris-2)

[9. Known issues and warnings
[61](#known-issues-and-warnings)](#known-issues-and-warnings)

[9.1. Known issues [61](#known-issues)](#known-issues)

[9.1.1. SpatGRIS, Mac version only.
[61](#spatgris-mac-version-only.)](#spatgris-mac-version-only.)

[9.1.2. ControlGRIS [61](#controlgris-3)](#controlgris-3)

[9.1.3. SpatGris, the plugin and SpatGRIS, the software
[61](#spatgris-the-plugin-and-spatgris-the-software)](#spatgris-the-plugin-and-spatgris-the-software)

[9.2. Reaper [61](#reaper)](#reaper)

[9.2.1. Mono tracks [61](#mono-tracks)](#mono-tracks)

[9.2.2. Device Preferences with Jack
[62](#device-preferences-with-jack)](#device-preferences-with-jack)

[9.3. Logic Pro [62](#logic-pro)](#logic-pro)

[9.3.1. Only one Surround output
[62](#only-one-surround-output)](#only-one-surround-output)

[9.3.2. Activate buttons [62](#activate-buttons)](#activate-buttons)

[9.4. Digital Performer 11 and Automated presets
[62](#digital-performer-11-and-automated-presets)](#digital-performer-11-and-automated-presets)

[9.5. Using SpatGRIS with live inputs
[62](#using-spatgris-with-live-inputs)](#using-spatgris-with-live-inputs)

[10. Tips and Tricks [63](#tips-and-tricks)](#tips-and-tricks)

[10.1. Acousmatic spatialisation
[63](#acousmatic-spatialisation)](#acousmatic-spatialisation)

[10.1.1. Mixing console [63](#mixing-console)](#mixing-console)

[10.1.2. Digital Audio Workstation
[63](#digital-audio-workstation)](#digital-audio-workstation)

[10.1.3. Acousmatic setup [63](#acousmatic-setup)](#acousmatic-setup)

[10.1.4. Scenario [64](#scenario)](#scenario)

[10.2. Using the PLAYER without you being present
[66](#using-the-player-without-you-being-present)](#using-the-player-without-you-being-present)

[10.3. HYBRYD mode to vary the trajectories
[66](#hybryd-mode-to-vary-the-trajectories)](#hybryd-mode-to-vary-the-trajectories)

[Index [68](#index)](#index)

**  
**

<img src="/media-en/media/image5.png"
style="width:1.02901in;height:1.02362in" />

# 1. General presentation

## 1.1. SpatGRIS is a spatialization tool

*SpatGRIS* does spatialization and localization. The spatialization
gives the listener the impression of being surrounded by the sound. It’s
an immersive experience. The localization is a way to place a sound at a
very precise place in the space. The two concepts can be used at the
same time in *SpatGRIS*.

### 1.1.1. Spatialization 

Using its two algorithms DOME or CUBE, *SpatGRIS* maps the sources —
which come from any audio software — to a speaker setup. The position of
the sources is provided by OSC messages. The spatialization is done
through a speaker system in a physical space.

### 1.1.2. Localization 

With the Direct Outputs options (independent or spatialized), *SpatGRIS*
makes it possible to access directly to the speakers, for example to
manage subwoofers, to place a sound on a particular speaker or to use a
channel-based approach to spatialization.

## 1.2. SpatGRIS is a recorder and a player

*SpatGRIS* allows recording the speaker outputs in spatialized modes
(DOME or CUBE) or two-channel modes (STEREO or BINAURAL) under two
standards - WAV, AIFF - and two formats - Mono Files or Interleaved.
With the PLAYER tool, *SpatGRIS* can play any multichannel works
recorded with it.

## 1.3. SpatGRIS makes speaker setups 

The speaker setup can adopt the form of a DOME or the free form of a
virtual CUBE.

### 1.3.1. DOME speaker setups

In the DOME, the distance between every speaker and the centre of the
DOME is fixed. Sound sources can be spatialized on the surface of the
DOME.

### 1.3.2 CUBE speaker setups

In the CUBE, speakers can be freely arranged in space. There is no fixed
distance between the speakers and the centre of the setup. Unlike DOME
setups, sound sources can enter, pass through, and exit the setup. Sound
sources that are outside the setup can be treated with attenuation
parameters (volume and filter).

## 1.4. The speakers can be part of the spatialization and the localization

Each loudspeaker has a unique number — whether in spatialized mode or as
a direct output — and can be used for these two functions:
spatialization and localization, thanks to the new direct output
functions. A speaker can be part of the spatialization and at the same
time be a direct output. This is a major conceptual difference compared
to previous version.

## 1.5. The three components of SpatGRIS

There are three components in *SpatGRIS* that are saved independently:
Project, Speaker Setup and Settings.

• Save Project. A project is coupled with a work and contains a certain
number of sources.

• Save Speaker Setup. A speaker setup is coupled with a physical
installation placed in a space.

• Save Settings. User settings are linked to a workstation (computer and
audio interface), including the stereo outputs used for stereo
reduction.

## 1.6. What’s new and improved in ControlGRIS/SpatGRIS?

• *SpatGRIS* is independent from any audio virtual device, either *Jack,
Enzian* or *BlackHole*. It’s the user’s choice.

• Direct Outs now have two functions: Independent, for speakers that are
not part of the spatialization, e.g. subwoofers; Spatialized, through
which the sound can be sent directly to any speaker that is part of the
speaker setup.

• Compatibility with the newest version of MacOS, from 10.15 (Catalina)
to 14.7 (Sonoma) and new machines (M1-M2-M3).

• ProTools compatibility with the addition of the *ControlGRIS* AAX
format*.*

• STEREO and BINAURAL can be assigned to any outputs of the sound card.

• Several speaker setups and projects templates are now integrated in
the software.

• *ControlGRIS* and *SpatGRIS* are available for Windows.

**What’s new:**

***SpatGRIS***

• Version 3.3.7

\- A general MUTE button has been added.

• Recent additions and patches

\- SpeakerView: Keep speaker numbers up-to-date

\- The 3D window representing speakers and sources is now independent of
*SpatGRIS*. The graphical representation is now done in *SpeakerView*,
with a much-improved graphical interface.

\- *SpatGRIS* and *BlackHole* are now 256 channels each.

\- CUBE Mode: Attenuation settings have a Bypass toggle button.

\- CUBE Mode: negative Z attenuation begins at the floor.

\- Stereo Reduction: Attenuation settings is functional in Stereo
reduction when in Cube or Hybrid mode.

\- Attenuation settings: They are saved with the projects.

\- Introduction of the PLAYER, a tool which allows *SpatGRIS* to be used
as a standalone software to play any piece recorded by it to any speaker
setup.

\- CUBE mode uses a new algorithm: MBAP (Matrix Based Amplitude
Panning).

\- Speaker Setup Edition in CUBE and HYBRID modes: added a Global Sound
Diffusion parameter.

\- Introduces theHYBRID mode that combines the DOME and the CUBE
algorithms.

\- Show numbers has been split into Show Source Numbers and Show Speaker
Numbers.

***ControlGRIS***

• Version 1.4.5

\- Fixes different issues with the Windows installer

\- Provides the possibility to place signals outside the CUBE on the Z
axis.

**Improvements and Fixes**

• The Speaker Setup Edition has been greatly optimized.

• Better compatibility in the parameters between *ControlGRIS* and
*SpatGRIS.*

• A lot of very practical enhancements and changes in the terminology!

## 1.7. Groupe de Recherche en Immersion Spatiale (GRIS)

Director: Robert Normandeau.

Main programmer: Gaël Lane Lépine.

Consultant: Devin Roth, creator of BlackHole.

Assistant.es: Nicola Giannini.

Former programmers: Samuel Béland, Olivier Bélanger, Vincent Berthiaume.

Former assistants: Simone d’Ambrosio, Theo Mathien, Raphaël
Néron-Baribeau, Ofer Pelz, Dominic Thibault, Alexis Langevin-Tétrault,
Vincent Monastesse, David Ledoux, Yohan Brimicombe, Christophe Lengelé,
Mélanie Frisoli, David Piazza, Gabrielle Caux..

Former trainees: Ludovic Laffineur, Antoine Landrieu, Nicolas Masson,
Hicheme Ben Gaied.

The GRIS received research grants from Hexagram, SSHRC and FRQSC since
2008 and up to 2025.

Thanks to Yohan Brimicombe for the creation of the web site:
<http://gris.musique.umontreal.ca>

# 2. INTRODUCTION

These instructions assume that you are familiar with the following
tools:

• The DAW you use, which must support AU, VST, VST3 or AAX plugins.

• Your audio interface.

## 2.1. Architecture

The *SpatGRIS* system is made of three elements:

• The *ControlGRIS* plugin where the trajectories are designed and
recorded in a DAW (or any OSC device).

• The *SpatGRIS* itself that spatializes the sound, according to the
setup of the speakers done in the Speaker Setup Edition window.

• The virtual audio device *BlackHole*[1] which connects the DAW to
*SpatGRIS*.

The whole architecture, including these elements, looks like this (audio
and OSC are working in parallel):

<img src="/media-en/media/image6.png"
style="width:4.69671in;height:3.15in" />

NOTE: In each track of the DAW, it’s mandatory that the audio output
channel numbers match the OSC source numbers (set by the First Source ID
parameter) in the corresponding ControlGRIS instance to have the sound
to be spatialized in *SpatGRIS*. Failure to do so will lead to silence
or frozen spatialization.

## 2.2. SpatGRIS

*SpatGRIS* is a standalone application that allows the spatialization of
sounds on different speaker configurations, in 2D or 3D. It could be
used with the virtual audio interface *BlackHole* that may provide up to
256 inputs and outputs. The trajectories are sent from the *ControlGRIS*
plugin, or from any other OSC software[2] to *SpatGRIS*. The audio
spatialization itself is performed by *SpatGRIS* and sent to the audio
interface.

### 2.2.1. History

The development of *SpatGRIS* began in 2020. It is a rewritten version
of *ServerGris* (2018) and *SpatGRIS2* (2020). The first official
version of *SpatGRIS* is 3.0.0 and was released in August 2021. It was
our first *Jack*[3] free spatialization tool!

### 2.2.2. System requirements

The software has been tested on the following OS:

• macOS from 10.15 Catalina™ to 14.7 Sonoma™

• It is native on Apple Silicon M1-M2-M3 machine (version 3.1.8 and up).

• Windows™ 10, 11.

### 2.2.3. Installation notes

• Download the latest version of *SpatGRIS* from SourceForge:

[https://sourceforge.net/projects/SpatGRIS3/](https://sourceforge.net/projects/spatgris3/)

*SpatGRIS* for Mac comprises two installers in the same folder:

SpatGRIS_v3:

• *SpatGRIS* itself.

• *SpeakerView* in three versions: Forward (recommended), Compatibility
and Mobile

• *ControlGRIS* as a compressed folder with the different formats of the
plugin.

BlackHole:

• The virtual audio device *BlackHole* that provides 64, 128 or 256
audio channels between the DAW and *SpatGRIS.*

Notes for MacOS users

• *SpatGRIS*, along with *SpeakerView* and a folder of utilities, are
now installed in a GRIS folder (in the Applications folder). It is
possible to rename the GRIS folder (to have multiple installations, for
example), but it is not advisable to rename anything inside this folder.

• To facilitate focus management between *SpeakerView* and *SpatGRIS*,
we recommend that you allow *SpeakerView* to control your computer when
requested. If *SpeakerView* does not request this, go to System Settings
\> Privacy & Security \> Accessibility, and authorize *SpeakerView*.

*SpatGRIS, SpeakerView, ControlGRIS* and *BlackHole* will be updated
separately. Please subscribe to our newsletter to be informed about the
software updates on our web site.

Two external controllers are available for *ControlGRIS*:

• An Open Stage Control patch for iPad™.

• A Lemur patch[4] for iPad™.

An Addendum manual pertaining to these *iPad* controllers is available
on SourceForge.

*SpatGRIS* for Windows has one installer:

• *SpatGRIS* itself.

• *ControlGRIS* as a compressed folder with the different formats of the
plugin.

There is no Windows version of *BlackHole*. For Reaper™ users, there is
the *ReaRoute* function which works similarly to *BlackHole*, but only
for Reaper. It is possible to use *Jack* on Windows[5]. When *BlackHole*
is mentioned in the manual, replace it by *ReaRoute* or *Jack* when
using Windows.

### 2.2.4. Access to the microphone

NOTE: Very important for Catalina (10.15) users and up.

Make sure that *SpatGRIS* has access to the microphone in the System
Preferences, Security & Privacy:

<img src="/media-en/media/image7.jpg"
style="width:1.9711in;height:1.69291in" />

### 2.2.5. BlackHole volume at 0 dB

After installing or reinstalling Blackhole, please make sure that the
volume of BlackHole is at 0 dB in the Audio Midi Setup.

<img src="/media-en/media/image8.jpg"
style="width:5.59231in;height:1.49606in"
alt="A screenshot of a chat Description automatically generated with low confidence" />

### 2.2.6. New Users of BlackHole and macOS 14 Sonoma

NOTE: New users of BlackHole and macOS 14 Sonoma should use the latest
BlackHole installer 0.6.0.

## 2.3. ControlGRIS

*ControlGRIS* is an OSC[6] plugin available in AU, VST, VST3 and AAX
formats (Mac) and VST and AAX formats (Windows). This free and
open-source plugin sends OSC data to *SpatGRIS* to spatialize multiple
sound sources on a variable set of speakers. Different modes of source
links and a trajectory system are provided for spatialization of mono,
stereo and multichannel sources (up to eight channels).

### 2.3.1. History

The development of *ControlGRIS* began in 2019. It was inspired by three
older plugins, *OctoGris* (2010), *ZirkOSC* (2012) and
*SpatGris1*(2017). The first version (1.1.0) was released in April 2020.

### 2.3.2. System requirements

The software has been tested on the following OS and DAWs:

• macOS from 10.15 Catalina™ to 14.7 Sonoma™; Digital Performer™ 10 and
11; Ableton Live™ 10 and 11; Logic Pro™ 10; Reaper™ 6; Pro Tools™
2023.6.

• It is native on Apple Silicon M1-M2-M3 machines (version 1.3.2 and
up).

• Windows™ 10, 11; Reaper™ 6.

### 2.3.3. Installation notes 

Download the latest version of *ControlGRIS* from SourceForge (the
installer is included in the *SpatGRIS* installer):

<https://sourceforge.net/projects/spatgris3/>

Decompress the downloaded file. The different formats will be installed
in their proper location. *ControlGRIS* appears under the “UdeM” folder
of your host application.

### 2.3.4. AU, VST, AAX

Mac versions were intensively tested but the Windows 10 and 11 versions,
not so much!

Comments are welcome.

Here are some particularities:

• Use the AU version in DP and Logic Pro on the Mac.

• Use the VST3 version in Reaper and Live.

• Use the AAX version in ProTools[7].

• Refer to the manual of your preferred DAW to determine which version
is better.

## 2.4. Quick Start Guide

*SpatGRIS* receives Open Sound Control (OSC) data from *ControlGRIS*, to
spatialize the sounds within a set of speakers. The sound itself is sent
from the DAW to *SpatGRIS* via *BlackHole*.

Don't need/want to read the manual? Here are the basic steps to
spatialize a stereo track on a 64-output audio interface.

NOTE: Adjust the Buffer size to the same value in both your DAW and
SpatGRIS. A value of 256 and up is recommended.

1\. Open *SpatGRIS.*

2\. Open the Settings (File menu) or click them directly in the Info bar
and assign the Audio input device to *BlackHole 128ch* and the Audio
output device to your audio interface (you must do that only the first
time). Close the window.

<img src="/media-en/media/image9.jpg"
style="width:1.56193in;height:1.5748in" />

3\. Open a DOME Speaker Setup (File menu) or use the default one.

4\. Open your DAW.

5\. Assign the audio output of your DAW to *BlackHole 128ch.*

6\. Create a stereo track and assign the outputs *to BlackHole 128ch
1-2.*

7\. Insert a *ControlGRIS* plugin on this track and set it to DOME mode.

8\. The number of sources should be already initialized and set at 2 and
First Source ID set at 1.

9\. Select *Circular Fully Fixed* in *Sources Link* and start the
sequencer.

10\. Play with Source No. 1 and see the result in *SpatGRIS.*

11\. The colour of the sources are the ones selected in the Sources (the
red dots in this example).

You are now ready to play and record automation.

<img src="/media-en/media/image10.png"
style="width:5.02968in;height:3.54in" />

<img src="/media-en/media/image11.png"
style="width:4.89639in;height:5.05in" />

NOTE: In each track of the DAW, it’s mandatory that the audio output
numbers match the OSC numbers (set by the First Source ID parameter) in
the corresponding ControlGRIS to have the sound to be spatialized in
SpatGRIS. Not doing that will lead to silence, or to freeze
spatialization.

Questions? Details? Read the manual!

This manual is in the Help menu:

<img src="/media-en/media/image12.jpg"
style="width:1.81222in;height:0.7in" />

###  

# 3. Connections

## 3.1. Connect the DAW to SpatGRIS 

### 3.1.1. Open SpatGRIS

The first time you open *SpatGRIS*, you'll have to:

• Determine the numbers of sources (up to 256). 64 would be enough in
most cases, but fewer sources mean less CPU load. Or use one of the
projects included in the Templates menu.

• Design a speaker setup or use one in the Templates menu.

After these first two steps, save the Speaker Setup and the Project. At
the next start-up of SpatGRIS, the last saved Speaker Setup and Project
will be loaded.

### 3.1.2. Adjust the output level

By default, the output level of *SpatGRIS* is set to unity gain: 0.00
dB. It may need to be attenuated or increased, especially if it is the
first time you try the system!

### 3.1.3. Assign the DAW to BlackHole

Open your DAW and assign *BlackHole* as the audio output device*.*
*BlackHole* should be detected like any other audio interface in Core
Audio. It is possible to allocate a certain number of active channels
according to the number set in Set Sources (± icon).

<img src="/media-en/media/image13.png"
style="width:4.90635in;height:2.2in" />

### 3.1.4. Multiclient

*SpatGRIS* is a multiclient software, which means that it can connect to
multiple audio software at the same time. Keep in mind, though, that its
primary usage is to spatialize sounds coming out of a single DAW. The
software receives two types of information:

• Audio signals from *BlackHole*

• OSC data from *ControlGRIS*.

Both signals are needed for the sound spatialization. For direct
outputs, only the audio signal is needed.

If you use only one DAW, there is no problem, but it’s mandatory that
the audio output numbers match the OSC numbers (set by First Source ID
parameter) in the corresponding *ControlGRIS* to have the sound to be
spatialized in *SpatGRIS*. Not doing that will lead to silence, or to
freeze spatialization. Things become a little bit more complicated if
you intend to use more than one software at a time.

• *BlackHole* has a limited number of 256 channels in total. If you want
to connect a DAW with 24 channels and another one with 8 channels, keep
in mind that the second DAW will have to be set to channels No. 25-32 in
*BlackHole* andand it will be necessary that ControlGRIS uses the
corresponding OSC numbers.

NOTE: Adjust the Buffer size to the same value in both your DAW and
SpatGRIS. A value of 256 and up is recommended.

## 3.2. Connect ControlGRIS to SpatGRIS

### 3.2.1. Numbering audio and OSC

The spatialization is handled by *SpatGRIS* which receives OSC data from
*ControlGRIS2*. It is mandatory to synchronize *BlackHole* audio output
numbers in the DAW with the OSC numbers in *ControlGRIS2*.

In the following example, three stereo tracks (red, blue, and green) are
assigned to *BlackHole* channel pairs 1-2, 3-4 and 5-6. The three
instances of *ControlGRIS2* use the same OSC numbering: 1-2, 3-4 and
5-6.

<img src="/media-en/media/image14.png"
style="width:4.82117in;height:5.12in" />

To help to keep things clear, it is recommended to use the same colour
scheme in the DAW and in *SpatGRIS*.

<img src="/media-en/media/image15.png"
style="width:4.98084in;height:3.3in" />

NOTE: If by mistake, you are using the same OSC numbers in more than one
ControlGRIS instance, the sources in SpatGRIS will oscillate between
different positions because they will receive two (or more) of the same
position from different *ControlGRIS*. It's a good indicator that
something is wrong.

### 3.2.2. Sources Colour

The colour of the sources can be set to any value by clicking in the
colour square. It opens a window where you can set the parameters of the
colour. This is the colour you will see in the 2D or the 3D window. If
you use a lot of sources, it is recommended that you design your colour
set carefully.

After closing this window, you can set the same colour to the next
source on the right by using right-clicking on a colour. You can set
this way the same colour to a pair of sources or to many contiguous
sources.

<img src="/media-en/media/image16.jpg"
style="width:2.3622in;height:1.9685in" />

# 4. ControlGRIS

*ControlGRIS* is an OSC plugin that offers two possibilities, according
to the mode chosen in *SpatGRIS*:

• DOME.

• CUBE.

These two modes will be explained in detail in the *SpatGRIS* section.

## 4.1. Introduction

*ControlGRIS* is an OSC spatialization plugin. This plugin allows
movements of multichannel sound sources on a variable set of speakers.
Several sources link modes and a trajectory system are provided to allow
the spatialization of mono, stereo, quad, 5.1 or multichannel sources of
up to eight channels. *ControlGRIS* doesn't handle audio, only data
which is sent to *SpatGRIS*. The audio itself is sent from the DAW
directly to *SpatGRIS via BlackHole*.

This document describes the operating instructions and functions
specific to *ControlGRIS*. It is assumed that the user has a working
knowledge of the host software and can perform basic functions to
configure it.

## 4.2. Graphical interface

The graphical interface allows the placement of the sound sources. It is
slightly different in DOME than in CUBE mode. In DOME, since the
Distance is fixed at 1.00, there are only the Azimuth and Elevation
parameters to adjust. In CUBE, the three parameters, Azimuth-Distance
and Elevation are adjustable on two different windows.

<img src="/media-en/media/image17.png"
style="width:6.38128in;height:4.6in" />

## 4.3. Configuration panel

The configuration panel gives access to different plugin parameters.
These settings are grouped under three tabs: Sources, Settings and
Controllers.

<img src="/media-en/media/image18.jpg"
style="width:4.02869in;height:1.2in" />

### 4.3.1. Settings

#### MODE

The DOME mode is based on the VBAP algorithm designed by Ville Pulkki.
In this mode, the space is represented by a dome where the distance
between every point of the surface to the centre of the dome is equal to
1.00.

The CUBE mode is based on an original MBAP[8] algorithm designed by Gaël
Lane Lépine. In this mode, the space is represented by a cube within
which it is possible to design any kind of speaker setup.

#### OSC Port

This is the OSC port number for communication between *ControlGRIS* and
*SpatGRIS*. They should be set to the same one. 18032 is the default
value.

#### IP Address

The default value here is 127.0.0.1 which corresponds to the address of
the internal device (i.e. your computer). This can be changed to send
the OSC to an external computer.

#### Number of Sources

The number of sources per track corresponds to the number of audio
channels in the track. The number is limited to eight channels (as it is
in most DAWs).

#### First Source ID

This number must be unique and different for each audio channel. You
must use the same numbers for audio and for OSC.

If you have only mono tracks, the numbers are successive. If you have
stereo tracks, you'll have only odd numbers to put here: 1, 3, 5, etc.
because the even numbers are set automatically to the right channel of
each stereo track. And if you work with octophonic sound files, the
first source ID will be 1, the second octophonic track will start at 9,
etc.

### 4.3.2. Sources

Under the Sources tab, it is possible to accurately position sources by
using the graphical interface or the text boxes. Using Sources
Placement, it is possible to position sources equidistantly, following a
clockwise or alternate order. To do so, simply select the desired layout
from the drop-down menu.

<img src="/media-en/media/image19.jpg"
style="width:1.72747in;height:1.25984in" />

Moreover, it is possible to manually adjust the position of each source
by entering its polar (DOME) or Cartesian (CUBE) coordinates. From the
Source Number drop-down menu, first select the number of the source to
be moved. Then, enter its new coordinates.

In DOME, Elevation and Azimuth correspond to the current polar
coordinates of the selected source:

<img src="/media-en/media/image20.jpg"
style="width:4.13386in;height:1.1811in" />

In CUBE, X, Y, and Z correspond to the current Cartesian coordinates of
the selected source:

<img src="/media-en/media/image21.jpg"
style="width:4.13386in;height:1.1811in" />

**NOTE: Manual positioning of individual sources only works when the
Independent mode is chosen under Sources Link.**

### 4.3.3. Controllers

<img src="/media-en/media/image22.png"
style="width:4.16in;height:1.28213in" />

*ControlGRIS* can be manipulated via an external Open Sound Control[9]
(OSC) controller. There is an interface made for Open Stage Control and
one made for Lemur to manipulate *ControlGRIS* parameters from an
iPad[10].

• OSC output plugin ID: to control different instances of *ControlGRIS*,
each one should have a different ID.

• Receive and Send should be set accordingly to the proper OSC channels
(Default: 9000 and 8000).

• IP port addresses should be set accordingly to your Wi-Fi network,
either public or local[11]. Both the computer and the controller should
be on the same network. *ControlGRIS* automatically receives the input
address from your network.

## 4.4. Spatialization views

*ControlGRIS* works in two different modes for sound spatialization:
DOME and CUBE.

### 4.4.1 View in DOME mode

In DOME mode, the graphical interface is limited to Azimuth-Elevation.
In this mode, the sound is spatialized on the surface of the dome.
Whereas a source placed in the centre is at the top of the dome, a
source placed at the periphery is at the bottom of the dome.

The dome is represented here from the top, examples with a stereo source
on the left, an octophonic source on the right:

<img src="/media-en/media/image23.jpg"
style="width:2.5in;height:1.51736in" /><img src="/media-en/media/image24.jpg"
style="width:2.5in;height:1.5211in" />

### 4.4.2. Spans in DOME mode

In both modes, Span parameters are available for azimuth and elevation.
Span spreads the signal to a larger zone than just the source itself. In
DOME mode, the spans look like an arc on each side of the source:

<img src="/media-en/media/image25.jpg"
style="width:2.5in;height:1.51969in" /><img src="/media-en/media/image26.jpg"
style="width:2.02551in;height:1.52in" />

### 4.4.3. View in CUBE mode

In CUBE mode, the graphical interface is divided between two screens:
Azimuth-Distance and Elevation. The CUBE mode adds distance and allows
moving a sound inside or outside the speaker setup (represented by the
internal white square). The CUBE is represented from the top on the left
and in profile on the right (the 3D view shows only in *SpatGRIS*).
Examples for stereo and octophonic sources:

<img src="/media-en/media/image27.jpg"
style="width:2.53063in;height:1.52in" />
<img src="/media-en/media/image28.jpg"
style="width:2.50435in;height:1.52in" />

### 4.4.4. Spans in CUBE mode

In CUBE mode, the spans look like a cylinder wrapped around the source:

<img src="/media-en/media/image29.jpg"
style="width:2.46662in;height:1.5in" /><img src="/media-en/media/image30.jpg"
style="width:1.75084in;height:1.5in" />

In some CUBE setups, where most speakers are spread across the walls and
the ceiling, a source can be lost in the centre of the hall. If you wish
to create a flat sound disk that activates only the speakers located at
the same height as the source, you can add a bit of Azimuth Span:

<img src="/media-en/media/image31.jpg"
style="width:6.15in;height:1.95144in" />

### 4.4.5. CUBE Elevation in Normal or Extended Top mode

Since version 1.4.1, *ControlGRIS* offers the possibility to put a
source outside of the CUBE in elevation. This was already possible on
the *x* and *y* axes, and it is now possible on the *z* axis. When using
the Extended Top mode, a white horizontal line appears in the elevation
diagram. This line represents the value 1.0 used in the Normal mode.
This is the point at with *SpatGRIS* Attenuation Settings start to take
effect in elevation. Sources will be filtered either in volume and/or in
frequencies as they move further away from the top of the cube:

<img src="/media-en/media/image32.jpg"
style="width:6.15in;height:1.91268in" />

### 4.4.6. CUBE Elevation in Extended Top and Bottom mode

A second line appears in Extended Top and Bottom mode to attenuate the
sounds that are sent below the floor (for the lucky few who have access
to a full cube!) The top line represents the value 1.0 of the normal
mode. The bottom line represents the value 0.0 of the Normal mode:

<img src="/media-en/media/image33.jpg"
style="width:6.15in;height:1.90611in" />

NOTE 1: Older projects can still be used in the Normal mode where the
full range from 0.00 to 1.00 is still available.

NOTE 2: It's not yet possible to go below the floor in a complete sphere
with ControlGRIS in DOME mode. We are working on that. But it's possible
to do so by using any software that sends OSC directly to SpatGRIS.

## 4.5. How to use ControlGRIS

*ControlGRIS* is a plugin that can be inserted on any track that
requires spatialization. *ControlGRIS* comprises a trajectory system
that can write predefined movements quickly and efficiently. The
automation function of the host software assures the recording and
playback of the source's movements. It is therefore essential to
understand the various automation modes in your preferred host.

### 4.5.1. Load the plugin on a track

*ControlGRIS* is loaded similarly to any other AU or VST plugin. Most
often, *ControlGRIS* is loaded at the end of the insert chain of the
track.

NOTE: In each track of the DAW, it’s mandatory that the audio output
numbers match the OSC numbers (set by the First Source ID parameter) in
the corresponding ControlGRIS to have the sound to be spatialized in
SpatGRIS. Not doing that will lead to silence, or to freeze
spatialization.

### 4.5.2. Save presets and recording automation

It is possible to save some of the *ControlGRIS* plugin parameters
within the 50 provided preset slots. The shortcuts are:

• Shift-Click Preset number: Save.

• Click Preset number: Load.

• Opt[12]-Click Preset number: Delete.

These functions appear below the rows 49-50:

<img src="/media-en/media/image34.jpg"
style="width:0.68056in;height:0.65278in" />

These presets allow you to save and recall the following parameters
only:

• Source positions (Azimuth-Distance-Elevation). These can also be
automated.

The parameters that are not saved but can be automated:

• Spans.

• Sources Link and Sources Link Alt.

• Presets.

• Bypass.

The parameters that are not saved and not automated, because they are
used to automatically generate a trajectory that will be written by the
DAW itself:

• Spans link.

• Trajectory Type.

• Dur per cycle.

• Sec(s)/Beat(s).

• Number of cycles dampening.

• Deviation degrees per cycle.

• Back & Forth.

• Activate.

Configuration tab

• The whole Configuration tab is not saved in the preset (this one is
saved with the DAW project). It is not a good idea to change these
settings within a track.

NOTE: While it is possible to record the position of all sources in
presets, it is only possible to record the automation of the source No.
1 in the sequencer. Source No. 1 is the leader while other sources are
followers.

### 4.5.3. Recall presets

As mentioned above, the presets store only the position of the sources.
When a preset is loaded, the sources are positioned according to the
stored data. Keep in mind though that the sequencer also has a memory of
the previous position of the sources, and both can interact strangely.
Very often then, it's only when you start the sequencer that the sources
take their real positions. To avoid any ambiguity, presets selection can
be automated.

## 4.6. Trajectories

<img src="/media-en/media/image35.jpg"
style="width:4.13386in;height:1.1811in" />

It is possible to automate the movement of sound sources using
predefined trajectories. Within the Trajectories control panel, you can
set and adjust these movements to the musical context. The concept
behind the trajectories is that there is a source leader while the
others are followers. Only the source No. 1 can be the leader.

If you try to record the automation of any other source than No. 1,
you’ll get this warning:

<img src="/media-en/media/image36.jpg"
style="width:4.13386in;height:1.1059in" />

### 4.6.1. Sources Link

Independent mode is only available for initially placing sources
independently in a multichannel track. But the position of sources can't
be automated independently. Only the automation of the Source No. 1 can
be recorded. Therefore, after placing the sources, a different source
link should be chosen before recording the automation.

#### Azimuth-Elevation (DOME) and Azimuth-Distance (CUBE) Links

Within the *Trajectories* section, under the *Sources Link* drop-down
menu, it is possible to choose different ways of linking sources
together. Depending on the number of channels, some links may not be
available:

• Mono: Independent only.

• Stereo: all links.

• Multichannel: all but Symmetric X and Y.

• Detailed representations of the Azimuth-Elevation and Azimuth-Distance
Links are shown at the Addendum 8.1.1.

<img src="/media-en/media/image37.jpg"
style="width:4.13386in;height:1.1811in" />

#### Elevation Links (CUBE mode only)

In CUBE mode, the Elevation Links between sources are independent from
the Azimuth-Distance parameters.

• Detailed representations of the Elevation Links are shown at the
Addendum 8.1.2.

<img src="/media-en/media/image38.jpg"
style="width:4.13386in;height:1.1811in" />

### 4.6.2. Trajectory Type

Automating the movement of a source is quite simple with the different
trajectory types provided.

• Detailed representations of the Trajectories are shown at the Addendum
8.2.

#### Azimuth-Elevation (DOME) and Azimuth-Distance (CUBE) Trajectory Type

A drop-down menu allows you to select from different types of
trajectories such as *Circle*, *Ellipse*, *Spiral*, *Square* and
*Triangle,* either in *Clockwise* or *Counter Clockwise* mode.

<img src="/media-en/media/image39.jpg"
style="width:4.1378in;height:2.33326in" />

#### Elevation (CUBE only) Trajectory Type

A drop-down menu with different types of trajectories allows you to
select from a variety such as *Up Down*, *Down Up.*

<img src="/media-en/media/image40.jpg"
style="width:4.13in;height:1.24915in" />

#### Other settings

• The duration of the trajectory in *second(s)* or *beat(s)* (linked to
the MIDI tempo of the host sequencer).

• The Number of cycles dampening: the total duration = Dur per cycle x
Number of cycles x 1,5. Dampening works only with Back & Forth.

• The Back & Forth option.

• The Deviation degrees per cycle.

#### Realtime

This is the usual automation recording: you move a parameter (or several
parameters) and it is recorded in the DAW.

#### Drawing

The Drawing mode allows you to draw a trajectory directly into the
plugin itself. This trajectory can then be modified by editing the
duration, dampening and deviation. When the desired settings are found,
they can be recorded in the DAW itself.

<img src="/media-en/media/image41.png"
style="width:5.28684in;height:3.5in" />

The Drawing mode is a freehand mode. When you select it, a light grey
cross will appear with which you draw a trajectory. The timing of the
trajectory and the design are temporarily stored within the plugin. In
Azimuth-Elevation (DOME) or Azimuth-Distance (CUBE), it's the position
that is recorded. In Elevation (CUBE only) it's the position over time.
Both windows share a cycle that can be modified with the regular
parameters. To see the trajectory in action, you can turn on the
Activate buttons and play the sequence. When the sequencer stops, the
Activate buttons return to off. Changes can be made and then it's
possible to switch on Activate again. Once satisfied with the results,
you can then record the trajectory in the DAW.

#### Shift-Click in Drawing mode

If Shift is pressed in the Drawing mode, it's possible to design
straight lines or irregular geometrical figures in the Azimuth-Elevation
(DOME) or the Azimuth-Distance (CUBE) window. Every time you click, a
new angle is created. Don't forget to click one last time once you’re
finished!

<img src="/media-en/media/image42.jpg"
style="width:1.31862in;height:1.40157in" /><img src="/media-en/media/image43.jpg"
style="width:1.31304in;height:1.4in" />

**NOTE: Be careful with the freehand trajectory because it’s temporary.
If you click anywhere in the window after drawing a trajectory, or close
the plugin or the session, it will automatically be erased. Only one
gesture can be temporarily recorded at a time. The X cross can be hidden
behind one of the sources. Just move one of those to find it back.**

#### Activate

<img src="/media-en/media/image44.jpg"
style="width:4.12043in;height:1.1811in" />

Pressing the Activate button makes *ControlGRIS* wait for the start of
the sequencer. When the sequence is initiated, the plugin will start the
trajectory according to the specified settings. The movement produced
can be recorded — X, Y and Z-coordinates of the source No. 1 — like any
other automation. When the sequencer stops, the *Activate* buttons
return to off. It's important to put the play head at the right position
before pressing on the activate button and putting the sequence into
play.

#### Trajectory recording in the DAW

As explained above, *ControlGRIS* waits for the host sequencer to start
before starting a trajectory. The tracks that contain *ControlGRIS* can
be set in a write mode (Touch, Latch, or Write — depending on the
options within your DAW) to record the sources' movements as automation.
This automation is then available for playback and editing.

NOTE: Only the source No. 1 (leader) is recorded, the other sources
being followers. It is always preferable to record the automation of
trajectories in the DAW after you have found the right settings, because
it frees up the CPU used by ControlGRIS.

### 4.6.3. A special case: the pendulum

A specific use of the Shift-Click in Drawing mode can be used to design
a pendulum. If a simple line is drawn with Shift-Click, it constitutes
the basic element of a pendulum. Then the Dur per cycle, Dampening,
Deviation and Back & Forth can be used to make this pendulum very
interesting. It can be placed anywhere in the space.

<img src="/media-en/media/image45.jpg"
style="width:1.29042in;height:2.3622in" />

### 4.6.4. Presets and automated trajectories

It's possible to record the presets selection in the sequencer. But to
avoid contradictory information between automated trajectories and
automated presets (which stores x-y position of the sources), in
automation recording, the x and y coordinates, registered in the preset,
will be automatically written in the x-y automation curves. The
automated presets are designed essentially to offer the possibility to
apply sudden changes in the position of the sources.

<img src="/media-en/media/image46.png"
style="width:5.56203in;height:3.46457in" />

NOTE: Be careful with that. If you overwrite the already existing X and
Y automations, they might become in competition with the information
stored in the presets. Then you will certainly get audio glitches.

# 5. SpatGRIS 

• *SpatGRIS* does spatialization and localization.

• *SpatGRIS* is a recorder and a player.

• *SpatGRIS* makes speaker setups.

## 5.1. Introduction

There are three components in *SpatGRIS* that are saved independently:
Project, Speaker Setup and Settings.

• **Save Project**. A project is coupled with a work that contains a
certain number of sources (outputs from the DAW) and the Mode used. This
is the component on the top right of *SpatGRIS*.

• **Save Speaker Setup**. A speaker setup is coupled to an installation
placed in a space and the algorithm used. This is the section shown in
*SpeakerView*.

• **Save Settings**. User settings are linked to a workstation —
computer and audio interface — including the stereo outputs used for
stereo reduction (even without showing them). Most of the settings are
shown in the Info bar. Click the Info bar or Settings in the File menu
(Cmd-,).

NOTE: The DOME and the CUBE modes are saved in Speaker Setups and
Projects, but the HYBRID mode is only saved in projects. The last opened
document — whether it be a Speaker Setup or a Project — determines the
Mode.

The *SpatGRIS* window is divided into different zones:

• Sources

• VU Meters.

• Settings and Info.

• Controls.

• Recording.

*SpeakerView* shows the speakers in a 3D view.

<img src="/media-en/media/image47.png"
style="width:6.5in;height:3.8681in" />

## 5.2. SpeakerView

As of *SpatGRIS* version 3.3.3, the 3D representation of loudspeakers is
supported by an independent application called *SpeakerView.* This
change was necessary in order to meet the requirements of Apple Silicon
processors for Mac. Everything is better here: speaker transparency,
number legibility and fluidity of movement have all been dramatically
improved.

*SpeakerView* is shown here with the new Show Hall function:

<img src="/media-en/media/image48.jpg"
style="width:3.32465in;height:3in" />

### 5.2.1. Visibility and keyboard shortcuts

*SpeakerView* is displayed independently of *SpatGRIS*. By default, it
is displayed at the same time as *SpatGRIS*. However, it can be opened
or closed independently (Mac: Opt-V. Windows: Alt-V).

Keyboard shortcuts in the *SpatGRIS* View menu control display options
in *SpeakerView*:

<img src="/media-en/media/image49.jpg"
style="width:1.6in;height:2.38881in" />

### 5.2.2. Two distinct applications

Although *SpeakerView* resembles the 3D representation that existed in
versions *of SpatGRIS* prior to 3.3.0, it is a separate application. It
can be moved and sized independently. You can also choose to force it to
stay on top of *SpatGRIS* (Keep SpeakerView On Top).

NOTE: SpeakerView is an autonomous application, but there is no need for
the user to worry about that, *SpatGRIS* will take care of everything.
We even strongly recommend that *SpeakerView* shouldn't be started
neither from the Finder nor the Dock. If it's opened this way, this the
warning message that will pop up:

<img src="/media-en/media/image50.jpg"
style="width:1.22256in;height:1in" />

## 5.3. Change the setup not the spatialization

The most interesting feature in *SpatGRIS* is that the *Sources,* which
come from the DAW and represent the audio and the spatialization of your
work, are independent of the *speakers*. So, if you initially defined a
very complex spatialization structure for a specific speaker
arrangement, you could play it on any other speaker setup afterwards,
especially in DOME mode. You simply have to change the Speaker Setup
from one location to the next.

Here's an example of a piece designed for a 16-Speaker Setup (on the
left), presented on an entirely different 24-speaker system (right),
simply by switching from one system to the other.

As you can see, all the sources remain at the exact same coordinates.
They will be played by different speakers but heard at the same location
in the concert hall.

<img src="/media-en/media/image51.jpg"
style="width:2.52231in;height:3.14961in" /><img src="/media-en/media/image52.jpg"
style="width:2.52292in;height:3.14931in" />

## 5.4. Settings

<img src="/media-en/media/image9.jpg"
style="width:1.95241in;height:1.9685in" />

Audio Settings

• Audio device type: Core Audio (default).

• Audio input device: *BlackHole* (ideally).

• Audio output device: your audio interface.

• Sampling Rate (Hz): from 44100 to 192000, according to your audio
interface.

• Buffer Size (spls): from 16 to 2048. Adjust the Buffer size at the
same value in your DAW and in *SpatGRIS*.

General Settings:

• OSC Input Port: default is 18032 which is the same as *ControlGRIS*.
If you want to use another incoming OSC device, use this port number as
the output port of that device, otherwise you must change this number
accordingly.

**Close**

Your settings are automatically saved. Under the name of the version of
*SpatGRIS,* the document is located here (Mac):

• ~/Library/Application Support/GRIS/SpatGRIS.0.0 (for example).

## 5.5. Controls

<img src="/media-en/media/image53.png"
style="width:6.375in;height:3in" />

## 5.6. The DOME and the CUBE

In DOME mode, it is possible to place the sources on the surface of the
dome made by the speaker setup while in CUBE mode it is possible to move
and place the sources inside and outside the speaker setup.

### 5.6.1. DOME

The DOME based on VBAP (Vector Base Amplitude Panning), allows the user
to spatialize the sound on a dome of speakers according to the relative
amplitude of three speakers (as opposed to two in stereo panning).
Therefore, the dome is made of triangles of speakers. This way, the
sound can travel smoothly on the surface of the dome, with no bumps or
holes.

It is possible to see the triangles by choosing Show Speaker Triplets
(Opt-T) in the *View* menu. If you have the chance to use a complete
sphere, it is possible to show it (Opt-O)!

<img src="/media-en/media/image54.jpg"
style="width:2.98251in;height:2.35in" /><img src="/media-en/media/image55.jpg"
style="width:2.48066in;height:2.35in" />

### 5.6.2. CUBE

Since version 3.2.0, the CUBE is based on the MBAP algorithm (Matrix
Base Amplitude Panning) and it allows the placement of a source anywhere
in a space represented by a cube. But it is not limited to the shape of
a cube. Any speaker setup can be placed within a cube (including a
dome!) Therefore, any sound installation or concert situation can be
simulated here. In CUBE mode, the distance of the source exiting the
speaker setup is considered to simulate the natural behaviour of the
sound moving away.

As the name suggests, the algorithm is based on a precomputed
three-dimensional matrix of multiple points per speaker that determines
the amplitude of a source at a specific position.

<img src="/media-en/media/image56.jpg"
style="width:3.03429in;height:2.36in" /><img src="/media-en/media/image57.jpg"
style="width:2.13694in;height:2.36in" />

## 5.7. The HYBRID mode: DOME and CUBE in the same project

The HYBRID mode is not really a new algorithm, but a combination of the
DOME and the CUBE ones. HYBRID mode can be selected in the Algorithm
section:

<img src="/media-en/media/image58.jpg"
style="width:1.60417in;height:0.5in" />

The Sources menu is then changed to offer the possibility of choosing
between the dome or the cube behaviour independently for each source:

<img src="/media-en/media/image59.jpg"
style="width:2.48684in;height:0.9in" />

The HYBRID mode uses the DOME algorithm, which means that the speaker
setup must be a dome (if not, you will be asked to convert it) within
which the sources can be moved according to CUBE behaviours where it's
possible to move the sound inside or outside the dome of speakers. In
HYBRID mode, the spans keep their usual dome or cube behaviour.

### 5.7.1. What is saved in HYBRID mode?

There are two types of information that are saved with the project in
HYBRID mode:

• The HYBRID mode itself is saved exclusively with the project.

• The selection of the DOME or the CUBE algorithm for each source is
also saved with the project.

### 5.72. What Mode is loaded according to the opening order of Speaker Setup and Project?

As a rule, it is always the last opened document — Speaker Setup or
Project — that determines the algorithm used by *SpatGRIS*.

A Speaker Setup (SS) followed by a Project (P):

1.1. SS Dome + P Dome = Dome.

2.1. SS Cube + P Cube = Cube.

3.1. SS Dome + P Cube = Cube. The SS Dome has been converted to SS Cube.
The shape of the SS does not change, since the Cube algorithm accepts
all domes (this can be confirmed by opening the Speaker Setup Edition
window). Before closing the SS, you'll be asked to save the changes.

4.1. SS Cube + P Dome = Dome. The SS Cube is converted into a Dome after
the conversion message is approved.

5.1. SS Dome + P Hybrid = Hybrid.

6.1. SS Cube + P Hybrid = Hybrid. SS Cube is converted to Dome after the
conversion message is approved.

In reverse order:

1.2. P Dome + SS Dome = Dome.

2.2. P Cube + SS Cube = Cube.

3.2. P Cube + SS Dome = Dome. The Cube project has been converted to SS
Dome.

4.2. P Dome + SS Cube = Cube. The Dome project has been converted to SS
Cube.

5.2. P Hybrid + SS Dome = Hybrid. This is the only exception where
Hybrid has priority, despite the fact it was loaded first. It's because
Hybrid projects works on SS Dome only.

6.2. P Hybrid + SS Cube = Cube. Hybrid disappears from the view since we
have just switched to Cube. This is normal. By selecting Hybrid manually
afterwards, the SS Cube is converted into a Dome after the conversion
message is approved. The saved information of the P Hybrid is then
recovered.

### 5.7.3. Attenuation settings in CUBE or HYBRID mode

In CUBE and HYBRID modes, there are an inner circle and an outer circle
in the middle of the Speaker Setup. Within the inner circle, attenuation
and/or filtering are not applied. Outside the inner circle, attenuation
and/or filtering can be applied to simulate the vanishing of a sound at
a faraway distance. At the outer circle, attenuation and filtering reach
their maximum values. You can indicate these maximum values in the
Attenuation settings menus. In HYBRID mode, Attenuation settings work
only on CUBE sources.

<img src="/media-en/media/image60.png"
style="width:2.70371in;height:3.5in" />

Actually, the inner circle is a sphere within which the attenuation
settings start to be calculated from the «floor», that is to say from
the coordinates (0.0, 0.0):

<img src="/media-en/media/image61.jpg"
style="width:2.7in;height:2.55894in" />

Attenuation settings parameters:

<img src="/media-en/media/image62.jpg"
style="width:3in;height:0.79808in" /><img src="/media-en/media/image63.jpg"
style="width:3in;height:0.8in" />

<img src="/media-en/media/image64.jpg"
style="width:3in;height:1.19167in" /><img src="/media-en/media/image65.jpg"
style="width:3in;height:1.19in" />

• On/Off

• Volume (dB): from 0 to -72, in -12dB steps.

• Filtering (Hz): from 125 to 16000, in octave steps.

• Volume and filtering are independent.

• In Elevation, attenuation starts at the top (Extended Top) and at the
bottom (Extended Top and Bottom) of the cube.

• Attenuation settings also work in STEREO and BINAURAL mode.

NOTE: Attenuation Settings are saved within the Project.

### 5.7.4. Convert from DOME to CUBE and vice versa

In the case of switching from DOME to CUBE, *SpatGRIS* uses XYZ
coordinates of the setup to maintain the integrity of the setup. This
does not apply to the transition from CUBE to DOME, since in the VBAP
algorithm the distance is always adjusted to 1.00. Elevation and
Distance do not have the same behaviour in the DOME and CUBE algorithms.
A speaker setup retains its appearance and XYZ coordinates when
transitioning from the DOME algorithm to the CUBE algorithm, but not the
other way around.

### 5.7.5. Spatialization in 2D and 3D

*SpatGRIS* is capable of 2D and 3D spatialization either in DOME or CUBE
mode. It can be useful to use *SpatGRIS* in 2D with DAWs that are
stereo-only like Ableton Live and Pro Tools native. Doing so gives these
stereo DAWs the possibility to manage multispeaker environment like
cinema standards. But of course, the real power of *SpatGRIS* lies in
its 3D capabilities.

The following images present an example of a 2D speaker setup — an
octophony—, and a 3D speaker setup — a cube of 24 (3x8) speakers.

<img src="/media-en/media/image66.jpg"
style="width:2.73896in;height:2.3622in" /><img src="/media-en/media/image67.jpg"
style="width:2.59476in;height:2.3622in" />

## 5.8. Speaker Setup

To design a speaker setup is the first step of the process. It is done
in the *Speaker Setup Edition* window (View menu, Opt-W).

A Templates menu is provided with different speaker setups in DOME or
CUBE format. The speaker setups in the Templates can’t be modified. You
can use them, edit them, and save them under the name of your choice by
using Save Speaker Setup As from the File menu.

<img src="/media-en/media/image68.jpg"
style="width:2.06464in;height:1.5in" />

### 5.8.1. Speaker Setup Edition

<img src="/media-en/media/image69.png"
style="width:6.2in;height:3.73565in" />

Since the introduction of the MBAP (version 3.20 and up) in CUBE mode,
the Global Sound Diffusion parameter allows changing the diffusion of
the sound globally for the whole set of speakers. Precise localization
is obtained with a small value, higher values will result with a blurred
spatial image. This parameter can also influence the smoothness of
trajectories.

Except for Distance which is set to 1.00 in DOME mode (by definition),
speaker setup parameters can be set by polar values in DOME (Azimuth,
Elevation) or by Cartesian values in CUBE (X, Y, Z). In DOME mode,
Cartesian values are greyed out. In CUBE mode, polar values are greyed
out.

### 5.8.2. Speakers’ order and image representation

By clicking at the top of each column (except for Gain and Highpass) in
the Speaker Setup Edition window, the order of the speakers can be
organized). The most important one is the Output column where you can
move manually or automatically each speaker. This order will be
reflected in the Speakers VU-meter ordering.

Consecutive order:

<img src="/media-en/media/image70.jpg"
style="width:4.72441in;height:1.41732in" />

Odd and even order followed by direct outputs:

<img src="/media-en/media/image71.jpg"
style="width:4.72441in;height:1.35373in" />

Here is an example of a speaker order that represents the actual
position of the speakers in a studio with respect to the Y-axis (See
5.9.1 for more information). One can see on the speaker VU-meter section
how the energy is distributed from the left to the right in the dome.
The speakers 11 and 20 are in the centre, and the subs on the extreme
left and right like they are placed in the studio. All the other
speakers are equally distributed along the Y-axis:

<img src="/media-en/media/image72.jpg"
style="width:6.25in;height:2.02457in" />

### 5.8.3. Minimal requirements

The DOME in particular needs minimal requirements to perform the VBAP
calculations. If the speaker setup doesn’t fulfill them, you’ll be
warned by one or two of these messages:

<img src="/media-en/media/image73.jpg"
style="width:3in;height:1in" /><img src="/media-en/media/image74.jpg"
style="width:3in;height:1in" />

### 5.8.4. Direct outputs

<img src="/media-en/media/image75.jpg"
style="width:0.38819in;height:1.96806in" />A sound Source can be sent
directly to a speaker via a direct output. There are two types of direct
outputs in *SpatGRIS*, which was not the case before.

#### Independent direct outputs

There are independent direct outputs intended for special uses like the
subwoofers. These speakers are identified with an orange rectangle in
the Speaker Setup Edition window.

<img src="/media-en/media/image76.jpg"
style="width:5.9in;height:0.53327in" />

Their placement in the setup is not that critical, since they are
independent of the spatialization, but if you intend to downmix your
project in a two-channel format, their sound will be placed in the
stereo image according to their left-right position. They are
represented in black in the 3D SpeakerView.

<img src="/media-en/media/image77.jpg"
style="width:6.18056in;height:1.38889in" />

#### Spatialized direct outputs

This is a new feature in *SpatGRIS*. Any speaker in the setup can be
used as a direct output and continue to be used by the spatialization
algorithms. Every source has a direct output text box that is empty by
default. Any speaker number can be put in there. The difference between
the types of direct outputs is that independent outputs are used only
for that purpose. There is no distinction in the speaker 3D view for the
spatialized direct outputs.

Spatialized direct outputs were created by Samuel Béland, a major
improvement of *SpatGRIS*.

One can see the distinction when selecting a direct output. The first
numbers, at the top of the column (17-18) are independent direct
outputs. The other numbers (1-16) can be used as a spatialized direct
output.

In the following example, source 5 is sent directly to speaker 9 and
source 8 to speaker 14. Both speakers 9 and 14 remains in the DOME
configuration. Finally, we have sources 15-16 sent to independent direct
outputs 17-18:

<img src="/media-en/media/image78.png"
style="width:4.56693in;height:5.70866in" />

NOTE: Since direct outputs are assigned to specific outputs, if you open
a project with different numbers of direct outputs than those in the
actual speaker setup, some outputs may be muted! There is no warning for
that!

### 5.8.5. Show Speaker Numbers

The location of the speakers and their numbers can be viewed in the 3D
window by choosing the Show Speaker Numbers option (Opt-Z[13]). Direct
outputs are shown in black. Clicking on a speaker or its number selects
it; right-clicking deselects it. In the above image, speaker 3 is
selected and independent direct outputs 17-18 are in black. Show Speaker
Numbers only works if Show Speakers is active in the View menu.

## 5.9. Sources and Speakers

*SpatGRIS* receives audio signals from the DAW and sends them to the
speakers. The two main sections are the *Sources* (from the DAW through
*BlackHole*) and the *Speakers.* There are also the direct outs that are
sent directly from the sources to these speakers (for subwoofers for
instance).

<img src="/media-en/media/image79.png"
style="width:5.25in;height:4.86111in" />

In this example, the sources are made of 4 X octophonic sources (1-32),
plus 1 X stereo source (33-34), 1 X stereo spatialized direct outputs
(35-36 sent to 53-54) and 1 X independent direct output (37-38, assigned
to 5-6) for a total of 38 sources identified by different groups of
colours, distributed on a 32-speaker dome with 2 independent direct outs
(5-6).

### 5.9.1. Mute and Solo

Each source and speaker have a *Mute* and a *Solo* button.

<img src="/media-en/media/image80.png"
style="width:3.40909in;height:3in" />

### 5.9.2. Peak indicators and Reset

A peak indicator is present for Sources and Speakers. There is a general
Reset Meter Clipping in the view menu (Opt-M).

## 5.10. STEREO reduction

### 5.10.1. STEREO

There is a STEREO mode to listen to a complex project on a pair of
speakers. All the sounds are sent to the corresponding speakers
depending on their location (left to left, right to right, no front-back
axis, no elevation). When STEREO is selected, the stereo routing option
appears to allow you to choose the outputs of your choice, depending on
your sound card. Only your sound card outputs are available for the
stereo reduction. When using the computer internal sound card, the
outputs are allocated to numbers 1 and 2. 

<img src="/media-en/media/image81.jpg"
style="width:2.38559in;height:0.8in" />

This mode can be used to downsize a multichannel project to stereo. The
sources are simply placed on the Y-axis from left to right. Only the
azimuth span is used in STEREO mode, not the Elevation span. Keep in
mind that the sources, except for the direct outputs, are never placed
directly on a speaker, but on many speakers — at least three on a DOME,
many more on a CUBE. So, the projection of the sources is probably not
accurate as it shows on this representation!

<img src="/media-en/media/image82.png"
style="width:5in;height:3.17343in" />

### 5.10.2. BINAURAL

This algorithm was implemented to help users to work on 3D
spatialization from home when access to a speaker dome is limited or
unavailable. It is based on a Head Related Transfer Function (HRTF).
HRTF is a function that reproduces the way we perceive the localization
of sounds in the space. It is a set of phase and amplitude calculations
for listening on headphones. Primarily, it is designed for 5.1
reproductions or immersive listening on headphones, situations found in
the gaming and the Virtual Reality industries. To minimize the number of
calculations (HRTF can be very demanding in terms of computing power),
*SpatGRIS* first calculates a VBAP spatialization over 16 speakers (with
the BINAURAL_SPEAKER_SETUP, made invisible in this version) and then
transfers the result to HRTF. Don't worry, even if your speaker setup
contains more than 16 speakers, no information is lost in the process.
BINAURAL modes use the stereo outputs of your choice. Both Spans are
available in BINAURAL mode.

For various reasons and due to technical considerations, the output
loudness of STEREO mode differs considerably from BINAURAL, mode
depending on the number of sources. Please adjust your listening level
accordingly.

NOTE: The Attenuation Settings used in Cube or Hybrid mode, are
functional in stereo reduction.

## 5.11. Recording

When the composition of the spatialization is completed, you have two
options:

1\. To play the piece "live" with your DAW and *SpatGRIS*.

2\. To record the spatialization to as many audio channels as the number
of the speakers in the setup.

*SpatGRIS* records mono files (AIFF or WAV according to your
preferences) or one interleaved file.

To record: press the big red button on the bottom right of the main
window.

<img src="/media-en/media/image83.jpg"
style="width:0.79167in;height:0.79167in" />

A pop-up window will then open, allowing you to specify:

• The location of the recorded files.

• Their name.

• The format: WAV or AIFF.

• The number of files: Mono Files or Interleaved.

• The possibility to export the Speaker Setup for the Player function
(chapter 6).

Pressing the Record button will start the recording and the timer, and
it will change the Record button to a blinking one. When it’s completed,
you can press the Record button again to stop the recording. You can
then import the separate mono files (or an interleaved file) into any
DAW to play your piece in concert.

<img src="/media-en/media/image84.jpg"
style="width:4.5in;height:1.20288in" />

Keep in mind that with interleaved files, there are some limitations,
and these limitations are reached quite rapidly on big projects:

• AIFF is limited to 2 GB.

• WAV is limited to 4 GB[14].

Also, if you record a file with many channels, you’ll find very few DAWs
capable of opening it. So, it’s preferable to record Mono files.

# 6. PLAYER

*SpatGRIS*, starting with version 3.2, introduces a new tool, the
PLAYER, which allows to use *SpatGRIS* as standalone software to play
any piece recorded by *SpatGRIS* with any speaker setup. The main idea
of the PLAYER is to help the diffusion of multichannel works among
different users and on different speaker setups. Works made in DOME
setup can be played in CUBE setup and vice versa. Direct outputs will be
assigned automatically but can be manually adjusted afterwards.

## 6.1. To make a recording for the PLAYER

The procedure for the recording of a piece for playback with the PLAYER
is almost identical to that of a normal recording. The main difference
is that, in addition to recording the audio files themselves, you must
export the coordinates of the used speaker setup by toggling the Export
Speaker Setup function. The audio files and the speaker setup will be
placed in the same folder and must remain there for the PLAYER to work
properly. These coordinates will be used by the PLAYER to correctly
position the sources in any given listening setup.

<img src="/media-en/media/image85.jpg"
style="width:4.5in;height:1.17019in" />

NOTE: Only mono files work with the PLAYER. You'll get an error message
if you try to open an interleaved file. The reason for this is that the
PLAYER uses the output numbers in the name of the audio files for the
spatialization. There is no way to encode this information in an
interleaved sound file.

<img src="/media-en/media/image86.jpg"
style="width:1.47736in;height:1.5in" />

## 6.2. To open and to play a project with the PLAYER

Once the recording is done, you can send the folder that includes the
sound files and the speaker setup to a listener who would use a
different setup. Or you can use it yourself to play the recording on a
different setup.

### 6.2.1. Open the listening speaker setup

Open the speaker setup in *SpatGRIS* on which you intend to listen to
the spatialized work. It could be a custom setup or a setup from the
templates.

### 6.2.2. Open the PLAYER window and load the files

View Menu —\> Show Player View

Load the audio files and Speaker Setup folder:

<img src="/media-en/media/image87.jpg"
style="width:5.5in;height:2.92804in" />

The PLAYER is now showing the basic waveform of the audio files:

<img src="/media-en/media/image88.jpg"
style="width:5.5in;height:2.92804in" />

The PLAYER will also show the speaker setup with which the work was
recorded. The original speaker locations are shown in red:

<img src="/media-en/media/image89.jpg"
style="width:4.71429in;height:3in" />

Please note that the current project loaded in *SpatGRIS* is being
replaced by the project of the recording.

### 6.2.3. To play the piece

The PLAYER is now ready to play the piece. Just use the Play and Stop
buttons. It's also possible to click anywhere in the soundfile to start
the playback from there.

### 6.2.4. DOME in CUBE or CUBE in DOME

Here's an example of a recording made with a dome setup
(Dome20(8-6-4-2)Subs4) and played within a cube setup
(Cube24(2X12)Subs2). As one can see the shape of the original dome is
well reproduced in the listening cube:

<img src="/media-en/media/image90.jpg"
style="width:5.5in;height:3in" />

Here is another example showing the opposite situation, a cube recording
(Cube24(3X8)Subs2) played within a dome (Dome20(8-6-4-2)Subs4). As one
can see the shape of the original cube is well reproduced in the
listening dome:

<img src="/media-en/media/image91.jpg"
style="width:5.5in;height:3in" />

### 6.2.5. Regarding the direct outs in the PLAYER

The PLAYER will try to assign direct outputs to the currently loaded
speaker setup direct outputs.

In the first previous example, the original setup had four direct
outputs (numbers **6-12-18** and **24**). But in the listening setup,
there are only two direct outputs (**25** and **26**). The PLAYER
assigned alternatively the direct output numbers from the original to
the available direct outs of the listening setup. These output numbers
can be manually adjusted afterwards:

<img src="/media-en/media/image92.jpg"
style="width:5.5in;height:2.87869in" />

## 6.3. To save a PLAYER project

If you have changed any element in the PLAYER project, it could be saved
by using the Save Player Project button. This document will be placed
automatically in the same folder as the audio files and the speaker
setup. The File Saved! button will blink for a while during the process.
All the files should remain in the same folder. The next time you use
the Load audio files and Speaker Setup folder button, everything will be
placed correctly according to the way it was saved.

<img src="/media-en/media/image93.jpg"
style="width:5.5in;height:2.94274in" />

NOTE: A player project remains active until the PLAYER window is open.
When you close it, SpatGRIS switches to its normal input mode, waiting
for audio and OSC to come from either a sequencer or any other software.

# 7. Menus

## 7.1. File menu

In the File menu you will find all the project-related functions, where
you can:

<img src="/media-en/media/image94.jpg"
style="width:1.6in;height:1.57569in" />

<img src="/media-en/media/image95.png"
style="width:1.6in;height:1.35903in" />• Create a New Project.

• Open an existing one.

• Open a project from the Project Templates folder. These templates
can’t be modified but they can be edited and saved as a new file.

• Save Project or Save As — make a copy.

• Open a speaker setup.

• Open a speaker setup from the Speaker SetupTemplates folder. These
templates can’t be modified but they can be edited and saved as a new
file.

• Save Speaker Setup or Save As — make a copy.

• Open the Settings window.

## 7.2. View menu

Under the View menu, you can choose from different perspectives to
visualize the speakers and sources in real time. The key modifier in
this menu is Option (Opt) for Mac and Alt for Windows.

<img src="/media-en/media/image96.png"
style="width:1.8in;height:2.0625in" /><img src="/media-en/media/image49.jpg"
style="width:1.8in;height:2.68741in" />• Show 2D view: A 2D view from
the top of the space is given showing only the sources.

• Speaker Setup Edition: Opens a window to access all the given
parameters for a valid configuration of speakers.

•Show Player View: open the Player window

• Show OSC monitor: for specialists! To help troubleshoot incoming OSC
message streams.

• Show SpeakerView: open the 3D view of the speakers

—

Keep SpeakerView On Top

—

• Show Hall: show the walls of the hall

• Show Numbers: Show or hide the numbers of the displayed sources and/or
speakers.

• Show Speakers: Show or hide the speakers in the 3D view.

• Show Speakers Triplets: Show or hide the triplets in the 3D view in
DOME mode. There are no triplets in CUBE mode.

• Show Source Activity: This option allows to see the position and
trajectories of the sources (large points) and their values for Azimuth
and Elevation Span (small points), according to the data sent by the
*ControlGRIS* plugin. Note that there is nothing to see when the DAW is
stopped. The threshold is set at -70 dB. When this option is not
selected, all sources that are part of a project are displayed, even
when the DAW is stopped. This option can be useful for checking that
there are no duplicate OSC channels sent from *ControlGRIS* to
*SpatGRIS*.

<img src="/media-en/media/image97.jpg"
style="width:2.12321in;height:1.9685in" /><img src="/media-en/media/image98.jpg"
style="width:2.12321in;height:1.9685in" />

<table>
<colgroup>
<col style="width: 46%" />
<col style="width: 53%" />
</colgroup>
<thead>
<tr class="header">
<th><em>Show Source Activity</em> Off: shows the position of all the
sources</th>
<th><em>Show Source Activity</em> On: shows only the real activity of
the sources in play mode</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

• Show Speaker Level: Shows how much energy each speaker delivers. From
grey (nothing) to white (maximum).

• Show Sphere/Cube: If you have the chance to play in a full sphere or
cube!

—

• Colorize Sources: This option allows you to set all the inputs to a
different colour within the visible spectra from red to purple. Be
careful, it erases all the custom colours already in place.

• Reset Sources Position: When switching from a project to another,
*SpatGRIS* could still show the sources from the previous project. Use
this option to clear up the 3D view.

• Reset Meter Clipping: clipping indicators can be reset individually by
clicking on them, or globally with Opt-M shortcut.

## 7.3. Naming and Saving

There are three sections in *SpatGRIS* that are saved independently:
Project, Speaker Setup and Settings.

• Save Project. A project is coupled with a work.

• Save Speaker Setup. A speaker setup is coupled to an installation
placed in a space.

• Save Settings. User settings are linked to a workstation — computer
and audio interface — including the stereo outputs used for stereo
reduction (even without showing it)

• Save Settings. The stereo outputs are coupled to a specific audio
interface.

Speaker setups and Project documents are saved under the .xml format.
There is no distinction between them. The Project document doesn't
include the speaker setup and they are therefore independent.
Consequently, we strongly recommend two things:

• Add the word "Speaker Dome" or " Speaker Cube" to the name of your
speaker setups and "Project Dome", "Project Cube" or "Project Hybrid" to
the name of your project files.

• Save the DOME or the CUBE speaker setups in two separate folders in a
folder named *Speaker*s.

• Save *SpatGRIS* projects in three separate folders inside a folder
named *Projects.*

The Templates menus we provide with *SpatGRIS* is a good example of the
right classification.

• Document format warnings

*SpatGRIS* always remembers the last opened speaker setup and the last
project.

If you try to open a *SpatGRIS* project with the command Load Speaker
Setup (or the opposite), you'll be warned:

<img src="/media-en/media/image99.jpg"
style="width:2.75265in;height:1.10236in" /><img src="/media-en/media/image100.jpg"
style="width:2.75in;height:1.10236in" />

NOTE: SpatGRIS documents adopt a new format and are not backward
compatible with older versions of SpatGRIS. By trying to open a SpatGRIS
project or a speaker setup from the version 2, you’ll get one of these
scary messages! Your files are OK, just not compatible:

<img src="/media-en/media/image101.jpg"
style="width:2.75in;height:1.1in" /><img src="/media-en/media/image102.jpg"
style="width:2.75in;height:1.1in" />

## 7.4. Representations

The 3D and 2D views in *SpatGRIS* are available for both DOME and CUBE
modes. The sources on the DOME are on the surface and the Spans spread
along that surface. In CUBE mode, the sources can be placed anywhere in
the space and the Spans spread locally around the sources.

### 7.4.1. 3D Representation

The 3D window in DOME mode (left) or in CUBE mode (right) of the same
session. Speakers and Sources are represented:

<img src="/media-en/media/image103.jpg"
style="width:2.75in;height:2.2999in" /><img src="/media-en/media/image104.jpg"
style="width:2.75in;height:2.30283in" />

### 7.4.2. 2D Representation

The 2D view in DOME mode (left) or in CUBE mode (right) of the same
session. Only Sources are represented:

<img src="/media-en/media/image105.jpg"
style="width:2.3in;height:2.39632in" /><img src="/media-en/media/image106.jpg"
style="width:2.3in;height:2.39608in" />

## 7.5. Performance and CPU burst

The performance of the *ControlGRIS*/*SpatGRIS* combination largely
depends on the different settings in your project. As a rule, a project
with 64 audio channels sent to 64 speakers will work perfectly well on
recent computers. We have tested projects with more than 100 audio
channels over a 256-speaker setup and that was still working well!

The factors which will significantly augment the CPU usage needed by our
tools are, in order of importance:

• The Mode: CUBE is more demanding than DOME, since the former uses more
speakers than the latter.

• The Spans: they distribute the signal to more speakers than when they
are not in use, and therefore the CPU demand increases very rapidly as
their values increase.

• The Interpolation: the interpolation factor helps some sounds to
achieve a more fluid transition time as they move from one place to the
next. Therefore, the higher this parameter, the higher the number of
speakers involved in the process, since a sound will reach a given
speaker earlier and take more time to leave it (not to mention, it also
blurs the localization).

• The number of speakers used in *SpatGRIS*. We measured comfortable
performance with a 96-speaker setup, which is largely enough in most
realistic situations!

• The number of tracks multiplied by the number of speakers determines
the reliability of the setup. Few tracks over a big speaker setup will
give the same result as many tracks over a small speaker setup.

If the CPU overpass 100%, this is the warning you'll get this alert:

<img src="/media-en/media/image107.jpg"
style="width:1.60048in;height:0.3937in" />

Want to know what to expect? Try it for yourself!

## 7.6. Help Menu

The Help menu comprises information about the GRIS and this manual,
under the Open Documentation option.

<img src="/media-en/media/image12.jpg"
style="width:1.81222in;height:0.7in" />

**Take the plunge and have fun!**

# 8. Addendum

## 8.1. Sources Link descriptions

### 8.1.1. Azimuth-Elevation and Azimuth-Distance

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>1) Independent</strong> MONO + STEREO + MULTIPHONIC</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><img src="/media-en/media/image108.jpeg"
style="width:1.33333in;height:1in" />This mode is selected by default.
The sources can be moved independently from one another.<img
src="/media-en/media/image109.jpeg"
style="width:1in;height:1in" /></td>
</tr>
<tr class="even">
<td><strong>2) Circular</strong> STEREO + MULTIPHONIC</td>
</tr>
<tr class="odd">
<td><p><img src="/media-en/media/image110.jpeg"
style="width:0.95288in;height:1in" />This mode enables the circular
grouped movement. The angles between the sources remain constant while
the radius adjusts proportionally.</p>
<p><img src="/media-en/media/image111.jpeg"
style="width:0.99788in;height:1in" /></p></td>
</tr>
<tr class="even">
<td><strong>3) Circular Fixed Radius</strong> STEREO + MULTIPHONIC</td>
</tr>
<tr class="odd">
<td><img src="/media-en/media/image112.jpeg"
style="width:1.04655in;height:1in" />The sources are linked in a
circular motion by the Radius parameter, which remains fixed and equal.
The relative distance between each source and the centre is the same for
all sources.<img src="/media-en/media/image113.jpeg"
style="width:0.99788in;height:1in" /></td>
</tr>
<tr class="even">
<td><strong>4) Circular Fixed Angle</strong> STEREO + MULTIPHONIC</td>
</tr>
<tr class="odd">
<td><p><img src="/media-en/media/image114.jpeg"
style="width:0.83333in;height:1in" />The sources are linked in a
circular motion with the Angle parameter, which remains fixed and
equal.</p>
<p>For example, in octophony the opening angle between each of the
sources will be fixed to 45°.<img
src="/media-en/media/image115.jpeg"
style="width:1in;height:1in" /></p></td>
</tr>
<tr class="even">
<td><strong>5) Circular Fully Fixed</strong> STEREO + MULTIPHONIC</td>
</tr>
<tr class="odd">
<td><img src="/media-en/media/image116.jpeg"
style="width:1.00167in;height:1in" />The sources are linked in a
circular motion by both the Radius and Angle parameters, which remain
fixed and equal. The opening between the sources and their radius is
therefore always identical.<img
src="/media-en/media/image117.jpeg"
style="width:1in;height:1in" /></td>
</tr>
<tr class="even">
<td><strong>6) Delta Lock</strong> STEREO + MULTIPHONIE</td>
</tr>
<tr class="odd">
<td><img src="/media-en/media/image118.jpeg"
style="width:1.21704in;height:1in" />This mode locks the position of the
sources in relation to others along the X and Y axes, without the
possibility of rotation.<img src="/media-en/media/image119.jpeg"
style="width:1in;height:1in" /></td>
</tr>
</tbody>
</table>

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>7) Symmetric X</strong> STEREO</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><img src="/media-en/media/image120.jpeg"
style="width:1.33333in;height:1in" />This mode enables the symmetry
between two sources following the X axis.<img
src="/media-en/media/image121.jpeg"
style="width:1in;height:1in" /></td>
</tr>
<tr class="even">
<td><strong>8) Symmetric Y</strong> STEREO</td>
</tr>
<tr class="odd">
<td><img src="/media-en/media/image122.jpeg"
style="width:1.33333in;height:1in" />This mode enables the symmetry
between two sources following the Y axis.<img
src="/media-en/media/image123.jpeg"
style="width:1in;height:1in" /></td>
</tr>
</tbody>
</table>

### 8.1.2. Elevation (CUBE mode only)

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>1) Independent</strong> MONO + STEREO + MULTIPHONIC</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><img src="/media-en/media/image124.jpg"
style="width:0.94654in;height:1in" /> This mode is selected by default.
The sources can be moved independently from one another.</td>
</tr>
<tr class="even">
<td><strong>2) Fixed Elevation</strong> STEREO + MULTIPHONIC</td>
</tr>
<tr class="odd">
<td><img src="/media-en/media/image125.jpg"
style="width:0.9375in;height:1in" />Same elevation for each source.</td>
</tr>
<tr class="even">
<td><strong>3) Bottom Top</strong> STEREO + MULTIPHONIC</td>
</tr>
<tr class="odd">
<td><img src="/media-en/media/image126.jpeg"
style="width:0.94643in;height:1in" />This mode locks the position of the
sources from a minimum to a maximum value in a linear relationship.</td>
</tr>
<tr class="even">
<td><strong>4) Top Bottom</strong> STEREO + MULTIPHONIC</td>
</tr>
<tr class="odd">
<td><img src="/media-en/media/image127.jpg"
style="width:0.94028in;height:1in" />This mode locks the position of the
sources from a maximum to a minimum value in a linear relationship.</td>
</tr>
</tbody>
</table>

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>5) Delta Lock</strong> STEREO + MULTIPHONIC</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><img src="/media-en/media/image128.jpg"
style="width:0.94654in;height:1in" />This mode locks the position of the
sources in relation to others.</td>
</tr>
</tbody>
</table>

## 8.2. Trajectory descriptions

### 8.2.1. Azimuth-Elevation and Azimuth-Distance

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>1) Circle</strong></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><img src="/media-en/media/image129.jpg"
style="width:0.94097in;height:1in" />Circular motion around the
centre.</p>
<p>Options: CW/CCW, Back &amp; Forth, Dampening, Deviation.</p></td>
</tr>
<tr class="even">
<td><strong>2) Ellipse</strong></td>
</tr>
<tr class="odd">
<td><p><img src="/media-en/media/image130.jpg"
style="width:0.94081in;height:1in" />Elliptical motion around the
centre.</p>
<p>Options: CW/CCW, Back &amp; Forth, Dampening, Deviation.</p></td>
</tr>
<tr class="even">
<td><strong>3) Spiral</strong></td>
</tr>
<tr class="odd">
<td><p><img src="/media-en/media/image131.jpg"
style="width:0.94048in;height:1in" />Concentric motion around the
centre.</p>
<p>Options: CW/CCW, Back &amp; Forth, Dampening, Deviation.</p></td>
</tr>
<tr class="even">
<td><strong>4) Square</strong></td>
</tr>
<tr class="odd">
<td><p><img src="/media-en/media/image132.jpg"
style="width:0.94395in;height:1in" />Square shape around the centre.</p>
<p>Options: CW/CCW, Back &amp; Forth, Dampening, Deviation.</p></td>
</tr>
<tr class="even">
<td><strong>5) Triangle</strong></td>
</tr>
<tr class="odd">
<td><p><img src="/media-en/media/image133.jpg"
style="width:0.94097in;height:1in" />Triangle shape around the
centre.</p>
<p>Options: CW/CCW, Back &amp; Forth, Dampening, Deviation.</p></td>
</tr>
</tbody>
</table>

### 8.2.2. Elevation (CUBE mode only)

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>1) Down Up</strong></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><img src="/media-en/media/image134.jpeg"
style="width:0.93146in;height:1in" />From the bottom to the top.</p>
<p>Options: Back &amp; Forth, Dampening.</p></td>
</tr>
<tr class="even">
<td><strong>2) Up Down</strong></td>
</tr>
<tr class="odd">
<td><p><img src="/media-en/media/image135.jpeg"
style="width:0.94063in;height:1in" /> From the top to the bottom.</p>
<p>Options: Back &amp; Forth, Dampening</p></td>
</tr>
</tbody>
</table>

## 8.3. OSC messages in SpatGRIS

OSC can be sent directly to *SpatGRIS* without having to use
*ControlGRIS*.

OSC Input port number: 18032 by default (can be changed in File -\>
Settings)

The server address is always /spat/serv.

**Please note that angles are always measured clockwise, starting from
the upstage centre (the positive Y direction).**

**pol** moves a source using polar coordinates in radians.

<table>
<colgroup>
<col style="width: 18%" />
<col style="width: 13%" />
<col style="width: 28%" />
<col style="width: 39%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>#parameter</strong></th>
<th><strong>type</strong></th>
<th><strong>allowed values</strong></th>
<th><strong>meaning</strong></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>1</td>
<td>string</td>
<td>pol</td>
<td>-</td>
</tr>
<tr class="even">
<td>2</td>
<td>int</td>
<td>[1, 256]</td>
<td>Source index</td>
</tr>
<tr class="odd">
<td>3</td>
<td>float</td>
<td>any</td>
<td>azimuth angle</td>
</tr>
<tr class="even">
<td>4</td>
<td>float</td>
<td>any</td>
<td>elevation angle</td>
</tr>
<tr class="odd">
<td>5</td>
<td>float</td>
<td>[-3.0, 3.0]</td>
<td>radius</td>
</tr>
<tr class="even">
<td>6</td>
<td>float</td>
<td>[0, 1]</td>
<td>Horizontal span</td>
</tr>
<tr class="odd">
<td>7</td>
<td>float</td>
<td>[0, 1]</td>
<td>Vertical span</td>
</tr>
</tbody>
</table>

ex : The message /spat/serv pol 7 0.0 0.78 0.5 0.1 0.2 moves the source
\#7 in the front at half elevation and placed at half the distance from
the origin, with an horizontal span of 10% and a vertical span of 20%.

**  
**

**deg** moves a source using polar coordinates in degrees.

<table>
<colgroup>
<col style="width: 20%" />
<col style="width: 15%" />
<col style="width: 26%" />
<col style="width: 38%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>index</strong></th>
<th><strong>type</strong></th>
<th><strong>allowed values</strong></th>
<th><strong>meaning</strong></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>1</td>
<td>string</td>
<td>deg</td>
<td>-</td>
</tr>
<tr class="even">
<td>2</td>
<td>int</td>
<td>[1, 256]</td>
<td>Source index</td>
</tr>
<tr class="odd">
<td>3</td>
<td>float</td>
<td>any</td>
<td>azimuth angle</td>
</tr>
<tr class="even">
<td>4</td>
<td>float</td>
<td>any</td>
<td>elevation angle</td>
</tr>
<tr class="odd">
<td>5</td>
<td>float</td>
<td>[-3.0, 3.0]</td>
<td>radius</td>
</tr>
<tr class="even">
<td>6</td>
<td>float</td>
<td>[0, 1]</td>
<td>Horizontal span</td>
</tr>
<tr class="odd">
<td>7</td>
<td>float</td>
<td>[0, 1]</td>
<td>Vertical span</td>
</tr>
</tbody>
</table>

ex : The message /spat/serv deg 7 -90.0 45.0 0.5 0.1 0.2 moves the
source \#7 at the extreme left, at half elevation and half the distance
of the space, with an horizontal span of 10% and a vertical span of 20%.

**car** moves a source using Cartesian coordinates.

<table>
<colgroup>
<col style="width: 19%" />
<col style="width: 18%" />
<col style="width: 22%" />
<col style="width: 38%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>index</strong></th>
<th><strong>type</strong></th>
<th><strong>allowed values</strong></th>
<th><strong>meaning</strong></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>1</td>
<td>string</td>
<td>car</td>
<td>-</td>
</tr>
<tr class="even">
<td>2</td>
<td>int</td>
<td>[1, 256]</td>
<td>Source index</td>
</tr>
<tr class="odd">
<td>3</td>
<td>float</td>
<td>[-1.66, 1.66]</td>
<td>x (left/right)</td>
</tr>
<tr class="even">
<td>4</td>
<td>float</td>
<td>[-1.66, 1.66]</td>
<td>y (back/front)</td>
</tr>
<tr class="odd">
<td>5</td>
<td>float</td>
<td>[-1.66, 1.66]</td>
<td>z (down/up)</td>
</tr>
<tr class="even">
<td>6</td>
<td>float</td>
<td>[0, 1]</td>
<td>Horizontal span</td>
</tr>
<tr class="odd">
<td>7</td>
<td>float</td>
<td>[0, 1]</td>
<td>Vertical span</td>
</tr>
</tbody>
</table>

ex : The message /spat/serv car 7 1.0 1.0 1.0 0.0 0.0 moves the source
\#7 at the top right corner, with no horizontal or vertical spans.

**clr** clears a source's position.

<table>
<colgroup>
<col style="width: 22%" />
<col style="width: 17%" />
<col style="width: 20%" />
<col style="width: 39%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>index</strong></th>
<th><strong>type</strong></th>
<th><strong>allowed values</strong></th>
<th><strong>meaning</strong></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>1</td>
<td>string</td>
<td>clr</td>
<td>clear</td>
</tr>
<tr class="even">
<td>2</td>
<td>int</td>
<td>[1, 256]</td>
<td>Source index</td>
</tr>
</tbody>
</table>

ex : The message /spat/serv clr 7 clears the seventh source's position.

**alg** sets a source's hybrid spatialization mode.

<table>
<colgroup>
<col style="width: 25%" />
<col style="width: 15%" />
<col style="width: 20%" />
<col style="width: 38%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>index</strong></th>
<th><strong>type</strong></th>
<th><strong>allowed values</strong></th>
<th><strong>meaning</strong></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>1</td>
<td>string</td>
<td>alg</td>
<td>-</td>
</tr>
<tr class="even">
<td>2</td>
<td>int</td>
<td>[1, 256]</td>
<td>Source index</td>
</tr>
<tr class="odd">
<td>3</td>
<td>string</td>
<td>dome or cube</td>
<td>Algorithm</td>
</tr>
</tbody>
</table>

ex : The message /spat/serv alg 7 cube sets the seventh source's
spatialization algorithm to "cube" (only works in *hybrid* mode).

## 8.4. OSC messages in ControlGRIS

There are the OSC messages that *ControlGRIS* can send and receive. The
first number corresponds to the plugin ID. The second number corresponds
to the source number. These are the default values:

• /controlgris/1/traj/1/x value =\> \[0.0;1.0\]

• /controlgris/1/traj/1/y value =\> \[0.0;1.0\]

• /controlgris/1/traj/1/z value =\> \[0.0;1.0\]

• /controlgris/1/traj/1/xyz/1 value =\> \[0.0;1.0\] 

• /controlgris/1/traj/1/xyz/2 value =\> \[0.0;1.0\]

• /controlgris/1/traj/1/xyz/3 value =\> \[0.0;1.0\]

• /controlgris/1/traj/1/xy values =\> \[0.0;1.0\] \[0.0;1.0\]

• /controlgris/1/traj/1/xyz values =\> \[0.0;1.0\] \[0.0;1.0\]
\[0.0;1.0\]

• /controlgris/1/azispan value =\> \[0.0;1.0\]

• /controlgris/1/elespan value =\> \[0.0;1.0\]

• /controlgris/1/sourcelink value =\> 1 to 8

1: Independent

2: Circular

3: Circular Fixed Radius

4: Circular Fixed angle

5: Circular Fully Fixed

6: Delta Lock

7: Symmetrix X

8: Symmetric Y

• /controlgris/1/sourcelinkalt value =\> 1 to 5

1: Independent

2: Equal Elevation

3: Bottom-Top

4: Top-Bottom

5: Delta Lock

• /controlgris/1/presets value =\> 1 to 50

• /controlgris/1/elevationmode value =\> 1 to 3

1: Normal

2: Extended Top

3: Extended Top and Bottom

## 8.5. Open Stage Control and Lemur

Two external controllers are available for *ControlGRIS*:

• An Open Stage Control patch for iPad™.

• A Lemur patch for iPad™.

An Addendum manual concerning these patches is available on SourceForge.

## 8.6. Uninstall

### 8.6.1. SpatGRIS

If you need to uninstall *SpatGRIS*, or if you find some strange
behaviour of the software, you'll have to do so manually.

• Put the application itself in the trash.

• Put these files to the trash:

~/Library/Preferences/ca.umontreal.musique.gris.spatgris.plist

~/Application Support/GRIS/ SpatGRIS.x.x.xml where x.x.x is the version
of *SpatGRIS* (3.2.1 for instance).

### 8.6.2. ControlGRIS

If you need to uninstall *ControlGRIS*.

Here are the paths for Mac users:

• To uninstall the Audio Unit version, delete it from the following
location: ~/Library/Audio/Plug-Ins/Components

• To uninstall the VST version, delete it from the VST folder to the
following location: ~/Library/Audio/Plug-Ins/VST

• To uninstall the VST3 version, delete it from the VST3 folder to the
following location: ~/Library/Audio/Plug-Ins/VST3.

• To uninstall the AAX version, delete it from the following location:
MacIntosh HD/Library/Application Support/Avid/Audio/Plug-Ins/

# 9. Known issues and warnings

There are so many different situations and setups that it would be
impossible for us to cover them all. So far, we haven't found any
situation where the system does not work at all. But we have found
situations where some parameters must be adjusted before the system
works properly. Here are a few of them.

## 9.1. Known issues

### 9.1.1. SpatGRIS, Mac version only.

We have a couple of graphical issues with the Apple Silicon machines.

• Issue \#378 (Github): When using the 'Show Speaker Level' function on
M1 and M2, the speakers are not visible unless an audio signal is sent
to them.

• Issue \#344 (Github): Unable to zoom out in the 3D display after a
maximum zoom in, only with Mac M1.

Both these issues are currently under review and should be resolved
soon.

### 9.1.2. ControlGRIS

• The usage of the Back & Forth option leads to many different and
unpredictable behaviours that vary according to the DAW and the kind of
tracks — audio, MIDI, Aux or Instruments — in which *ControlGRIS* is
inserted (Issue \# 94).

• *ControlGRIS* is in an intensive process of refurbishment at the
moment. Stay tuned!

### 9.1.3. SpatGris, the plugin and SpatGRIS, the software

For those who used the plugin *SpatGris1*, you’ll notice that it isn't
working anymore on most recent macOS and on the Apple Silicon machines.
We recommend switching to *ControlGRIS*. The development of *SpatGris*
ended in 2018.

## 9.2. Reaper 

### 9.2.1. Mono tracks

• Create a track and insert an instance of *ControlGRIS* and a mono
audio file into it.

• Click on the Route button located to the right of the track gain
adjustment knob.

• In the window that opens, uncheck Master send.

• At the bottom left of this same window, click on the Add new hardware
output…

• At the very bottom of the list of outputs on the output interface are
the individual, mono outputs.

• Select the output that corresponds to the number assigned to the
source in *ControlGRIS*.

There is no need to pan mono sources to the left for odd tracks and to
the right for even tracks, since you don't have to choose the stereo
outputs of Blackhole. Also, currently the Master track in Reaper is
limited to 128 channels, so it is convenient to use the Reaper hardware
outputs directly as described.

### 9.2.2. Device Preferences with Jack

In the Preferences of Reaper, under Audio tab: uncheck *Close audio
device when stopped and application is inactive*. Otherwise, *Jack* will
lose contact with Reaper when it is inactive, and the system will never
work.

<img src="/media-en/media/image136.jpg"
style="width:3in;height:1.98883in" />

## 9.3. Logic Pro

### 9.3.1. Only one Surround output

In Logic Pro, there is only one possible *Surround* instance. This means
that it is not possible to have multiple multichannel tracks in Logic
Pro while using *SpatGRIS*. To avoid this restriction, use only mono and
stereo tracks in Logic Pro.

### 9.3.2. Activate buttons

When using *ControlGRIS* predefined trajectories, there is an exception
about the activate button in Logic Pro. If there is no more audio in the
track at the stop position, the *Activate* buttons will not turn to off.
They will have to be deactivated manually.

## 9.4. Digital Performer 11 and Automated presets

The recorded presets in DP show soft curves instead of the square
expected ones. It means that changing from one automated preset to the
next is very smooth and progressive, where it’s expected to be drastic.
We are working on that.

## 9.5. Using SpatGRIS with live inputs

When using live inputs, we recommend using the Aggregate Device on a
Mac. According to our tests, the system is stable when you create an
aggregate device comprising *BlackHole* and the sound card you're using.
This aggregate device must be designated as the audio input and output
device in your DAW and as the audio input and output device in
*SpatGRIS*.

For channel numbering, please refer to the Audio / Midi Configuration
application on your Mac once you have created your aggregated device. By
placing your physical sound card as the first device element, you won't
need to change the numbering of speaker configurations. This workflow
has been tested with Ableton Live.

For Windows use, using *Jack* seems sufficient, but we haven't tested it
in depth.

NOTE: Adjust the Buffer size to the same value, both in your DAW and
SpatGRIS. A value of 256 and up is recommended.

# 10. Tips and Tricks

In addition to the normal use of SpatGRIS for programming the
spatialization of sound from a wide variety of sources, here are a few
examples of other uses that might not immediately spring to mind. Over
the years, these uses have emerged through the inventive practices of
our users.

## 10.1. Acousmatic spatialisation

It is perfectly possible to use SpatGRIS in the context of traditional
acousmatic spatialization, where a stereophonic source is multiplied
over as many pairs of loudspeakers in the concert hall. We have used it
in this way for years during the weekly concerts in the History of
Electro Music course.

### 10.1.1. Mixing console

To achieve spatialization in an acousmatic context, you need a mixing
console with Ethernet transmission (ideal, like an AVID S1 or an
Euphonix) or MIDI (slower, like a Mackie Control or a Behringer).

### 10.1.2. Digital Audio Workstation

In the DAW of your choice (DP, Logic, Live, Nuendo, Reaper, etc.), you
place the stereo audio file on the first stereo track, on which you also
place a ControlGRIS plug-in. You then multiply copies of this first
stereo track on as many additional copies as your spatialization
scenario requires. It's also possible to have just one audio track and
as many auxiliary outputs as you need, if your SAN allows. Each track
and each instance of ControlGRIS will be assigned consecutive numbers.
It's important to mention here that we're not talking about one
potentiometer = one loudspeaker. Each loudspeaker can be used for
several **spatialization** scenarios

### 10.1.3. Acousmatic setup

Let's use the Dome24(8-5x2-6)Subs2 Acousmonium setup present in the
SpatGRIS Templates. This consists of:

• 1 octophonic, from 1 to 8

• 1 asymmetric pair on the left 9-10 (direct outputs)

• 1 central solo pair 11-12 (direct outputs)

• 1 main stereo pair 13-14 (direct outputs)

• 1 pair centre-right asymmetric 15-16 (direct outputs)

• 1 asymmetric pair on the left 17-18 (direct outputs)

• 1 hexaphonic group 19 to 24

• 1 pair of subwoofers 25-26 (direct outputs)

<img src="/media-en/media/image137.jpg"
style="width:3.13643in;height:2.8in" />

### 10.1.4. Scenario

The first scenario would involve assigning each potentiometer to a
loudspeaker group in the order mentioned above. This requires 8
potentiometers, as there are 8 loudspeaker groups. Direct outputs do not
need ControlGRIS.

• Potentiometer 1: ControlGRIS 1-2, BlackHole audio outputs 1-2,
Left-Right position, Azimuth Span at 50%.

<img src="/media-en/media/image138.jpg"
style="width:1.63309in;height:2in" />

In this way, the stereo source is fully distributed over the 8 hp of the
octophonic group.

The left channel on the odd-numbered speakers (in pale turquoise) and
the right channel on the even-numbered speakers (in darker turquoise):

<img src="/media-en/media/image139.jpg"
style="width:3.80385in;height:3in" />

• Potentiometer 2: no ControlGRIS, BlackHole outputs 3-4, H-P 9-10
direct outputs in SpatGRIS (in black):

<img src="/media-en/media/image140.jpg"
style="width:0.92099in;height:2in" /><img src="/media-en/media/image141.jpg"
style="width:2.95918in;height:2in" />

• Potentiometer 3: no ControlGRIS, BlackHole outputs 5-6, H-P 11-12
direct outputs in SpatGRIS (in black):

<img src="/media-en/media/image142.jpg"
style="width:0.89686in;height:2in" /><img src="/media-en/media/image143.jpg"
style="width:2.72247in;height:2in" />

• Potentiometer 4: no ControlGRIS, BlackHole outputs 7-8, H-P 13-14
direct outputs in SpatGRIS (in black):

Same scenario

• Potentiometer 5: no ControlGRIS, BlackHole outputs 9-10, H-P 15-16
direct outputs in SpatGRIS (in black):

Same scenario

• Potentiometer 6: no ControlGRIS, BlackHole outputs 11-12, H-P 17-18
direct outputs in SpatGRIS (in black):

Same scenario

• Potentiometer 7: ControlGRIS 13-14, BlackHole outputs 13-14, H-P 19-24
Left-right position, Azimuth Span at 50%, Elevation at top of dome:

<img src="/media-en/media/image144.jpg"
style="width:1.94032in;height:1.8in" /><img src="/media-en/media/image145.jpg"
style="width:1.23699in;height:1.8in" />

The left channel on odd-numbered hp (in light orange) and the right
channel on even-numbered hp (in darker orange):

<img src="/media-en/media/image146.jpg"
style="width:3.65482in;height:2in" />

## 10.2. Using the PLAYER without you being present

The PLAYER (see chapter 6. PLAYER) is a very powerful tool in *SpatGRIS*
which allows you to record a project in the original setup and then play
it in another setup, in a concert hall for example. A typical situation
is when one of your works is played elsewhere in your absence. You can
then record your project using the Record function (see section 5.11.
Recording) by checking the Export Speaker Setup box:

<img src="/media-en/media/image85.jpg"
style="width:4.5in;height:1.17019in" />

The audio files and the original loudspeaker setup will be saved in the
same folder. You can send this one to your destination, who could play
your piece on their own setup. This function is very useful for helping
to spread multichannel music.

## 10.3. HYBRYD mode to vary the trajectories

HYBRID mode (see section 5.7. The HYBRID mode) is actually a DOME in
which sources can be moved in CUBE mode. In exclusive DOME mode, the
sources must be placed on the surface of the dome. This is imposed by
the VBAP algorithm. It is therefore not possible to place a sound inside
or outside the dome. By adopting HYBRID mode, the sources can either
behave in DOME mode or in CUBE mode:

<img src="/media-en/media/image147.jpg"
style="width:4.40323in;height:0.9in" />

As can be seen here, some sources (in burgundy) are located outside the
dome, while others (in light blue) are inside it:

<img src="/media-en/media/image148.jpg"
style="width:6.5in;height:4.23542in" />

HYBRID mode allows you to vary the trajectories in DOME mode.

# Index

2

256 inputs and outputs · 8

3

3D and 2D views · 52

A

access to the microphone · 9

Activate · 26

AIFF is limited to 2 GB · 44

AIFF or WAV · 43

Alt for Windows · 50

Apple Silicon M1-M2 · 8, 10

automated presets · 26

automated trajectories · 26

Azimuth-Distance and Elevation · 19

Azimuth-Elevation · 18

B

Back & Forth · 24

BINAURAL · 43

*BlackHole* · 8

Buffer size · 11, 31

C

Cartesian (CUBE) · 18

Catalina · 8

CPU usage · 53

CUBE · 16

D

dampening · 24

Deviation · 24

Document format warnings · 52

DOME · 16

DP · 10

Drawing · 25

E

Extended Top · 20

Extended Top and Bottom · 21

F

Filtering (Hz) · 35

First Source ID · 17

G

Gaël Lane Lépine · 17

Global Sound Diffusion · 37

H

Head Related Transfer Function (HRTF) · 43

HYBRID mode · 32

I

Independent direct outputs · 39

Interpolation · 53

IP Address · 17

J

*Jack* · 8

L

Lemur · 8, 18, 59

Logic Pro · 10, 61

M

Matrix Base Amplitude Panning · 32

MBAP · 37

microphone · 9

MIDI tempo · 24

minimal requirements · 38

multiclient · 13

Mute and Solo · 42

O

*OctoGris* · 9

Olivier Bélanger · 17

Open Documentation · 53

Open Stage Control · 8, 18, 59

Option (Opt) for Mac · 50

OSC channels · 18

OSC Input Port · 31

OSC Input port number · 57

output level · 13

P

peak · 42

pendulum · 26

performance · 53

polar (DOME) · 18

R

*Reaper* · 61

*ReaRoute* · 8

Record button · 44

Reset Meter Clipping · 42, 51

Reset Sources Position · 51

S

Samuel Béland · 39

Save Project · 28

Save Settings · 28

Save Speaker Setup · 28

Security & Privacy · 9

server address · 57

Shift-Click in Drawing mode · 25

Show Speaker Numbers · 40

Show Speaker Triplets · 32

Sources Link descriptions · 54

Sources tab · 17

Spans · 20, 52, 53

*SpatGris1* · 10, 60

Spatialized direct outputs · 39

Speakers’ order · 37

*SpeakerView.* · 29

STEREO · 42

subwoofers · 39

T

The threshold is set at -70 dB · 50

Trajectories · 22

Trajectory descriptions · 56

U

uninstall *ControlGRIS* · 59

uninstall *SpatGRIS* · 59

V

VBAP · 17

Vector Base Amplitude Panning · 32

Ville Pulkki · 17

Volume (dB): · 35

W

WAV is limited to 4 GB · 44

X

xml format · 51

Z

*ZirkOSC* · 9

[1] *BlackHole* is not mandatory. Any software that can send audio to
*SpatGRIS* can be used. *BlackHole* is a HAL plugin.

[2] See the format of the OSC messages in the Addendum.

[3] JackRouter is a HAL plugin that was not compatible with MacOS 10.15
and up, and was not supported for a while.

[4] Designed by Christophe Lengelé

[5] See this link for more information: https://jackaudio.org/downloads/

[6] Open Sound Control

[7] The AAX plugin for Windows is signed using a self-issued
certificate. It is unclear for now whether this is sufficient for
ProTools and/or Windows Defender.

[8] Since version 3.2.0, the LBAP, Layer Base Amplitude Panning,
designed by Olivier Bélanger, is not in use anymore.

[9] <http://opensoundcontrol.org>

[10] See the Addendum manual for more information.

[11] See the Open Stage Control manual for that:
https://openstagecontrol.ammd.net/

[12] On the Mac, most keyboards use Option (Opt), while others use Alt.
Opt will be used in this manual.

[13] It seems that on some Azerty keyboard, this key combination is not
working. The function is still available though.

[14] CAF (Core Audio Format) and WAV RF64 will eventually be implemented
enabling size to exceed 4 GB.
