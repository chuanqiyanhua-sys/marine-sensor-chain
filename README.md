# Supporting Data for the Marine Sensor Chain Deployment and Retrieval System

## Overview

This dataset accompanies the manuscript entitled *Design of an Automatic Control System for Marine Sensor Chain Deployment and Retrieval*. It provides selected numerical data associated with the winch retrieval tests and the temperature-calibration results presented in the manuscript.

The dataset is organized by the corresponding manuscript tables and figures. It contains reported test summaries, averaged calibration measurements, and processed values used to generate a plotted residual curve.

## Data files and manuscript correspondence

| File | Manuscript item | Description |
| --- | --- | --- |
| [winch_retrieval_data.csv](winch_retrieval_data.csv) | Table 2 and Figures 11–12 | Reported retrieval-test values for three motor-speed settings. The time per unit length is calculated from the reported retrieval time and cable length. |
| [temperature_calibration_data.csv](temperature_calibration_data.csv) | Figure 13(a), measured markers | Eight calibration points, represented by the mean thermistor resistance and mean reference-temperature reading at each nominal setpoint. |
| [temperature_residuals.csv](temperature_residuals.csv) | Figure 13(b) | 733 temperature–residual pairs used for the plotted fitting-residual curve. |

## Column definitions

### `winch_retrieval_data.csv`

| Column | Description | Unit |
| --- | --- | --- |
| `motor_speed_r_min` | Motor-speed setting | r/min |
| `load_mass_kg` | Test load mass | kg |
| `retrieval_time_s` | Reported retrieval time | s |
| `cable_length_m` | Cable length | m |
| `retrieval_speed_reported_m_s` | Retrieval speed reported in Table 2 | m/s |
| `time_per_unit_length_s_m` | Retrieval time divided by cable length; rounded to two decimal places | s/m |

### `temperature_calibration_data.csv`

| Column | Description | Unit |
| --- | --- | --- |
| `nominal_setpoint_deg_c` | Nominal temperature setpoint | °C |
| `mean_thermistor_resistance_ohm` | Mean thermistor resistance at the setpoint | Ω |
| `mean_reference_temperature_deg_c` | Mean reference-temperature reading at the setpoint | °C |

### `temperature_residuals.csv`

| Column | Description | Unit |
| --- | --- | --- |
| `temperature_deg_c` | Temperature coordinate used in Figure 13(b) | °C |
| `fitting_residual_deg_c` | Fitting residual corresponding to the temperature coordinate | °C |

## Data format and scope

- All files are comma-separated CSV files encoded in UTF-8.
- A period (`.`) is used as the decimal separator.
- Column names are written in English and include units where applicable.
- The winch file contains reported test-summary values and a derived time-per-unit-length value.
- The calibration file contains averaged values for the eight measured markers shown in Figure 13(a); it is not a record of every individual acquisition.
- The residual file contains processed plotting values for Figure 13(b), rather than the complete raw temperature-acquisition record.

This release is limited to the data files listed above. It should not be interpreted as a complete archive of all raw measurements or intermediate calculations associated with every temperature-performance statistic reported in the manuscript.

## Dataset version and citation

The repository release or archived dataset record identifies the version of these files. When citing or reusing the dataset, please refer to the specific release associated with the manuscript. A persistent identifier and the final dataset citation should be added here once the dataset has been formally deposited and released.
