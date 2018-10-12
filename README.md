**Supporting information**

**1. Files**

`thermoML_search.ipynb`

    Jupyter notebook that curates the ThermoML database and fetches the infinite dilution activity coefficients.

`correct_systems_and_thermoML_activities.pickle` and `correct_systems_and_thermoML_activities.json`

    Files containing data extracted from the ThermoML database.
    
`create_input.ipynb`

    Jupyter notebook that creates the input files for the Orion simulations.
    
`general.yaml`

    General YANK input files containing free energy calculation and simulation parameters.
    
`results_final.oeb.gz`

    OpenEye binary containing the results of the simulations
    
`results_idac.pickle` and `results_idac.json`

    Files containing the results of the simulations in a more accessible format. (Python, Pickle 3.X)

`data_analysis_and_plots.ipynb`

    Jupyter notebook containing analysis script.

`tools.py`

    Python script with statistical tools used in `data_analysis_and_plots.ipynb`.


**2. How to access the IDAC data**

You should have Python 3.5 installed with the `pandas` package. The data is stored in `pandas.DataFrame` objects and can be retrieved by the following commands:

```
import pandas as pd

data = pd.read_pickle(`correct_systems_and_thermoML_activities.pickle`)
data = pd.read_json(`correct_systems_and_thermoML_activities.json`)
```

**3. Software**

    - Thermopyl

    - OpenMM==7.1.1

    - OpenMolTools==0.8.1

    - ambermini==16.16.0

    - Parmed==2.7.3

    - Yank==0.20.1

    - oeommtools==0.14.0

    - OpenEye-Toolkits==2018.2.1

    - PACKMOL==17.221

    - oenotebook

* Thermopyl currently does not run in Python 3.5

