## Caillet et al. (2022)

Paper submitted to JGR Oceans

* NEMO-3.6 : dev_r5151_UKMO_ISF branch at revision 5932. Initial configuration produced by Nicolas Jourdain.
  
* Very few personal customizations (in MY_SRC)

* Configuration name : AMUXL025.L75. (1/4°, 75 vertical levels)

* Original simulation names: 
   - nemo\_AMUXL025\_REFERENCE (1958-2018, reference case)
   - nemo\_AMUXL025\_SXX\_PREC*_SLP (1958-2018, precipitation perturbed cases)
     with XX a number and * in (048, 06, 07, 08, 09, 141, 199) which correspond respectively to the multiplying factor (0.48, 0.6, 0.7, 0.8, 0.9, 1.41, 1.99) 
   - nemo\_AMUXL025\_SXX\_TEMP*_SLP (1958-2018, temperature perturbed cases)
     with XX a number and * in (m10, m5, m25, m1, m05, p2, p5, p10) which correspond respectively to the shift factor (-10°C, -5°C, -2.5°C, -1°C, -0.5°C, +2°C, +5°C, +10°C) 
   - nemo\_AMUXL025\_SXX\_WIND*_SLP (1958-2018, wind perturbed cases)
     with XX a number and * in (47dN, 2degN, 1degN, 05dN, 12degS, 24degS, 47degS) which correspond respectively to the shift factor (4.7°N, 2.35°N, 1.18°N, 0.5°N, 1.18°S, 2.35°S, 4.7°S)
   - nemo\_AMUXL025\_S19\_TOT_TEMPm05 (1958-2018, overall perturbed cases, climate -0.5°C)
     which correspond to the current climate -0.5°C (TEMP -0.5°C, WIND shifted by 0.24°N , PREC x 0.96) 
   - nemo\_AMUXL025\_SXX\_REVERSIBLE (1958-2018, cold-to-warm reversible cases)
     with XX the corresponding number of the studied configuration
   - nemo\_AMUXL025\_SXX\_REVERSIBLE_WC (1958-2018, warm-to-cold reversible cases)
     with XX the corresponding number of the studied configuration
   - nemo\_AMUXL025\_SXX\_ACCUMULATION (1958-2018, verification of the accumulation phenomenon)
     with XX the corresponding number of the studied configuration 
     
* See ocean and sea-ice model parameters in files:
   - cpp_AMU12r_htau_flux.fcm (for all cases except wind perturbed configuration) and cpp_AMU12r_wind.fcm (for wind perturbed configuration)
   - namelist_nemo_GENERIC_AMUXL025 
   - namelist_ice_nemo_GENERIC_AMUXL025


* Output and forcing files available on request to <justine.caillet@univ-grenoble-alpes.fr> 
