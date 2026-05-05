■ main_cDR_v3.py:

The function that calculates the expected data rate, shown in eq.(11) of the submitted paper.
Available for the 2 types of the PPCP classes; Thomas point process (->TCP) and Mattern cluster process (->MCP).
1st argument: the system parameter set csv; see "param_set_example.csv".
2nd argument: the PPCP class indicator; TCP(tcp)/MCP(mcp).
Run this script AFTER running "main_cDR-per-period_v3.py" and making an empty directory named "database/" (otherwise this script does not work).
 - Running command example: mkdir database/; python main_cDR_v3.py param_set_example.csv MCP
Required modules: sys, csv, time, NumPy, SciPy, func_MeanPeriod_v3 (just put "func_MeanPeriod_v3.py" on the same directory)

Operation confirmed in Python 3.12.3.

■ main_cDR-per-period_v3-d200.py:

The function that calculates the expected received data in a cycle, shown in eq.(9) of the submitted paper.
 > "d200" implies the numerical resolution Pattern~2; see Table~A.3 of the submitted paper.
Available for the 2 types of the PPCP classes; Thomas point process (->TCP) and Mattern cluster process (->MCP).
1st argument: the system parameter set csv; see "param_set_example.csv".
2nd argument: the PPCP class indicator; TCP(tcp)/MCP(mcp).
 - Running command example: python main_cDR-per-period_v3.py param_set_example.csv MCP
Required modules: sys, csv, time, NumPy, SciPy, func_MeanPeriod_v3 (just put "func_MeanPeriod_v3.py" on the same directory)

Operation confirmed in Python 3.12.3.

■ main_cHOR_v3-d200.py:

The function that calculates the expected longterm average of the handover rate, shown in eq.(11) of the submitted paper.
 > "d200" implies the numerical resolution Pattern~2; see Table~A.3 of the submitted paper.
Available for the 2 types of the PPCP classes; Thomas point process (->TCP) and Mattern cluster process (->MCP).
1st argument: the system parameter set csv; see "param_set_example.csv".
2nd argument: the PPCP class indicator; TCP(tcp)/MCP(mcp).
 - Running command example: python main_cHOR_v3-d200.py param_set_example.csv
Required modules: sys, csv, random, time, NumPy, SciPy, func_MeanPeriod_v3 (just put "func_MeanPeriod_v3.py" on the same directory)

Operation confirmed in Python 3.12.3.
