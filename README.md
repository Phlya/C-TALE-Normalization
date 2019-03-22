# C-TALE-Normalization
Code and examples for C-TALE normalization.
# Usage:
python2 C-TALE-normalize.py cool_file chr ROI_start ROI_end resolution coeffitient output_cool_file


cool_file - Cool file with C-TALE HiC map.

chr, ROI_start, ROI_end - Genomics coordinates in bp of Region of interest. <chr> can be number or letter if you generate cool using hiclib.

resolution -resolution of C-TALE HiC map in bp.

coefficient - float that will be used for multiplicating around ROI (see original manuscript).

output_cool_file - name of new cool file that will be generated.

# IMPORTANT
Script generate new file with normalized matrix, but delete raw matrix. So for parsing cool file you should use balance=False.
We fix this in future.
