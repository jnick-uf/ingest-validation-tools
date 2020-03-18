# codex

Related files:
- [JSON Schema](schema.yaml)
- [TSV Template](template.tsv)

## `donor_id`
HuBMAP ID of the donor of the assayed tissue.

## `parent_id`
HuBMAP ID of the assayed tissue.

## `execution_datetime`
Start date and time of assay. YYYY-MM-DD hh:mm ZZZ”, where YYYY is the year, MM is the month with leading 0s, and DD is the day with leading 0s, hh is the hour with leading zeros, mm are the minutes with leading zeros, and ZZZ is the three letter timezone abbreviation.

## `protocols_io_doi`
DOI for protocols.io referring to the protocol for this assay.

## `operator`
Name of the person responsible for executing the assay.

## `operator_email`
Email address for the operator.

## `pi`
Name of the principal investigator responsible for the data.

## `pi_email`
Email address for the principal investigator.

## `assay_category`
Each assay is placed into one of the following 3 general categories: generation of images of microscopic entities, identification & quantitation of molecules by mass spectrometry, and determination of nucleotide sequence.

## `assay_type`
The specific type of assay being executed.

## `analyte_class`
Analytes are the target molecules being measured with the assay.

## `is_targeted`
Specifies whether or not a specific molecule(s) is/are targeted for detection/measurement by the assay .The CODEX analyte is protein.

## `acquisition_instrument_vendor`
An acquisition_instrument is the device that contains the signal detection hardware and signal processing software. Assays generate signals such as light of various intensities or color or signals representing molecular mass.

## `acquisition_instrument_model`
Manufacturers of an acquisition instrument may offer various versions (models) of that instrument with different features or sensitivities. Differences in features or sensitivities may be relevant to processing or interpretation of the data.

## `resolution_x_value`
The width of a pixel. (Akoya pixel is 377nm square)

## `resolution_x_unit`
The unit of measurement of width of a pixel.(nm)

## `resolution_y_value`
The height of a pixel. (Akoya pixel is 377nm square)

## `resolution_y_unit`
The unit of measurement of height of a pixel. (nm)

## `resolution_z_value`
Optional if assay does not have multiple z-levels. Note that this is resolution within a given sample: z-pitch (resolution_z_value) is the increment distance between image slices (for Akoya, z-pitch=1.5um) ie. the microscope stage is moved up or down in increments of 1.5um to capture images of several focal planes. The best one will be used & the rest discarded. The thickness of the sample itself is sample metadata.

## `resolution_z_unit`
The unit of incremental distance between image slices.(um)

## `preparation_instrument_vendor`
The manufacturer of the instrument used to prepare the sample for the assay.

## `preparation_instrument_model`
The model number/name of the instrument used to prepare the sample for the assay

## `number_of_antibodies`
Number of antibodies

## `number_of_cycles`
Number of cycles of 1. oligo application, 2. fluor application, 3. washes

## `section_prep_protocols_io_doi`
DOI for protocols.io referring to the protocol for preparing tissue sections for the assay.

## `reagent_prep_protocols_io_doi`
DOI for protocols.io referring to the protocol for preparing reagents for the assay.

## `metadata_path`
Relative path to file or directory with free-form or instrument/lab specific metadata. Optional.

## `data_path`
Relative path to file or directory with instrument data. Downstream processing will depend on filename extension conventions. Required.
