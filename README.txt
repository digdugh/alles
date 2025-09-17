Kepler-34 (KIC 8572936) — allesfitter starter pack
--------------------------------------------------
FILES
- settings.csv  : allesfitter run settings
- params.csv    : initial parameters & priors for the eclipsing binary
- KEPLER.csv    : example CSV with columns: time,flux,flux_err (replace with your data)

NOTES
• Time should be in days; for Kepler, use BJD−2454833. If you use absolute BJD, adjust B_epoch accordingly.
• Starter values based on literature: P_bin≈27.7958103 d, e≈0.52, i≈89.86°, (R_A+R_B)/a≈0.0458, R_B/R_A≈0.9405.
• Replace KEPLER.csv with your Lightkurve-exported data (normalized near unity).

HOW TO RUN
import allesfitter
allesfitter.show_initial_guess('PATH_TO_THIS_FOLDER')
allesfitter.ns_fit('PATH_TO_THIS_FOLDER')
allesfitter.ns_output('PATH_TO_THIS_FOLDER')
